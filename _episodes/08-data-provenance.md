---
title: "Capturing Provenance"
teaching: 25
exercises: 10
questions:
- "What should I be recording while I do my analyses?"
objectives:
- "Train yourself to record important metadata needed for"
keypoints:
- "You can't go back in time and collect some kinds of metadata. You have to keep good notes and records."
---

## Where are we?

Now we are going to talk about what you can do during the Analysis phase of your data life cycle to implement FAIR practices.

<img src="../fig/datalifecycle-analysis.png" alt="datalifecycle-analysis" style="zoom:30%;" />

## Provenance

Have you ever come back to plots or data you created and have no idea how you make them? At that point the provenance is gone.  You can't go back in time and collect some kinds of metadata. You have to keep good notes and records while you work with your data.

## What to keep in mind during your analyses

- **Document where you get your source data** so you can cite it later.  If you collected it yourself, make sure you have all the metadata about how, when, and where you collected it. Keep notes about what processing you do to the data. 
- **Keep your source data separate from your analysis tables**. Never manipulate your source data during your analyses! Make a separate copy for manipulating however you need to during the analyses. Make a system to keep track of your workflow and identify different data tables.  This can be a formal version control system (e.g. git/github) or a documented plan for folder and file naming conventions along with notes.
- **Write notes like you are explaining it to someone else.**  Look at your plots and data and pretend you are stepping someone else through how you would produce the same thing.  Even if you come back to it yourself in the future, it's likely you would have forgotten all the details. Help yourself out with good documentation.
- **Record the filename and path you save to.** Make it clear what was done to produce each file. 

> Example notes:
> 
> 2022-06-22: 
> Downloaded a subset of dataset "Niskin bottle samples" which spans 2004 to 2008 to folder "BATS_niskin/orig/bcodmo_dataset_3782_2004_to_2008.csv"
> 
> data source citation:
> Johnson, R. (2019) Niskin bottle water samples and CTD measurements at water sample depths collected at Bermuda Atlantic Time-Series sites in the Sargasso Sea ongoing from 1955-01-29 (BATS project). Biological and Chemical Oceanography Data Management Office (BCO-DMO). (Version 1) Version Date 2019-05-29 [Subset 2004 to 2008]. http://lod.bco-dmo.org/id/dataset/3782 [Accessed on 2022-06-22]
>
> Data were binned data by hour, ordered table by station, cast, pressure and saved to "BATS_niskin_2004_to_2008/hourly/BATS_niskin_hourly.xlsx" 
> * exported Sheet 1 to "BATS_niskin_2004_to_2008/hourly/BATS_niskin_hourly.csv." 
> * exported plot in Sheet 2 to "BATS_niskin_2004_to_2008/hourly/BATS_profiles.png"

Having clear records about how a plot was produced with the table you used to produce it is very important for reports and journal publications.  It allows your results to be reproducible, transparent, and fascilitate peer review. It also makes writing your publication easier since you already have the figure captions written!

## Anyone can create metadata

You don't need any special skills to write metadata and documentation to keep track of your provenance.  

However, there are specifications and tools you can learn that have huge benefits.   See more about metadata specifications like [PROV](https://www.w3.org/2001/sw/wiki/PROV).

**Version control** (e.g. git/github) is a great way to keep track of all the changes in your files.  It does have a learning curve but will save you time and frustration in the long run after you learn it. 

I'm sure everyone has experienced this frustration:

> ![version_control_meme](../fig/ew-versions.png)
> from: Wit and wisdom from Jorge Cham (http://phdcomics.com/)

Git will keeps track of all the differences in your files over time, no need to keep a million copies!  You can make notes for each version of your files too.

> Learn more about [Version Control and Git in a Software Carpentry](https://swcarpentry.github.io/git-novice/).
