# world-cup.json

Free open public domain football data for the world cups in the JSON
(JavaScript Object Notation)
data interchange format
incl. Russia 2018 and more - No API key required ;-).



Example - World Cup in Russia 2018 Match Schedule (Fixtures and Results) - [`2018/worldcup.json`](https://raw.githubusercontent.com/openfootball/world-cup.json/master/2018/worldcup.json):

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
$ curl https://raw.githubusercontent.com/openfootball/world-cup.json/master/2018/worldcup.json
```


## Projects in the Real-World Using world_cup.json 

### World Cup 2018

_Feel free to add your project! Yes, you're more than welcome to send a pull request (PR) with your project!_


* https://github.com/sportdb/footty
(command line tool in ruby; shows today's matches or yesterday's or tomorrows or all past or all upcoming)

* https://github.com/geeknat/heyrussia
(command line tool in go; shows matches, stadiums, groups, standings, etc.)  



## Updates / Contributions Welcome - Please Update the Source Text Files

Note: The JSON files get (auto-)generated using the football.db datasets, thus, **please do NOT
edit the JSON files but the source text files in the world cup (and friends) repos** e.g.:

- World Cups in [`/world-cup`](https://github.com/openfootball/world-cup)
- National Teams in [`/national-teams`](https://github.com/openfootball/national-teams)
- Stadiums in [`/stadiums`](https://github.com/openfootball/stadiums)
- and so on


Note: For the World Cup 2018 please update the source text file
[`/world-cup/2018--russia/cup.txt`](https://github.com/openfootball/world-cup/blob/master/2018--russia/cup.txt) for the group stage and
[`/world-cup/2018--russia/cup_finals.txt`](https://github.com/openfootball/world-cup/blob/master/2018--russia/cup_finals.txt) for the knockout (quarter-finals, semi-finals, etc.) stage.




## Automate, Automate, Automate

If all works (almost) daily updates get pushed by yorobot.
See the [`yorobot/football.db`](https://github.com/yorobot/football.db) build scripts for
the (auto-)update machinery.


## Contributions Welcome - Add Your Leagues and Tournaments!

Any leagues or tournaments missing? Contributions welcome!
For starting your own repo from scratch see the [League Quick Starter Kit](https://github.com/openfootball/your-league-starter).



## License

![](https://publicdomainworks.github.io/buttons/zero88x31.png)

The world-cup.json schema, data and scripts are dedicated to the public domain. Use it as you please with no restrictions whatsoever.


## Questions? Comments?

Send them along to the
[Open Sports & Friends Forum/Mailing List](http://groups.google.com/group/opensport).
Thanks!
