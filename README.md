# League of Legends Azir Soloq (Patch 10.7 - 10.13) Analysis: Project Overview

* Collect raw data from Riot API and transcribe it into more easily manipulable dataframe.
* Look at some basic stats and drawing a personal conclusion about the champion and how I play the champion
* https://na.op.gg/summoner/userName=%C3%ACrelia

# Code and Resources Used
**Python Version:** 3.7

**Packages:** pandas, matplotlib, riotwatchers

**Riot API Wrapper Used:** https://riot-watcher.readthedocs.io/en/latest/

**Using Riot API Article:** https://towardsdatascience.com/how-to-use-riot-api-with-python-b93be82dbbd6

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
