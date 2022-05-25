# Step 4 - Building Machine Learning in Power BI

## Prerequisites

1. [Step 3 - Working with Cognitive Services](https://github.com/Alexandrovdi/PowerBI_AI/blob/main/Challenge%20steps/Step%203%20-%20CognitiveServices.md) should be done successfully.

## Introduction
The purpose of this challenge is to train an operationalize an ML model leveraging AutoML in Power BI premium capacity.

## Basic Steps to Complete
1. Edit the existing data flow and import additional entities for BikeBuyerTraining and ProspectiveBuyer from the Azure SQL Database source
2. Save and refresh the dataflow
3. Add a new machine learning model to the dataflow
4. Select BikeBuyerTraining as the data source and BikeBuyer as the target column to predict
5. Select 1 as the target value, and provide labels for the positive and negative test cases
6. Select all the provided columns to train (Note: we've pruned the dataset to avoid errors, but this is where you'd have an opportunity to exclude fields from the training)
7. Move the slider to reduce the training time to **5 minutes** (Note: the default is 120)
8. Run the training
9. When training completes you'll be able to generate a report to view the details of your model and see which fields had the most impact on the results
10. Now that you have a trained model, select apply model to score your prospective buyers, map the fields and execute the scoring
11. In Power BI desktop load the scored data and build reports

## Hints

1.  This step requires A2 capacity to complete, the AI features won't show up unless an A2 capacity is assigned to the workspace.
2.  The datasets for ProspectiveBuyer and BikeBuyer don't match exactly. ProspectiveBuyer has a birthday column not an age column.   You need to manipulate the BirthDate column to calculate the age before you can apply the model to ProspectiveBuyer.
