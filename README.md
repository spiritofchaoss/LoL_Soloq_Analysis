# League of Legends Azir Soloq (Patch 10.7 - 10.13) Analysis: Project Overview

* Collect raw data from Riot API and transcribe it into more easily manipulable dataframe.
* Look at some basic stats and drawing a personal conclusion about the champion and how I play the champion
* https://na.op.gg/summoner/userName=%C3%ACrelia

# Code and Resources Used
**Python Version:** 3.7

**Packages:** pandas, matplotlib, riotwatchers

**Riot API Wrapper Used:** https://riot-watcher.readthedocs.io/en/latest/

**Using Riot API Article:** https://towardsdatascience.com/how-to-use-riot-api-with-python-b93be82dbbd6

**Data Dragon Riot API Library:** https://riot-api-libraries.readthedocs.io/en/latest/ddragon.html

# Data Collection
Used RiotWatcher wrapper (above) to collect data from Riot API. Data include but are not limited to:
* TeamId  
* ParticipantId
* Champion 
* Role
* Lane
* Summoner Spells
* Items
* Wins
* Kills
* Deaths
* Assists
* etc...

Also converted Id to names of its corresponding champion, rune, and item names using DDragon (above)

# Data Cleaning
After collecting a total of ~100 games yielding 1000 rows (10 players per game) I made the following changes to narrow the csv file down to only rows containing games where I played Azir. Changes made include:
* Changed Unnamed: 0 column to summonerId
* Parsed out only the summoner name
* Located and kept only rows where summonerId was me and champion played was Azir

# Exploratory Data Analysis
Most stats were fairly clean and needed minimal editing. Looked deeper into combined stats using mostly value_counts() and describe().
Here is a simple snapshot of what I have found (only applies to me, how I pilot this champion, and some personal statistics).

<img src="Images/ss, keystone, items.png"

* I am fixed on the way I play. I choose same summoner spells, keystones, items majority of the time. Perhaps if I be alittle more flexible to specific matchups or try variations on builds, runes, and spells I may yield different results.


