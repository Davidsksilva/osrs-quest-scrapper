# Old School Runescape Quest Scrapper

## Introduction

This program is a webscrapper used to retrive the following data of all osrs quests:
- Quest name
- Quest QP reward
- Quest length
- Quest membership requirement
- Quest wiki url

The website used to scrap the data was the osrs [wikia](http://oldschoolrunescape.wikia.com/wiki/Quest_info_table) quest table.

The program is written in python using xpath hierarchy, to find the apropriate data. After that, the array of quests was saved in a JSON format.

## Running

To run the program, just execute ``main.py``:
```
python main.py
```
The output will be displayed in the ``quests.json``. For example:

```
[
    {
        "name": "Black Knight's Fortress",
        "quest_points_reward": "3",
        "length": "3 Medium",
        "membership_requirement": false,
        "url": "http://oldschoolrunescape.wikia.com/wiki/Black_Knight%27s_Fortress"
    },
    {
        "name": "Cook's Assistant",
        "quest_points_reward": "1",
        "length": "2 Short",
        "membership_requirement": false,
        "url": "http://oldschoolrunescape.wikia.com/wiki/Cook%27s_Assistant"
    },
    
    ...
```
