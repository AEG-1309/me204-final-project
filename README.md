# ME204 Final Project: Is catching them all really worth it? An analysis of power creep in Pokemon


| GitHub username                           | LSE ID            |
| ----------------------------------------- | ----------------- |
| AEG-1309                                  | 250093214         |



Remove the unused row if you work alone.
Replace every `[bracketed]` placeholder once you fill it in.

## Overview

Over its 30 years and 9 generations, has Pokemon experienced power creep? If so, to what extent?

This project was done as part of ME204, offered at LSE.

## Data sources

Primary API: [PokeAPI](https://pokeapi.co/docs/v2#info) (specifically, their Games, Pokemon Species, and Pokemon endpoints)
- Required to access: Nothing. This API is open to access for everybody, so no sign up or special API keys are required.
Supplementary Data Sources: No static data sources were used in the creation of this project, but outside information was accessed through other soruces:
- [Bulbapedia](https://bulbapedia.bulbagarden.net/wiki/Main_Page)
- ['Pokemon Database'](https://pokemondb.net/)
- [Serebii](https://www.serebii.net/)
Information about what power creep is:

Information consulted when deciding a threshold as to what constitutes a 'powerful Pokemon' in terms of BST:
- ['This post on the Smogon Forums, a competitive Pokemon-focused website'](https://www.smogon.com/forums/threads/the-pok%C3%A9mon-bst-power-hierarchy.3774319/)
- ['This post on the GameFAQs Forums'](https://gamefaqs.gamespot.com/boards/696959-pokemon-x/67994675)
- ['This post on the Pokemon Database Forums'](https://pokemondb.net/pokebase/414499/minimum-values-pokemon-considered-attacker-defender-speedster)
- ['This other post on the Pokemon Databse Forums'](https://pokemondb.net/pokebase/355610/what-pokemon-have-the-best-stat-totals-of-each-type)
- ['This Reddit thread'](https://www.reddit.com/r/stunfisk/comments/11lee7z/how_high_does_a_pok%C3%A9mons_stat_need_to_be/)
- ['This other Reddit threat'](https://www.reddit.com/r/VGC/comments/1927er0/what_are_considered_good_base_stats_and_totals/)
- ['This post on the Bulbagarden Forums'](https://bulbagarden.net/threads/what-do-you-consider-to-be-a-high-base-stat-total.153779/)
- ['This base stat guide on the Marriland webiste, a website focused on all things Pokemon'](https://marriland.com/glossary/base-stats/)

## How to reproduce

To access the APIs used for this data exploration, you will need to go to the PokeAPI [Docs](https://pokeapi.co/docs/v2#info). The specific API endpoints you will need are the [Games endpoint](https://pokeapi.co/docs/v2#games-section) to get the list of Pokemon introduced in each generation, the [Pokemon Species endpoint](https://pokeapi.co/docs/v2#pokemon-species) to get information about all of a Pokemon's alternate forms, as well as their status of whether they are legendary or mythical, and the [Pokemon endpoint](https://pokeapi.co/docs/v2#pokemon) to get all of a Pokemon's stats. The Games and Pokemon Species endpoints will provide API calls that will lead you to the next endpoint in the series, so there is no need to fetch all of them from the docs, but the docs will provide valuable information about what data each API endpoint actually returns.

In terms of Python libraries, you will need the json, requests, pandas, and plotly.express libraries. These libraries, as well as import statements, are provided at the top of every notebook. If the import statements do not work, then you will have to run a !pip install for each individual libraries. These are not included at the top of each notebook.

In terms of Python skills, you will need at least basic knowledge of how Pandas and Plotly works, Python functions, and how to import, load, and read .json files in Python. My code will be easier to read and understand with knowledge of how to do these things in Python.
