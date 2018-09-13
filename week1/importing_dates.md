


## Importing Text Data Into Excel and Types


### CSV Import

We need some data to start with.  A common "raw data" file format is CSV, or "comma separated values."  (In France it is usually ";" separated.)

*VIDEOS*:

>Mac English Excel Video: [Import CSV](https://youtu.be/7U5WgW_mQ8o)

>Windows French Excel 2016: [Import CSV](https://youtu.be/eB2NR0P55r0)


It is very common for a raw data set to be in a text format, not excel. Usually it will be in “CSV” or “TSV” format — “comma separated values” or “tab separated values.”

The difference is the character that separates the columns of data — for instance, this is CSV data with 2 columns (and no “header” title on the first row):

<img src="week1_pic/csv_data.png" width="111" height="250">   


#### Importing steps (Mac, English)

(See the video links above for other formats.)

1. Click on File menu, then “Import....” and make sure this dialog says CSV:

<img src="week1_pic/import_menu.png" width="500" height="353">   

2. If it is “tab separated”, you could choose text. But you can also use CSV for tab separated data.


<img src="week1_pic/delimiter1.png" width="500" height="355">

2.a. It's important to change the source menu if you are using a data file from a region with a different currency or date format.  For some copies of Excel, this seems to be the key to converting for your own regional display correctly.  For instance, using a file from the US, in a French copy of Excel, I make sure the origin says Etats-Unis (where the yellow is):

<img src="week1_pic/import_origin_menu.PNG">

On Mac, importing a French file into American Excel, I have to choose something for European (no "France" option shows).

<img src="week1_pic/mac_import_file_origin.png">

**NOTE: This does not fix the problem for all versions of Excel and regions.  Dates may still be interpreted incorrectly. To be sure, you can import your dates as a text column, which means it will not be re-interpreted as an incorrect date in your regional settings. You will then have to fix it with formulaes. See below.**

2.b. Here you specify what the character delimiter is between your data columns. You can type in a special one in "other".

<img src="week1_pic/delimiter2.png" width="500" height="355">   


3. The “Types” Dialog:

You can also change your data types after importing, but there is one important issue here: **decimal number format**.  


<img src="week1_pic/dialog_types.png" width="500" height="440">   

Click on “Advanced...”

This issue caused a lot of difficulty to students last semester.  

<img src="week1_pic/comma_issues.png" width="304" height="200">  

 :zap: :zap: **All of my data files use international formatting for decimals: “point” or “dot”, not “comma.”** :zap: :zap:

Make sure you change this to match my settings when you import text data with numbers.

4. The last dialog - if you are in a blank new workbook, use $A$1:

<img src="week1_pic/import_data.png" width="400" height="202">  

#### alternatively... some Excel versions can open CSV files for you:

In a blank workbook, click File menu, choose Open.... and change the dialog to show or enable “All files”:  

<img src="week1_pic/all_files.png" width="500" height="403">  

Navigate to and click on **ChiCrimes_Chicago2008.csv** to open it.   
Hopefully it will understand the csv format and load it correctly for you:

![Chicago_csv](week1_pic/Chicago_csv.png)

###### If it does not... all of it will be in one column, with no headers.

Then your solution is to split the single column using the same dialogs, accessible from the “text to columns” button (under Data / Donnees tab).

On Windows it will be called "convertir", not "text to columns":

French:
<img src="week1_pic/french_excel_text_to_cols.PNG">

English:
<img src="week1_pic/txt_col.png" width="250" height="73">  

Video Demo: [Mac Text to Columns](https://youtu.be/xs4QmuhFgSo)

## Verifying: Date/Time types

When you import a CSV file, make sure you know the origin for date and currency handling.  You should set the origin when you import (although this is still not always sufficient):

Video: [Importing French Data into American Excel](https://youtu.be/HxRai7NZH50)

Video: [Importing French Data into French Excel with US Settings](https://youtu.be/HxRai7NZH50)

The data type is very important in Excel.  To check the type, put your mouse on a column and check the type in the "Number" cell on your home ribbon:

<img src="assets/importing_dates-26b59.png">

The type will generally be "Standard" or "General" for unspecific types.  It can be changed if you want special behavior, such as for dates.

### Dates - Beware:

When we import from CSV (or other text formats), Excel may guess “wrong” for the date/time fields.

> **A common problem**  
> One issue people frequently run into is that Excel occasionally misinterprets text fields as dates.  
> An example is here :  
> <img src="week1_pic/Excel.png" width="300" height="89">   
> Be careful when entering dates, especially if you are importing from other data sources, to make sure that you "Jan-13" is being stored as January 13, 2013 !
>
***- http://www.exceltactics.com/definitive-guide-using-dates-times-excel/ -***

### Field Types - Especially Dates

To change a field type, especially to format dates differently, you can adjust using "Custom" or "Autres Formats..." (bottom of the pulldown menu).

![format_cells](week1_pic/format_cells.png)

### Formating Times as Custom...

![time_format](week1_pic/time_format.png)

Choose the time format you prefer from the Custom dialog.

Try this with me on the Dates tab in the **ChiCrimes** file.
Change the time to show am/pm.   
You must select the entire column, not just a single cell!  
Do that by clicking the C on top.

Then choose “Custom...”

<img src="week1_pic/custom_format.png" width="600" height="371">   

You should have a date option that includes AM/PM in the time.

<img src="week1_pic/am_pm_dates.png" width="500" height="494">   

###### What if we wanted the date and time in different columns?

Hint: Copy the Date column to 2 new columns. Reformat them.  
Rename the original col to “date-time” and the other 2 to “Date” and “Time”. Or use formulae.

<img src="week1_pic/date.png" width="350" height="305">

Notice that when you mouse in a cell, you see the full date information.

### Now save this edited data as CSV. Call it “chi2.csv”.
  * Save As...  
  * Pick format CSV  
  * Give it the name “chi2.csv”

Video: [Save as CSV](https://youtu.be/uJ_cSdF8hkk)

<img src="week1_pic/chi_csv.png" width="300" height="131">

*Note: you are going to upload this file after the exercises, so make sure you do this and work in it now.*

Now open that new file you made. What do you see about the new “Date” and “Time” columns now?

**This is why we kept the original column with both...**  

Excel format saves more info than csv. CSV is a text format that preserves **only the text visible** in the cells.   
That’s why format types matter so much in the display in the cell. Make sure you have your data formatted with the info you need.

## Being Even More Careful With Dates

  * The advice in Browman & Woo is to save your dates in the international standard YYYY-MM-DD.  This is
  * Article: [Dates as Data](http://www.datacarpentry.org/spreadsheet-ecology-lesson/03-dates-as-data/)
  * Store your day, month, year separately (allows some special analysis by each) &/or
  * Be sure text fields are interpreted as date types correctly.

**Your safest behavior is to import a date column as text and then "fix" it with a formulae by parsing the text column using the "DATE" function and string functions like "LEFT" and "RIGHT".**


English:
> =Date(year, month, day)

French:
> =DATE(year; month; day)

From ExcelJet article:

<img src="assets/importing_dates-8a698.png">

Read this: https://exceljet.net/formula/convert-text-to-date
