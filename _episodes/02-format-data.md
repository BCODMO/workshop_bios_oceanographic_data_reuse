---
title: "Formatting Data Tables"
teaching: 10
exercises: 10
questions:
- "Why is formatting data tables important?"
- "Why should I track analysis?"
- "How to structure data in spreadsheets?"
objectives:
- "Understand difference between spreadsheets and lab notebooks"
- "Describe best practices for data entry and formatting in spreadsheets."
- "Apply best practices to arrange variables and observations in a spreadsheet."
keypoints:
- "Computers need to be able to understand data tables"
- "Never modify your raw data."  
- "Keep track of all of the steps you take to clean your data."  
- "Organize your data according to tidy data principles."  
---

### Spreadsheets are not lab notebooks 

We know now that we can use spreadsheets for data entry. The most **common mistake** made is **treating spreadsheet programs like lab notebooks**, that is, relying on context, notes in the margin, spatial layout of data and fields to convey information. As humans, we can (usually) interpret these things, but computers don't view information the same way, and unless we explain to the computer what every single thing means (and that can be hard!), it will not be able to see how our data fits together.

Using the power of computers, we can manage and analyze data in much more effective and faster ways, but to use that power, we have to **set up our data for the computer to be able to understand it** (and computers are very literal).

<img src="../fig/labnotes.png" alt="data-life-cycle-acquisition" style="width:70%;" />



Spreadsheet-like lab notebook:

<img src="../fig/excel-notebook.png" alt="excel-noteook" style="zoom:30%;" />



You can set things up in different ways in spreadsheets, but some of these choices can limit your ability to work with the data in other programs or have the you-of-6-months-from-now or your collaborator work with the data. These are the **interoperable and reusable parts of F.AI.I.R data principles.**

> Note: the best layouts/formats (as well as software and interfaces) for data entry and data analysis might be different. It is important to take this into account, and ideally automate the conversion from one to another.

### Keeping track of your analyses

When you're working with spreadsheets, during data clean up or analyses, it's very easy to end up with a spreadsheet that looks very different from the one you started with. In order to be able to reproduce your analyses or figure out what you did when Reviewer #3 asks for a different analysis, you should

- create a new file with your cleaned or analyzed data. **Don't modify the original dataset**, or you will never know where you started!
- **keep track of the steps you took in your clean up** or analysis. You should track these steps as you would any step in an experiment. We recommend that you do this in a plain text file stored in the same folder as the data file. 

This might be an example of a spreadsheet setup:

![spreadsheet setup](../fig/spreadsheet-setup-updated.png)

Put these principles in to practice today during your Exercises.




### Structuring data in spreadsheets


The cardinal rule of using spreadsheet programs for data is to **keep it "tidy"**:

1. Put all your variables in columns - the thing you're measuring, like 'weight' or 'temperature'.
2. Put each observation in its own row.
3. Don't combine multiple pieces of information in one cell. Sometimes it just seems like one thing, but think if that's the only way you'll want to be able to use or sort that data.
4. Leave the raw data raw - don't change it!
5. Export the cleaned data to a text-based format like CSV (comma-separated values) format. This ensures that anyone can use the data, and is required by most data repositories.

For instance, we have data from a survey of small mammals in a desert ecosystem. Different people have gone to the field and entered data into a spreadsheet. They keep track of things like species, plot, weight, sex and date collected.

If they were to keep track of the data like this:

![multiple-info example](../fig/multiple-info.png)

the problem is that species and sex are in the same field. So, if they wanted to look at all of one species or look at different weight distributions by sex, it would be hard to do this using this data setup. If instead we put sex and species in different columns, you can see that it would be much easier. 

### Columns for variables and rows for observations

The rule of thumb, when setting up a datasheet, is columns = variables, rows = observations, cells = data (values).

So, instead we should have:

![single-info example](../fig/single-info.png)

> ## Discussion
> The dataset that will be used during the next exercise is the  [Portal Project Teaching Dataset](http://www.datacarpentry.org/ecology-workshop/data/). 
> 
>These data are observations of a small mammal community in southern Arizona. This is part of a project studying the effects of rodents and ants on the plant community that has been running for almost 40 years. The rodents are sampled on a series of 24 plots, with different experimental manipulations controlling which rodents are allowed to access which plots.
> 
> This is a real dataset that has been used in over 100 publications. We’ve simplified it just a little bit for the workshop, but you can download the full dataset and work with it using exactly the same tools we’ll learn about today.  
> {: .discussion}


> ## Exercise
> 
> We're going to take a messy version of the survey data and describe how we would clean it up.
>
> 1. Download the data by clicking [here](https://ndownloader.figshare.com/files/2252083) to get it from FigShare.
> 2. Open up the data in a spreadsheet program. 
> 3. You can see that there are two tabs. Two field assistants conducted the surveys, one
in 2013 and one in 2014, and they both kept track of the data in their own way. Now
you're the person in charge of this project and you want to be able to start analyzing the data.   
4. Identify what is wrong with this spreadsheet. Also discuss the steps you would need to take to clean up the 2013 and 2014 tabs, and to put them all together in one spreadsheet. 
> 
>**Important** Do not forget our first piece of advice: to create a new file (or tab) for the cleaned data, never modify your original (raw) data.
> 
> After you go through this exercise, we'll discuss as a group what was wrong with this data and how you would fix it. 
> 
> > ## Solution
> > - Take about 10 minutes to work on this exercise.
> >   {: .solution}
> >   {: .challenge}

