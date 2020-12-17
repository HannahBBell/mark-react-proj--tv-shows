---
module: React

level: 1

methods:
  - team
  - pair
  - solo

tags:
  - wip
---

# Academy Project: TV Shows

<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a>.

## Overview

You must make a React app which shows details of all of the episodes of a TV show.

The episode data will come from [TV Maze](http://www.tvmaze.com/).

## About the episode data

### Where do I get the episode data from?

Initially, you will manually save data from their [API](http://www.tvmaze.com/api) to a JSON file in your project source.

In later exercises you may be challenged to have your app dynamically `fetch` the data from the API.

In all cases, you will be working with an array of objects, each of which represents an episode of a TV show.

### What does it look like?

Here's an excerpt of [this file](https://api.tvmaze.com/shows/82/episodes) showing an example of one such episode from the list.

```js
{
    id: 4952,
    url:
      "http://www.tvmaze.com/episodes/4952/game-of-thrones-1x01-winter-is-coming",
    name: "Winter is Coming",
    season: 1,
    number: 1,
    airdate: "2011-04-17",
    airtime: "21:00",
    airstamp: "2011-04-18T01:00:00+00:00",
    runtime: 60,
    image: {
      medium:
        "http://static.tvmaze.com/uploads/images/medium_landscape/1/2668.jpg",
      original:
        "http://static.tvmaze.com/uploads/images/original_untouched/1/2668.jpg"
    },
    summary:
      "<p>Lord Eddard Stark, ruler of the North, is summoned to court by his old friend, King Robert Baratheon, to serve as the King's Hand. Eddard reluctantly agrees after learning of a possible threat to the King's life. Eddard's bastard son Jon Snow must make a painful decision about his own future, while in the distant east Viserys Targaryen plots to reclaim his father's throne, usurped by Robert, by selling his sister in marriage.</p>",
    _links: {
      self: {
        href: "http://api.tvmaze.com/episodes/4952"
      }
    }
  }
```

### Rules about the episode data

You MUST NOT edit the static episode data. If you find that the data is unsuitable (e.g. fields are missing, or have unwanted characters), you should improve your own code so that _it_ can deal with such issues at run-time.

Why? If your app is later extended to allow the downloading of episode data for any one of hundreds of possible shows, frequently updated, tidying the data by hand will NOT be a feasible solution!

## Setup

- Create a new React app on your machine called `tv-shows`. Make sure you set up with TypeScript not the JavaScript default. TODO: add link to instructions: "React project creation setup (w typescript)".

- Publish the project repo to github. Call it `tv-shows`. TODO: add link to instructions: "publishing new project repo to github".

- Set up continuous deployment of your app to [Netlify](https://netlify.app/) as `academy-yourgithubusername-tv-shows`.netlify.app where `yourgithubusername` is your github username. TODO: add link to Netlify deploy instructions.

### Setup - get the episode data:

- Download the episode data for the show "Game Of Thrones" from TV Maze API using this URL:
  https://api.tvmaze.com/shows/82/episodes

- Save the file as `episodes.json` in your project's `src` directory, and import it into your code.

- If your JSON data is all on one long line, open it in your text editor and simply save. It will format (or "pretty-print") it for easier reading.

## Project Levels

This project is broken into various levels:

- [level 100](./level-100.md)
- [level 200](./level-200.md)
- [level 300](./level-300.md)
- [level 350](./level-350.md)
- [level 400](./level-400.md)
- [level 500](./level-500.md)
- [level 999 (further work)](./level-999.md)

## Getting started

Follow the instructions in [getting-started.md](./getting-started.md)
