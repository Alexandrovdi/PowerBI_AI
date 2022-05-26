# Step 3 - Working with Cognitive Services

## Prerequisites

1. [Step 2 - Working with Data in Power BI](https://github.com/Alexandrovdi/PowerBI_AI/blob/main/Challenge%20steps/Step%202%20-%20Dataflows.md) should be done successfully.


## Introduction

The purpose of this challenge is to show users how to operationalize cognitive services in Power BI Dataflows.


## Basic Steps to Complete
1. Edit the existing dataflow (on msit.powerbi.com) and import a new tables to include the Bike Reviews data
1. Enter the connection information for the csv/text file from a [url](https://raw.githubusercontent.com/Alexandrovdi/PowerBI_AI/main/Data/bike%20reviews.csv)
2. Rename from Query to BikeReviews
3. Add an AI step to the data flow to detect language using the review text
4. Expand the structured results of the cognitive service to retrieve the language and language iso code
5. Add another AI step to score sentiment using the review text and the language iso code as inputs
6. Add another AI step to extract key phrases using the review text and language iso code as inputs
7. Save, close, and refresh the data dataflow
8. In Power BI Desktop import the new bike reviews entity from the data flow source, and examine the results

## Potential pitfalls

1.  Sometimes dataflows will have a sequencing problem that causes the dataflow to change prior to the AI logic being applied. If this occurs, you'll need to cancel your save and start over on applying the AI. Best bet is to save after each AI step to be safe.


[Next step (Building Machine Learning in Power BI) >](https://github.com/Alexandrovdi/PowerBI_AI/blob/main/Challenge%20steps/Step%204%20-%20Building%20Machine%20Learning.md)
