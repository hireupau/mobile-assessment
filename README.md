# Mobile-assessment - Searchable Select List

## Overview
We'd like you to create a searchable select list that retrieves Marvel characters from our Superhero API.

The following designs were created for a progressive web app test that can be
viewed here: https://github.com/hireupau/frontend-assessment.

For this task you are expected to create a native iOS equivalent. It does
not need to match exactly but should follow as closely as is reasonably possible
taking into account the differences between a PWA and a native app.

## Prerequisites
1. Node.js and NPM installed on your local machine

## API set-up

Within this repo is an api folder that contains a script for running a local rest-api and some data.

The server can be started with:

```npm install```

```npm start```

### Request

To retrieve a list of all characters:

```GET http://localhost:1337/superheroes ```

To query for characters by their name:

```GET http://localhost:1337/superheroes?name_like=Iron```

This can be combined with filtering by other fields

```GET http://localhost:1337/superheroes?name_like=Iron&work.base_like=New%20York```

Details and more advanced queries can be found [here](https://github.com/typicode/json-server#routes)


### Response

An example response can be seen below.

```json
[
  {
    "id": 345,
    "name": "Iron Fist",
    "slug": "345-iron-fist",
    "powerstats": {
      "intelligence": 75,
      "strength": 55,
      "speed": 33,
      "durability": 50,
      "power": 95,
      "combat": 100
    },
    "appearance": {
      "gender": "Male",
      "race": "Human",
      "height": [
        "5'11",
        "180 cm"
      ],
      "weight": [
        "175 lb",
        "79 kg"
      ],
      "eyeColor": "Blue",
      "hairColor": "Blond"
    },
    "biography": {
      "fullName": "Danny Rand",
      "alterEgos": "No alter egos found.",
      "aliases": [
        "Daredevil",
        "Daniel Thomas Rand",
        "the Living Weapon",
        "Young Dragon",
        "Danny Rand"
      ],
      "placeOfBirth": "-",
      "firstAppearance": "Marvel Premiere #15 (May 1974)",
      "publisher": "Marvel Comics",
      "alignment": "good"
    },
    "work": {
      "occupation": "Adventurer; formerly co-owner of Rand-Meachum, Inc., bodyguard, private investigator, research assistant, warrior",
      "base": "New York"
    },
    "connections": {
      "groupAffiliation": "New Avengers, Heroes for Hire, Inc., Secret Defenders, Defenders, Misty Knight, Luke Cage",
      "relatives": "Wendell Rand-K'ai (father, deceased), Heather Duncan Rand (mother, deceased), Yu-Ti (adopted uncle), Miranda Rand-K'ai (half-sister), Lord Tuan (adopted paternal grandfather, deceased), Lady Ming (adopted paternal grandmother, deceased), Thomas Duncan (maternal grandfather)"
    },
    "images": {
      "xs": "https://cdn.rawgit.com/akabab/superhero-api/0.2.0/api/images/xs/345-iron-fist.jpg",
      "sm": "https://cdn.rawgit.com/akabab/superhero-api/0.2.0/api/images/sm/345-iron-fist.jpg",
      "md": "https://cdn.rawgit.com/akabab/superhero-api/0.2.0/api/images/md/345-iron-fist.jpg",
      "lg": "https://cdn.rawgit.com/akabab/superhero-api/0.2.0/api/images/lg/345-iron-fist.jpg"
    }
  }
]
```

## Mandatory Requirements
- Must be completed in Swift
- Must contain equivalent behaviour to the PWA

## Submission
The submission should be committed to Github and a link provided to the submission along with a readme on how to setup and run the solution. The solution is expected to incorporate good software development practices such as comments and tests.

**If you have any problems with this assessment, you can create a GitHub issue that will be answered shortly by one of the Hireup development team or email us directly at tech@hireup.com.au**

## Examples

Mobile Example 1 - Closed Select
![ScreenShot4](https://i.imgur.com/KUaenjW.jpg)

Mobile Example 2 - Opened Select
![ScreenShot5](https://i.imgur.com/KAJvi1s.jpg)

Mobile Example 3 - No Results Select
![ScreenShot6](https://i.imgur.com/0938RCR.jpg)

