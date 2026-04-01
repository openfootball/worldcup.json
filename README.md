
<!--

## What's News?

Tip - You can now use the [`fbtxt2json` command-line tool](https://github.com/sportdb/footty/tree/master/fbtxt2json) to convert any file in the Football.TXT format to JSON. 

Let's try to convert the Club World Cup 2025
in the Football.TXT format (see [`club-worldcup/2025/clubworldcup.txt`](https://github.com/openfootball/club-worldcup/blob/master/2025/clubworldcup.txt)) to JSON:

```
$ fbtxt2json club-worldcup/2025/clubworldcup.txt -o clubworldcup.json
```

Or let's try to convert the World Cup 2022
in the Football.TXT format (see [`worldcup/2022--qatar/cup.txt`](https://github.com/openfootball/worldcup/blob/master/2022--qatar/cup.txt), [`worldcup/2022--qatar/cup_finals.txt`](https://github.com/openfootball/worldcup/blob/master/2022--qatar/cup_finals.txt)) to JSON:

```
$ fbtxt2json worldcup/2022--qatar/cup.txt worldcup/2022--qatar/cup_finals.txt -o worldcup.json
```

-->


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
    "group": "Group A",
    "ground": "Mexico City"
   },
   {"round": "Matchday 1",
    "date": "2026-06-11",
    "time": "20:00 UTC-6",
    "team1": "South Korea",
    "team2": "Czech Republic",
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
     [{"name": "Enner Valencia", "minute": 16, "penalty": true},
      {"name": "Enner Valencia", "minute": 31}],
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
     [{"name": "Cody Gakpo", "minute": 84},
      {"name": "Davy Klaassen", "minute": 90, "offset": 9}],
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
     [{"name": "Lionel Messi", "minute": 23, "penalty": true},
      {"name": "Lionel Messi", "minute": 108},
      {"name": "Ángel Di María", "minute": 36}],
    "goals2": 
     [{"name": "Kylian Mbappé", "minute": 80, "penalty": true},
      {"name": "Kylian Mbappé", "minute": 81},
      {"name": "Kylian Mbappé", "minute": 118, "penalty": true}],
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



## Updates / Contributions Welcome - Please Update the Source Text Files

Note: The JSON files get (auto-)generated using the football.db datasets, thus, **please do NOT
edit the JSON files but the source text files in the world cup (and friends) repos** e.g.:


National Teams:
- World Cups in [`/worldcup`](https://github.com/openfootball/worldcup)
<!--
- National Teams in [`/national-teams`](https://github.com/openfootball/national-teams)
- Stadiums in [`/stadiums`](https://github.com/openfootball/stadiums)
- and so on
-->

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

The worldcup.json schema, data and scripts are dedicated to the public domain. Use it as you please with no restrictions whatsoever.




## Projects in the Real-World Using worldcup.json

_Yes, you're more than welcome to send a pull request (PR) with your project!_

### World Cup 2026


- <https://github.com/jeff-knurek/fifa26> -- iCal generation of Fifa 2026 World Cup matches

- <https://github.com/sportdb/footty> -- command line tool in ruby; shows todays' matches or yesterdays' or tomorrows' or all past or all upcoming

_Feel free to add your project here!_

<!--
### World Cup 2018

* https://github.com/geeknat/heyrussia -- command line tool in go; shows matches, stadiums, groups, standings, etc.

-->


## Questions? Comments?

Yes, you can. More than welcome.
See [Help & Support »](https://github.com/openfootball/help)
