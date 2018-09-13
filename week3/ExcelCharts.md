## Excel Charts

### Making a Chart With Defaults.
1. Select some data column(s). You can use the data in AnnotationChart.xlsx, on the "Your Work Here" tab.
2. Click the chart tab  
<img src="assets/Readme-91bce.png">
3. Pick a chart type!  
<img src="assets/Readme-b9b1d.png">
*Examples_Charts.xlsx*


## Parts of a Chart  

  * Title and Legend
<img src="assets/Readme-8ff14.png">

  * Data Labels and Axes
<img src="assets/Readme-e1a11.png">

## General Design Tips
* Only color sparingly - use a different one for the
* Remove or reduce saturation of grids/axes and ticks (especially remove ticks)
* Add annotation or label on “interesting” points
* Have useful titles and axis labels.
* You can remove your legend if there is only one series shown.

Remember the [Data to Ink Ratio gif](https://www.darkhorseanalytics.com/blog/data-looks-better-naked).

We made a chart with defaults... (the defaults shown are an old version of Excel, by the way, the new one seems better).

Now we need to customize it.

Click on the chart, which will open the tabs for the chart on your ribbon bar.
Go to Chart Layout Tab >> Format.   
Click in the Title Field on the Chart to Change it. In an older Excel, you may see this:

<img src="assets/Readme-544c5.png">

In newer Excel on Mac, it looks like:

<img src="assets/ExcelCharts-178f4.png">

 Many more things you can customize...  

Click on parts of the graph, and then RIGHT CLICK, you will get menus to format:  
  * Axes
  * Gridlines
  * Legend
  * Text
  * data series
  * labels...

<img src="assets/Readme-fb024.png">  

Highlights and Annotations  
<img src="assets/Readme-55639.png">
 Let’s go thru the first tab in *Examples_Charts File*

 Video here: [Create and Customize Chart](https://youtu.be/ucowDtR1IM4)

### Custom Colors and Formatting   
  *(in AnnotationChart.xlsx)*  

 * Click once on a data element to select the whole series

<img src="assets/Readme-7a560.png" height="300">  
 * Click a second time to select on data element, the single bar.

<img src="assets/Readme-75f4e.png" height="300">  

 * RIGHT-CLICK for this dialog and select Format Data Point:  
  Btw, avoid 3-D, glow, etc.  A dialog will open on the right panel (in a recent Excel). You want to choose "fill" to change the color of the bar -- the paint bucket:

  <img src="assets/ExcelCharts-65bba.png" height="300">


Add the Labels / Annotations

 * One click for all data bars, 2 clicks for a single bar,
 * then right-click, pick Add Data Label(s):

<img src="assets/Readme-1fb27.png" height="300">  

 Default label is the value in your data column-  we will see how to format the red bar label differently below.

<img src="assets/ExcelCharts-43932.png">

### Format Data Labels

To add data labels to your chart, you can use the option in the toolbar on the far left (of the Chart tab). (In older excel, these options are lined up under the chart formatting tab label).

<img src="assets/ExcelCharts-c3996.png" height="300">

To adjust the font size, style, etc. you can right-click on the label(s) you want to adjust (color, $ sign, etc.). Pick "Format Data Labels." This gives you formatting controls.

<img src="assets/Readme-d2f21.png" height="300">

If you want to only format one label -- like make it red, or bold, or bigger, you can select once or twice to get the right one selected before you choose the menu item.

Then to customize the text CONTENT in one label, to make it more explicit, you can select the label itself and modify the text carefully.

<img src="assets/ExcelCharts-598c3.png">


### Formatting the Axis: Number Type, Display, Ticks...

 * Right-click on chart element to get these menus.

<img src="assets/Readme-d42de.png" height="300">

<img src="assets/Readme-7ea50.png">

** Formatting for number style on tick marks, needed for the homework:**

<img src="assets/ExcelCharts-cc3f8.png" height="300">

Video demo: [Custom tick marks](https://youtu.be/NgJrkgNSN1A)


### Adding Text Labels Elsewhere

#### Tip: Inserting Text Boxes in Charts (on a Mac)  

With the chart **NOT** selected, use the Insert menu. Move the text box to where you want it on the chart.

<img src="assets/Readme-313df.png" height="300">


#### Understanding Data Series in a Chart  


When you click on a chart, you’ll see the data fields in the spreadsheet outlined. Those outlines are draggable/resizable.

<img src="assets/Readme-72ae9.png">

If you drag the bottom right to include a second column of data, it will automatically add it to your chart:

<img src="assets/ExcelCharts-9acfb.png">

You may need to reformat it at that point!

#### Data Series Dialog

*Important "Under-the-Hood" (How it Works)...*

 Even more importantly, the data series dialog:  

Choose "Select Data" in the toolbar:

<img src="assets/ExcelCharts-90412.png">

OR click on the chart, right click, and pick Select Data. This dialog is how you add series, change labels, etc.

<img src="assets/Readme-5398c.png">

What if you wanted to have non-adjacent data in your chart? You would use this dialog to pick it.  It's more complex, you can't just select the extra column from the drag-and-drop outline.

<img src="assets/ExcelCharts-3bb44.png">

Video demo: [Custom Columns of Data in Select Data](https://youtu.be/_hWw7W4fPVo)


## Conditional Formatting & Sparklines

### 1. Conditional Formatting and "heat maps":

You don't have this particular file, but we can do it on another one.

 <img src="assets/Readme-51591.png">

Heatmaps in the media:  
http://graphics.wsj.com/infectious-diseases-and-vaccines/

<img src="assets/Readme-6e437.png">  

### 2. Highlighting Cells

 Highlighting duplicates is very useful for comparing  overlaps or finding uniques.   
 Shoot injuries, for instance.

 <img src="assets/Readme-1a3ef.png">

 You can go to town on formatting...

<img src="assets/Readme-7ebc5.png">

### 3. Sparklines  

 *In data set ParisRainfall...*

 Insert tab, sparklines menu:

<img src="assets/ExcelCharts-b3923.png">

In a cell, a tiny chart
(concept from [Edward Tufte](http://www.edwardtufe.com/bboard/q-and-a-fetch-msg?msg_id=0001OR).)

  - Insert or Chart tab:   
<img src="assets/Readme-e626a.png">

  - Add to the right of the months.  

<img src="assets/Readme-74b2c.png">

### 4. Advanced Maneuver: “Interactive” Charts

The Developer Tab is added via the Preferences, Ribbon.  We won't do this in class, though.

<img src="assets/Readme-1d022.png">

 These are a powerful way to deliver a report or explore yourself.... or build a simple prototype for an interactive project!

 <img src="assets/Readme-f871b.png">

We're not going over these in class, but you can build little applications right in Excel if you want.

## Design Example Using Pivots and Charts

Using the rainfall file... (Paris Rainfall Unpivoted.xlsx).  This is a "big data" charting problem.  Too many data points for any pattern to emerge!

- Adding Trendlines
*Paris_Rainfall_graphs.xlsm*

<img src="assets/Readme-18152.png">

Date Grouping power: Average, by month, by century.

*Paris Rainfall - Year (Centuries)*

<img src="assets/Readme-3fe04.png">



## Examples Excel Makeovers To Inspire You

###### 1. Cole Nussbaumer’s Students

Student Makeover examples:  
  - by Brittney Younger

<img src="assets/Readme-139fb.png">  
  - by Marianne Siblini

<img src="assets/Readme-3644b.png">

What's wrong with the originals?

*http://www.storytellingwithdata.com/2013/11/intro-to-information-visualization.html*

###### 2. Jon Schwabish Excel Remakes

 - Redoing a Bureau of Labor Statistics employment graph  
http://thewhyaxis.info/defaults/

<img src="assets/Readme-edf45.png" height="300">

 - Redoing a Gender Gap graph from NYT Economix blog: http://thewhyaxis.info/gap-remake/

<img src="assets/Readme-a19ba.png" height="300">

## Fun Chart Types

- Stephanie Evergreen:
http://stephanieevergreen.com/how-to-make-dumbbell-dot-plots-in-excel/

<img src="assets/Readme-5a708.png" height="300">

- Slope Graphs: http://peltiertech.com/slope-graphs-in-excel/

<img src="assets/Readme-dd7d6.png" height="400">

- Small Multiples / Cycle Plots:

<img src="assets/Readme-9b49c.png" height="300">

<img src="assets/Readme-0e32b.png">

- Dot Plots with a helper tool from Jon Peltier.

<img src="assets/Readme-5bb70.png">  
Using [Peltier Chart Utility plugin](http://peltiertech.com/Utility20/), with customization.



## A Few Excel Charting Resources

* Great book by Jorge Camoes with Excel examples: [Data at Work](https://www.amazon.com/Data-Work-practices-effective-information/dp/0134268636/ref=as_li_ss_il?ie=UTF8&qid=1479988665&sr=8-1&keywords=data+at+work&linkCode=li3&tag=camoesjott-20&linkId=700a9059bdb09dfd5509965c061b241e)

* [Excel Charting Do’s And Don’ts](http://peltiertech.com/WordPress/excel-charting-dos-and-donts/)

* Jon Schwabish tutorial: [Making Excel Graphs Better](http://www.slideshare.net/jschwabish/making-excel-graphs-better)

* Book: Michael Alexander’s Excel 2007 Dashboards

* [Peltier Chart utility](http://peltiertech.com/Utility20/)
