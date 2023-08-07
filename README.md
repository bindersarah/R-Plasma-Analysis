# R Plasma Analysis

## Intro
The code written here represents my analysis of a dataset containing information garnered from plasma assays.
The fields include research subject ID, dates of amyloid & tau PET scans, dates of blood draw, and the subsequent values per assays which were derived from the blood sample.

## Step 1: Excel
I received the data as a "messy" Excel worksheet. Every subject had multiple blood draws and values per assay were shown in separate sheets within the Excel worksheet.
My task on this project was to prepare the data for analysis. First, I did some basic cleaning and preparing of the data in Excel. 
I had to select the draw date that was closest to the PET scan dates, which required selection of data based on matching ID and date. For this I used VLOOKUP in Excel.
In Excel, I also performed essential data cleaning such as using DATEVALUE to make the program recognize the date as a workable data type.

## Step 2: R
Next, I moved in to R once I had my selected draw dates. In R, I performed more cleaning and aggregating of the data- mutating data types, re-naming column headers, removing extraneous info, etc. 
I needed to standardize the data per assay, so that I could bind & join the data into one dataframe. 

## Functions used
Text data manipulation, filter, subset, group by > summarize(n()), mutate merge, join, rbind, ifelse, difftime to calculate intervals
