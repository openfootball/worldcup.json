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
          "team1": {
            "key": "rus",
            "name": "Russia",
            "code": "RUS"
          },
          "team2": {
            "key": "ksa",
            "name": "Saudi Arabia",
            "code": "KSA"
          },
          "score1": null,
          "score2": null,
          "score1i": null,
          "score2i": null,
          "score1et": null,
          "score2et": null,
          "score1p": null,
          "score2p": null,
          "knockout": false,
          "group": "Group A",
          "ground": null
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
          "team1": {
            "key": "egy",
            "name": "Egypt",
            "code": "EGY"
          },
          "team2": {
            "key": "uru",
            "name": "Uruguay",
            "code": "URU"
          },
          "score1": null,
          "score2": null,
          "score1i": null,
          "score2i": null,
          "score1et": null,
          "score2et": null,
          "score1p": null,
          "score2p": null,
          "knockout": false,
          "group": "Group A",
          "ground": null
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





## Automate, Automate, Automate

Note: The JSON files get (auto-)generated using the football.db datasets, thus, please do NOT
edit the JSON files but the source files in the world cup (and friends) repos e.g.:

- World Cups in [`/world-cup`](https://github.com/openfootball/world-cup)
- National Teams in [`/national-teams`](https://github.com/openfootball/national-teams)
- Stadiums in [`/stadiums`](https://github.com/openfootball/stadiums)
- and so on


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
