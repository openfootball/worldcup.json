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


# worldcup.json 

Free open public domain football data for the world cups (national teams and clubs) in the JSON
(JavaScript Object Notation)
data interchange format
incl. USA 2025, Qatar 2022, Russia 2018 and more - No API key required ;-).


## Clubs

Example - Club World Cup in USA 2025 Match Schedule (Fixtures and Results) - [`2025/clubworldcup.json`](https://raw.githubusercontent.com/openfootball/worldcup.json/master/2025/clubworldcup.json):

``` json
{
  "name": "Club World Cup 2025",
  "matches": [
    {
      "round": "Group A",
      "date": "2025-06-14",
      "time": "20:00",
      "team1": "Al Ahly SC (EGY)",
      "team2": "Inter Miami CF (USA)",
      "score": {
      }
    },
    {
      "round": "Group A",
      "date": "2025-06-15",
      "time": "18:00",
      "team1": "Palmeiras (BRA)",
      "team2": "FC Porto (POR)",
      "score": {
      }
    },
    ...
  ]
}
```


## National Teams

Example - World Cup in Russia 2018 Match Schedule (Fixtures and Results) - [`2018/worldcup.json`](https://raw.githubusercontent.com/openfootball/worldcup.json/master/2018/worldcup.json):

``` json
{
  "name": "World Cup 2018",
  "rounds": [
    {
      "name": "Matchday 1",
      "matches": [
        {
          "num": 1,
          "date": "2018-06-14",
          "time": "18:00",
          "team1": { "name": "Russia",       "code": "RUS" },
          "team2": { "name": "Saudi Arabia", "code": "KSA" },
          "score1":  5,
          "score2":  0,
          "score1i": 2,
          "score2i": 0,
          "goals1": [
            { "name": "Gazinsky",   "minute": 12,              "score1": 1, "score2": 0 },
            { "name": "Cheryshev",  "minute": 43,              "score1": 2, "score2": 0 },
            { "name": "Dzyuba",     "minute": 71,              "score1": 3, "score2": 0 },
            { "name": "Cheryshev",  "minute": 90, "offset": 1, "score1": 4, "score2": 0 },
            { "name": "Golovin",    "minute": 90, "offset": 4, "score1": 5, "score2": 0 }
          ],
          "goals2": [],
          "group": "Group A",
          "stadium": { "key": "luzhniki", "name": "Luzhniki Stadium" },
          "city": "Moscow",
          "timezone": "UTC+3"
        }
      ]
    },
    {
      "name": "Matchday 2",
      "matches": [
        {
          "num": 2,
          "date": "2018-06-15",
          "time": "17:00",
          "team1": { "name": "Egypt",   "code": "EGY" },
          "team2": { "name": "Uruguay", "code": "URU" },
          "score1":  0,
          "score2":  1,
          "score1i": 0,
          "score2i": 0,
          "goals1": [],
          "goals2": [
            { "name": "Giménez",  "minute": 89,  "score1": 0, "score2": 1 }
          ],
          "group": "Group A",
          "stadium": { "key": "ekaterinburg", "name": "Ekaterinburg Arena" },
          "city": "Ekaterinburg",
          "timezone": "UTC+5"
        },
        ...
      ],
    },
  ],
}
```


## How to Use the Public JSON HTTP API (Micro) Web Service - No API Key Required ;-)

Use the "raw" links served by GitHub (otherwise you get the complete "formatted" GitHub web page).
Example:

```
$ curl https://raw.githubusercontent.com/openfootball/worldcup.json/master/2025/clubworldcup.json
```


## Updates / Contributions Welcome - Please Update the Source Text Files

Note: The JSON files get (auto-)generated using the football.db datasets, thus, **please do NOT
edit the JSON files but the source text files in the world cup (and friends) repos** e.g.:

Clubs:
- Club World Cups in [`/club-worldcup`](https://github.com/openfootball/club-worldcup)

Note: For the Club World Cup 2025 please update the source text file
[`/club-worldcup/2025/clubworldcup.txt`](https://github.com/openfootball/club-worldcup/blob/master/2025/clubworldcup.txt) 


National Teams:
- World Cups in [`/worldcup`](https://github.com/openfootball/worldcup)
<!--
- National Teams in [`/national-teams`](https://github.com/openfootball/national-teams)
- Stadiums in [`/stadiums`](https://github.com/openfootball/stadiums)
- and so on
-->

Note: For the World Cup 2022 please update the source text file
[`/worldcup/2022--qatar/cup.txt`](https://github.com/openfootball/worldcup/blob/master/2022--qatar/cup.txt) for the group stage and
[`/worldcup/2022--qatar/cup_finals.txt`](https://github.com/openfootball/worldcup/blob/master/2022--qatar/cup_finals.txt) for the knockout (quarter-finals, semi-finals, etc.) stage.



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

### World Cup 2018

_Yes, you're more than welcome to send a pull request (PR) with your project!_

* https://github.com/sportdb/footty -- command line tool in ruby; shows todays' matches or yesterdays' or tomorrows' or all past or all upcoming

* https://github.com/geeknat/heyrussia -- command line tool in go; shows matches, stadiums, groups, standings, etc.


_Feel free to add your project here!_

## Questions? Comments?

Yes, you can. More than welcome.
See [Help & Support »](https://github.com/openfootball/help)
