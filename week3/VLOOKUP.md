# VLOOKUP

##  Lookup formulas

In place of SQL joins, in Excel we have **lookups** — where we use one table to “look up” another value, usually to add a column to a table.

**VLOOKUP** and **HLOOKUP** are the usual examples.
VLOOKUP is more common (vertical look up)

FRENCH: **RECHERCHEV**!!

### Tutorials

* http://www.gcflearnfree.org/excel-tips/how-to-use-excels-vlookup-function/1/
* https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1
* https://www.ablebits.com/office-addins-blog/2014/07/17/excel-vlookup-tutorial-beginner/
* You can search for more - very common question.

#### Examples

In your files, *VLOOKUP_Examples.xlsx*

First is a one sheet example, then there are 2 sheets plus some IF statements.

<img src="assets/VLOOKUP_HW-7a7c5.png">

<img src="assets/VLOOKUP_HW-129a9.png">

<img src="assets/VLOOKUP_HW-9f64e.png">

### Handling errors

If there’s no match in the lookup table, you get an error #NA in Excel.  

<img src="assets/VLOOKUP_HW-ffc47.png">

You can put an **IFERROR** test here and return “NONE” if you have an error!

### Reminder about Formula References!!

 *A2 vs $A2 vs $A$2*

Be careful to use absolute references ($A$2) in your VLOOKUP second argument, because you don’t want the lookup range to change when you copy and paste the formula.
