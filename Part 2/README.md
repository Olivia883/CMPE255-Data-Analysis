# Part 2 – Agentic Exploratory Data Analysis (EDA)

## Project Overview

This project demonstrates how an AI agent can perform exploratory data analysis (EDA) using natural language questions.

The AI agent uses Google Gemini to understand user questions, select the appropriate tools, analyze the Iris dataset, generate visualizations, and explain the results.

Instead of manually writing code for every analysis, users can ask the AI agent questions in plain English.

## Dataset

**Iris Dataset**

- Total Records: 150
- Total Features: 5 columns
- Numerical Features: 4
- Categorical Features: 1
- Missing Values: 0
- Dataset Source: Scikit-learn

### Dataset Features

| Feature | Description |
|---|---|
| Sepal Length | Length of the flower's sepal |
| Sepal Width | Width of the flower's sepal |
| Petal Length | Length of the flower's petal |
| Petal Width | Width of the flower's petal |
| Species | Type of Iris flower |

### Flower Species

- Setosa
- Versicolor
- Virginica

The dataset is loaded directly from Scikit-learn, so a separate CSV file is not required.

## Project Objectives

- Create an AI-powered data analysis agent.
- Analyze a dataset using natural language questions.
- Allow the AI agent to automatically select analysis tools.
- Identify missing values and important data patterns.
- Generate charts and visualizations.
- Provide clear explanations of the results.

## AI Agent Tools

| Tool | Purpose |
|---|---|
| dataset_summary | Provides dataset information and summary statistics |
| missing_values | Identifies missing values |
| correlations | Finds relationships between numerical features |
| create_chart | Generates charts and visualizations |

## AI Agent Workflow

1. Load the Iris dataset.
2. Connect to the Google Gemini API.
3. Define and register the EDA tools.
4. Ask the AI agent a question.
5. Allow the agent to select the appropriate tools.
6. Execute the selected tools.
7. Return the results to the AI agent.
8. Generate findings, charts, and explanations.

## Exploratory Data Analysis

What analyses were performed:

- Dataset exploration
- Summary statistics
- Missing value analysis
- Feature relationship analysis
- Scatter plot visualization
- Species distribution analysis
- Correlation heatmap
- Comprehensive AI-generated analysis

## Key Findings

- The Iris dataset contains 150 records and 5 columns.
- There are no missing values.
- The dataset contains three flower species.
- Each species contains 50 records.
- Petal length and petal width have a strong positive relationship.
- Petal measurements help distinguish between flower species.
- The AI agent successfully selected and executed analysis tools based on user questions.

## Technologies Used

- Python
- Google Colab
- Google Gemini API
- Gemini 3.5 Flash-Lite
- OpenAI Python SDK (Gemini-compatible API interface)
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- JSON

## Project Files

- [Agentic_EDA_Analysis.ipynb](Agentic_EDA_Analysis.ipynb) – Complete Google Colab notebook containing the AI agent, EDA tools, analysis, visualizations, and results.
- README.md – Project Documentation

Google AI Studio: https://aistudio.google.com/apikey

This project was completed without purchasing API credits.

API key is not included in the notebook or GitHub repository.

## Video Demonstration

The video includes a code walkthrough and user journey demonstrating how the AI agent works, selects tools, analyzes the dataset, and generates results.

- **Video Link:** [YouTube Video Link](INSERT_YOUTUBE_LINK_HERE)

## Conclusion

I created an AI agent using Google Gemini to explore and analyze the Iris dataset.

The AI agent successfully analyzed the dataset, checked for missing values, identified relationships between features, generated visualizations, and explained important findings.

Instead of manually writing code for every analysis, I was able to ask the AI agent questions in plain English. The agent selected the appropriate tools, performed the analysis, and explained the results.
