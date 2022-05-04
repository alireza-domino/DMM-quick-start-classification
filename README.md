#  DMM-quick-start-classification
Repo with template files for setting up DMM demos in Domino 4.6

source: https://dominodatalab.atlassian.net/wiki/spaces/salesengineering/pages/2088075277/Domino+Model+Monitor+DMM+Demo+Set+Up

```
{
    "variables": [
        {
            "name": "custid",
            "valueType": "string",
            "variableType": "row_identifier"
        },
        {
            "name": "dropperc",
            "valueType": "numerical",
            "variableType": "feature",
            "featureImportance": 0.7
        },
        {
            "name": "mins",
            "valueType": "numerical",
            "variableType": "feature",
            "featureImportance": 0.9
        },
        {
            "name": "consecmonths",
            "valueType": "numerical",
            "variableType": "feature",
            "featureImportance": 0.1
        },
        {
            "name": "income",
            "valueType": "numerical",
            "variableType": "feature",
            "featureImportance": 0.3
        },
        {
            "name": "age",
            "valueType": "numerical",
            "variableType": "feature",
            "featureImportance": 0.5
        },
        {
            "name": "churn_Y",
            "valueType": "categorical",
            "variableType": "prediction"
        },
        {
            "name": "predictionProbability",
            "valueType": "numerical",
            "variableType": "prediction_probability",
            "forPredictionOutput": "churn_Y"
        }
    ],
    "datasetDetails": {
        "name": "ChurnTrainingDataPP.csv",
        "datasetType": "file",
        "datasetConfig": {
            "path": "ChurnTrainingDataPP.csv",
            "fileFormat": "csv"
        },
        "datasourceName": "churn-dmm-46",
        "datasourceType": "s3"
    },
    "modelMetadata": {
        "name": "customer-churn",
        "modelType": "classification",
        "version": "1.0",
        "description": "Classification model to predict customer churn",
        "author": "Elliott Botwick"
    }
}

```
