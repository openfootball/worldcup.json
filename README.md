
## Update - What's news?

Q: [Updates for upcoming rounds?](https://github.com/openfootball/worldcup/issues/91)

A: sorry for the déjà vu.  yes, your help is more than welcome to fill-in the teams once known for the round of 32/16/8 etc.
please note - the datasets for the knock-out (k.o.) matches are (auto-)generated from the upstream text source 
here <https://github.com/openfootball/worldcup/blob/master/2026--usa/cup_finals.txt>    

---

thanks to [Dr. Chester Ismay](https://github.com/ismayc) (maker of [World Cup Viewer¹](https://ismayc.github.io/world-cup-viewer/)) for the upstream (auto-filler) updates getting close to post-match live score updates here!   

and thanks for your updates & corrections (old school) by hand.      

¹: yes, you can. add your projects using worldcup.json [on this page right here](#projects-in-the-real-world-using-worldcupjson).

---  

sorry for the slow start-up on day 1. good morning it was 9am here in austria when i checked in.  
please note,  the datasets are (auto-)generated from the upstream text source 
here <https://github.com/openfootball/worldcup/blob/master/2026--usa/cup.txt>    

yes, you can. you are more than welcome to help with updates upstream.  
**anyone interested, please let me know / ping me [here](https://github.com/openfootball/worldcup.json/pull/29) or [here](https://github.com/openfootball/worldcup.json/pull/30) (as an opt-in / to give me permission)** 
and i send you an invite via github for the openfootball (github) org here 
than you can edit in-place (without pull requests AND the worldcup.json gets generated via github action on commit - see the [actions log @ /worldcup](https://github.com/openfootball/worldcup/actions)). 


> [!NOTE] 
> [@upbound-web](https://github.com/openfootball/worldcup.json/issues/33) has put together an alternate "fast-updating" worldcup.json mirror. see [upbound-web/worldcup-live.json](https://github.com/upbound-web/worldcup-live.json)




## World Cup 2026 Frequently Asked Questions (FAQ) & Answers

Q: [Will it update live match data?](https://github.com/openfootball/help/issues/57)
[How live is the (worldcup.json) data?](https://github.com/openfootball/help/issues/58)

A:  Sorry, no. worldcup.json works like a wiki. everytime the upstream (source) text, that is, [`worldcup/2026--usa/cup.txt`](https://github.com/openfootball/worldcup/blob/master/2026--usa/cup.txt) gets updated (by hand), 
the [2026/worldcup.json](https://github.com/openfootball/worldcup.json/blob/master/2026/worldcup.json) 
datatset here gets automatically generated & updated (via github action - see the [actions log @ /worldcup](https://github.com/openfootball/worldcup/actions)). 

Again note the upstream (source) text updates are not live or automated. [I (Gerald Bauer)](https://github.com/geraldb) 
try to update once a day and note - I am in Austria, that is, Central European Summer Time (UTC+2).

Anyways, to guarantee updates the best way is for you to contribute and update the score yourself. yes, you can. 
Send a pull request and I will merge and happy to send you an invite to join the github org (if you agree and opt-in by saying yes) 
so you can edit "in place" from than on.

PS:  For full match details incl. line-ups, (yellow/red card) bookings, player substitutions, penalty shootouts, and more 
I will put together an (alternate) upstream (source) text - 
see [`worldcup/more`](https://github.com/openfootball/worldcup/tree/master/more) for the history from 1930 to 2022 -  but again sorry, that, page will NOT be live updated.


<!--
For, live updates try the unoffical/offical fifa api <>.
-->


> [!TIP]
>  You can use the [`fbtxt2json` command-line tool](https://github.com/openfootball/quick-starter)
>  to convert any file in the Football.TXT format to JSON (or use `fbtxt2csv` to convert to CSV).

  

# worldcup.json

Free open public domain football data for the world cups (national teams and clubs) in the JSON
(JavaScript Object Notation)
data interchange format
incl. Canada/USA/Mexico 2026, USA 2025, Qatar 2022, Russia 2018 and more - No API key required ;-).


## National Teams

Example - World Cup in Canada/USA/Mexico 2026 Match Schedule (Fixtures and Results) - [`2026/worldcup.json`](https://raw.githubusercontent.com/openfootball/worldcup.json/master/2026/worldcup.json):


``` json
{
 "name": "World Cup 2026",
 "matches": [
   {"round": "Matchday 1",
    "date": "2026-06-11",
    "time": "13:00 UTC-6",
    "team1": "Mexico",
    "team2": "South Africa",
    "score": {"ft": [2, 0], "ht": [1, 0]},
    "goals1": [{"name": "Julián Quiñones", "minute": "9"},
               {"name": "Raúl Jiménez", "minute": "67"}],
    "goals2": [],
    "group": "Group A",
    "ground": "Mexico City"
   },
   {"round": "Matchday 1",
    "date": "2026-06-11",
    "time": "20:00 UTC-6",
    "team1": "South Korea",
    "team2": "Czech Republic",
    "score": {"ft": [2, 1], "ht": [0, 0]},
    "goals1": [{"name": "Hwang In-Beom", "minute": "67"},
               {"name": "Oh Hyeon-Gyu", "minute": "80"}],
    "goals2": [{"name": "Ladislav Krejcí", "minute": "59"}],
    "group": "Group A",
    "ground": "Guadalajara (Zapopan)"
   },
   {"round": "Matchday 8",
    "date": "2026-06-18",
    "time": "12:00 UTC-4",
    "team1": "Czech Republic",
    "team2": "South Africa",
    "group": "Group A",
    "ground": "Atlanta"
   },
   {"round": "Matchday 8",
    "date": "2026-06-18",
    "time": "19:00 UTC-6",
    "team1": "Mexico",
    "team2": "South Korea",
    "group": "Group A",
    "ground": "Guadalajara (Zapopan)"
   },
   ...
   {"round": "Final",
    "date": "2026-07-19",
    "time": "15:00 UTC-4",
    "team1": "W101",
    "team2": "W102",
    "ground": "New York/New Jersey (East Rutherford)"
   }
]}
```

Example - World Cup in Qatar 2022 Match Schedule (Fixtures and Results) - [`2022/worldcup.json`](https://raw.githubusercontent.com/openfootball/worldcup.json/master/2022/worldcup.json):

``` json
{
 "name": "World Cup 2022",
 "matches":
  [{"round": "Matchday 1",
    "date": "2022-11-20",
    "time": "19:00",
    "team1": "Qatar",
    "team2": "Ecuador",
    "score": {"ft": [0, 2], "ht": [0, 2]},
    "goals1": [],
    "goals2":
     [{"name": "Enner Valencia", "minute": "16", "penalty": true},
      {"name": "Enner Valencia", "minute": "31"}],
    "group": "Group A",
    "ground": "Al Bayt Stadium, Al Khor"
   },
   {"round": "Matchday 2",
    "date": "2022-11-21",
    "time": "19:00",
    "team1": "Senegal",
    "team2": "Netherlands",
    "score": {"ft": [0, 2], "ht": [0, 0]},
    "goals1": [],
    "goals2":
     [{"name": "Cody Gakpo", "minute": "84"},
      {"name": "Davy Klaassen", "minute": "90+9"}],
    "group": "Group A",
    "ground": "Al Thumama Stadium, Doha"
  },
  ...
  {"round": "Final",
    "date": "2022-12-18",
    "time": "18:00",
    "team1": "Argentina",
    "team2": "France",
    "score": {"p": [4, 2], "et": [3, 3], "ft": [2, 2], "ht": [2, 0]},
    "goals1":
     [{"name": "Lionel Messi", "minute": "23", "penalty": true},
      {"name": "Lionel Messi", "minute": "108"},
      {"name": "Ángel Di María", "minute": "36"}],
    "goals2":
     [{"name": "Kylian Mbappé", "minute": "80", "penalty": true},
      {"name": "Kylian Mbappé", "minute": "81"},
      {"name": "Kylian Mbappé", "minute": "118", "penalty": true}],
    "ground": "Lusail Iconic Stadium, Lusail"
  }
]}
```





## Clubs

Example - Club World Cup in USA 2025 Match Schedule (Fixtures and Results) - [`2025/clubworldcup.json`](https://raw.githubusercontent.com/openfootball/worldcup.json/master/2025/clubworldcup.json):

``` json
{
 "name": "Club World Cup 2025",
 "matches":
  [{"round": "Group A",
    "date": "2025-06-14",
    "time": "20:00",
    "team1": "Al Ahly SC (EGY)",
    "team2": "Inter Miami CF (USA)",
    "score": {"ft": [0, 0]}
   },
   {"round": "Group A",
    "date": "2025-06-15",
    "time": "18:00",
    "team1": "Palmeiras (BRA)",
    "team2": "FC Porto (POR)",
    "score": {"ft": [0, 0]}
  },
  ...
  {"round": "Final",
   "date": "2025-07-13",
   "time": "15:00",
   "team1": "Chelsea FC (ENG)",
   "team2": "Paris Saint-Germain (FRA)",
   "score": {"ft": [3, 0], "ht": [3, 0]}
  }
]}
```


## How to Use the Public JSON HTTP API (Micro) Web Service - No API Key Required ;-)

Use the "raw" links served by GitHub (otherwise you get the complete "formatted" GitHub web page).
Example:

```
$ curl https://raw.githubusercontent.com/openfootball/worldcup.json/master/2026/worldcup.json
```



## Updates / Contributions Welcome - Please Update the Upstream (Source) Text Files

Note: The JSON files get (auto-)generated using the football.db datasets, thus, **please do NOT
edit the JSON files here but the upstream (source) text files in the `/worldcup` (and friends) repos** e.g.:


National Teams:
- World Cups in [`/worldcup`](https://github.com/openfootball/worldcup)

Note: For the World Cup 2026 please update the source text file
[`/worldcup/2026--usa/cup.txt`](https://github.com/openfootball/worldcup/blob/master/2026--usa/cup.txt) for the group stage and
[`/worldcup/2026--usa/cup_finals.txt`](https://github.com/openfootball/worldcup/blob/master/2026--usa/cup_finals.txt) for the knockout (quarter-finals, semi-finals, etc.) stage.


Clubs:
- Club World Cups in [`/club-worldcup`](https://github.com/openfootball/club-worldcup)

Note: For the Club World Cup 2025 please update the source text file
[`/club-worldcup/2025/clubworldcup.txt`](https://github.com/openfootball/club-worldcup/blob/master/2025/clubworldcup.txt)




<!--
## Automate, Automate, Automate

If all works (almost) daily updates get pushed by yorobot.
See the [`yorobot/football.db`](https://github.com/yorobot/football.db) build scripts for
the (auto-)update machinery.

  add how to generate your own json files from the source datasets or something?

-->


## Contributions Welcome - Add Your Leagues and Tournaments!

Any leagues or tournaments missing? Contributions welcome!
For starting your own repo from scratch see the [League Quick Starter Kit](https://github.com/openfootball/your-league-starter).



## License

The worldcup.json schema, data and scripts are dedicated to the public domain. Use as you please with no restrictions whatsoever.




## Projects in the Real-World Using worldcup.json

_Yes, you're more than welcome to send a pull request (PR) with your project!_

### World Cup 2026


- <https://github.com/jeff-knurek/fifa26> -- iCal generation of Fifa 2026 World Cup matches

- <https://github.com/Roast-Labs/World-Cup-2026-Fixtures-and-Results-Slack-Bot> -- World Cup 2026 Slack bot - a self-installing Google apps script that posts a daily message to a Slack channel every morning with last night's results and today's fixtures for the 2026 World Cup 

- <https://github.com/salah23222/worldcup2026>  -- an open-source, bilingual (Arabic/English) companion site for the 2026 World Cup

- <https://github.com/ismayc/world-cup-viewer> -- World Cup 2026 Schedule Viewer; web app showing all 104 matches of the word cup in your timezone, with where to watch, host city/stadium, a bracket, group standings, and live results

- <https://github.com/sportdb/footty> -- command line tool in ruby; shows todays' matches or yesterdays' or tomorrows' or all past or all upcoming

- <https://ganska.lat/vm2026> -- Swedish World Cup 2026 site with data based on Openfootball 

- <https://wc2026.carbine.dev> -- A model-driven 2026 World Cup prediction almanac; forecasts all 48 teams using World Football Elo and a Dixon-Coles model, in the spirit of the (much-missed) fivethirtyeight.

- <https://roy2ez.github.io/wc2026-scorers/> -- bilingual (English/Chinese) 2026 World Cup Goalscorer dashboard: top scorers, goal origins by nation/league/club with filter and search, a latest-goals feed, goal-timing charts and so on; backed by a full 1,248-player database, updated daily.

- <https://dailypythonprojects.substack.com/p/world-cup-2026-tracker-with-python>  --  we start building a World Cup 2026 Tracker - a three-day project that turns a free public football API into your own personal tournament dashboard.

- <https://observablehq.com/@ehouais/world-cup-data-viz>  --  An [Observable](https://observablehq.com) notebook that generates various data viz based on *worldcup.json* data (primarily designed for pen plotters).


_Feel free to add your project here!_

<!--
### World Cup 2018

* https://github.com/geeknat/heyrussia -- command line tool in go; shows matches, stadiums, groups, standings, etc.

-->


## Questions? Comments?

Yes, you can. More than welcome.
See [Help & Support »](https://github.com/openfootball/help)
