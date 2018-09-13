# Week2 Analyst Toolbelt : Pivot Tables

## Goals
  * Making a pivot table with rows
  * sorting
  * top 10
  * Columns and Rows
  * Nesting
  * calculations other than count
  * time groupings

### Pivot Tables like Tall, Raw Data   

 Pivot Input data is as on the right...
“Wide” data is on the left.  Sometimes "wide" table data is the result of a Pivot table operation.

<img src="week2_pic/2.png" width="600" height="410">  
                                                    “Tall” or “Long” data   

To see more, see the section for [Tidy Data](TidyData.md).

## Finding the Pivot Table Command

Video Demos:

* [Mac Excel English Pivot, Count Values](https://youtu.be/fxP81RaPBFQ)
* [Windows Excel French Pivot](https://youtu.be/fsre1PJYDM4)

1. Select your data. Find and Click the PivotTable (“Table Croisée”) on the ribbon toolbar or menu.  
2. *On Windows,* check the “Insert” Ribbon Tab.
	*On Mac,* the “Data” Ribbon Tab.  
3. Also look at the menus (check Insert and Data menus).  

You should get the dialog:  
<img src="week2_pic/3.png" width="600" height="461">   

 *Note: Every column needs a label for this to work!*

4. Click OK (after making sure it shows your selection.)  

On Mac, it makes a “default” pivot table.   On Windows, you need to select the option on the bottom of the suggestions dialog for "Table Vide."

It should show the “Builder” open. The command to open it is on top on the ribbon (in case you lose it/close it).

<img src="week2_pic/4.png" width="600" height="439">   

If you have items in your builder, drag them “out” of the dialog to empty it (see Mac video). Goal is to start from empty:

<img src="week2_pic/5.png" width="600" height="445">   

The parts of the builder dialog:

<img src="week2_pic/6.png" width="400" height="415">   

5. Do this: Drag “Primary Type” into both Rows and Values:

<img src="week2_pic/7.png" width="600" height="559">   

By default, it produces a Count of each Primary Value.  
And the row labels are alphabetic.  

**A quick pivot can reveal a need to clean... Keep an eye on the results you see!**

This is another data set: *Hunting Injury Data – VictimACTIVITY (Victim Activity) by Count of WOUNDs*  

<img src="week2_pic/8.png" width="600" height="676">

(How would you clean that data?  You could edit the text so it's consistent in a copy of the raw data! Then the counts will be more accurate.)

### You can change the sort order.

On Windows, right click inside a cell in Values. Choose sort (Trier).
On Mac, click the Sort button in the Data tab while your mouse is in the column.

(The videos above show this too.)

###### Show the top primary crimes in order, descending.

 Let’s do that with chi2.csv, our Chicago dataset.

*Mac UI, result:*   
<img src="week2_pic/10.png" width="250" height="551">   

### Filter Results to Top 10... on Windows:
Right click on first column item, and you’ll see Filter > Top 10...
(or filter by other options!)  
Get the top 10 crime types.

Video Demo: [Windows Excel Top 10 Pivot Results By Value](https://youtu.be/CSHWmbSH8rg)

<img src="week2_pic/11.png" width="400" height="556">   

### Top 10 on Mac:  
Pick Menu on Row Labels, Choose the menu beside “By Value”...

<img src="week2_pic/12.png">   

Helpful link: https://www.techonthenet.com/excel/pivottbls/top10_2011.php

###### Exercise 1- Do the same operations with Streets now (in chi2.csv, the data we cleaned last week). (Streets, not block!)  

*What is the street with the most crimes? What are the top 10?*

### Using Columns Too

*What if we wanted to find out which streets had the most arrests?*

Now Add “Arrest” to columns in your pivot table builder UI:

<img src="week2_pic/13.png">

Now what about what kind of crimes had the most arrests?

Make Arrests your columns, and the primary type the rows. Sort by Arrests, True.

*Result:*
<img src="week2_pic/14.png" width="300" height="337">   


### Filters on Pivot Tables

If you want to dig into a particular type of data, you can make a filter.   
Drag “Primary Type” into the filters area — it will appear above the pivot results —


<img src="week2_pic/15.png" width="282" height="450">   

and set it to Narcotics.   
<img src="week2_pic/16.png" width="200" height="93">

[Video of simple filtering on pivot table](https://youtu.be/l1nc62R-68k)


### Nested Rows

If you want to learn more about each ROW (or column) of data, you can add another variable to the same group.       
Try adding Location Description to the Rows under “Street”:  
<img src="week2_pic/17.png" width="400" height="618">   

**Feel free to change the filter!**

<img src="week2_pic/18.png" width="400" height="307">   

 Now try...

<img src="week2_pic/19.png" width="400" height="436">   

 What’s interesting there?

[Video demo of nesting rows and sorting](https://youtu.be/8a3Ny3Pi93w)


## Pivots with Quantitative Data & Groups

:zap: **This file is due for homework.** :zap:

*What if we want a calculation or combination of quantitative numbers, instead of Count of qualitative data?*

For instance, if you have numeric data like Sales figures over time, or rainfall per month.

**Import Paris_Rainfall_Unpivoted.csv** in a tab.

1. Create a pivot table on a new tab (empty all the Builder fields!).
2. Set it up this way... Year and Value:
  * click on the option for Values and edit it to be SUM instead.
  * With numeric data, you can summarize by other calculations than count.

<img src="week2_pic/20.png">   

Now sort by Values, descending.

Call this tab “annual_sum.”
<img src="week2_pic/21.png" width="200" height="403">     

Video demo: [changing to sum/somme](https://youtu.be/nxFxNAQDnAw)

Now do average per year, in a new tab.

If you sort descending by Total, what’s the top year?  

Call this tab “annual_avg."
<img src="week2_pic/22.png" width="200" height="280">   

How would we get to the original data we “unpivoted”?

Call this tab “by_month.”

<img src="week2_pic/23.png">

## Grouping & Dates

We can “group” numeric data to make a manual histogram or to handle date ranges.  

Start from a sum of rainfall by year pivot, with the years in order, ascending (i.e., don't sort it).

If you have years in your row labels, with your mouse on one year cell,
right click to open the group option. In French it is "Grouper".

#### Group Years by Centuries (100 years)

<img src="week2_pic/25.png" width="800" height="417">

Choose "Sum" of values, not count.  You should have this:

<img src="assets/PivotTables-70caf.png">

Call this tab "century_totals".

**Alert: If you group one pivot table, it will group the others. That's ok right now.**

### Filter by Months - Winter Months Avg.

Repeat this on a new tab. Now filter by months...

Set the filter to Jan, Feb, and Dec.   

<img src="assets/PivotTables-e25f7.png">

Set your Aggregation to Mean (Moyenne).

Call this tab “mean_winter".

***Your file should have these tabs:***
  * annual_sum
  * annual_avg
  * by_month
  * century_totals
  * mean_winter

Plus a histogram - see [Histogram.md](Histograms.md).
You'll add a histogram tab next.
You will turn this in as an excel file for HW. (Leaving things grouped is fine.)
