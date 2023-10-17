# pandas-challenge
Module 4 Pandas HW


For assistance with the unique number count I used the website "https://www.tutorialspoint.com/how-to-count-unique-values-in-a-pandas-groupby-object#:~:text=To%20count%20unique%20values%20in%20a%20pandas%20Groupby%20object%2C%20we,or%20to%20the%20entire%20object."


Because I kept getting a type error: TypeError: '<' not supported between instances of 'int' and 'str' I used chat GPT to break down why that error was occuring, although it couldn't specifically figure out why my code was producing that error it did suggest to remove the prior formatting

I used the following code to complete this in the Scores by School Spending section.

per_school_summary["Average Math Score"] = per_school_summary["Average Math Score"].str.replace(',', '').astype(float)

per_school_summary["Average Reading Score"] = per_school_summary["Average Reading Score"].str.replace(',', '').astype(float)

per_school_summary["% Passing Math"] = per_school_summary["% Passing Math"].str.replace('%', '').astype(float)

per_school_summary["% Passing Reading"] = per_school_summary["% Passing Reading"].str.replace('%', '').astype(float)

per_school_summary["% Overall Passing"] = per_school_summary["% Overall Passing"].str.replace('%', '').astype(float)
