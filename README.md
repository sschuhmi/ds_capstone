## Capstone Project "Predicting Results of modern Football matches using StatsBomb analysis data and advanced multi-output Machine Learning Regressors"

This project was created as capstone project within Udacity´s Data Scientist Nanodegree Program [nd025](https://www.udacity.com/enrollment/nd025)

### Table of Contents
 
1. [Project Motivation](#motivation)
2. [StatsBomb Open Data](#surveydata)
3. [Provided Files](#files)
4. [Installation & Libraries](#installation)
5. [Results and Blog Post](#results)
6. [Licensing and Acknowledgements](#licensing)

## Project Motivation <a name="motivation"></a>

In this project, we exploit the free StarsBomb open data set and use moderen Machine Learning multi-output Classifiers and Regressors to predict the winner of a match, compared to a simple non-ML Classifier which randomly decides one of the possible three results - first team wins, second team wins, or there is a draw between the teams.

## StatsBomb Open Data <a name="surveydata"></a>

Currently in October 2024, StatsBomb´s open data represents only a small, but yet comprehensive subset of the overall StatsBomb data.

The data is provided as JSON files exported from the StatsBomb Data API, in the following structure:
- 21 competitions with 74 seasons
- Almost 3500 matches, spread among the above mentioned competitions and seasons
- Events and lineups for each of these matches, included additional StatsBomb 360 data for selected matches

A fine-grained documentation of the files, their formats and their contents is also included in StatsBomb´s [GitHub repository](https://github.com/statsbomb/open-data).

## Provided Files <a name="files"></a>

The following files are provided within this project:
<ul>
  <li><b>DS-Capstone_PredictingFootballMatches.ipynb:</b> Jupyter Notebook containing the Python code for this project</li>
  <li><b>data/competitions_matches.zip:</b> ZIP file containing the used competitions and matches of StatsBomb open data</li>
  <li><b>data/events1.zip & data/events2.zip:</b> ZIP files containing the used events within the above matches of StatsBomb open data. There are 2 ZIP files due to the file restriction of 25MB per file in GitHub.</li>
  <li><b>README.md:</b> This file</li>
</ul>

## Installation & Libraries <a name="installation"></a>

To analyze the data, I used Python (version 3.9.19) in combination with Jupyter Notebooks (version 6.4.5). The code is provided within the ipynb-File and should run on any Python 3 version (3.0.* or higher) without any issues. It was tested using the Anaconda distribution of Python.</br>

The relevant StatsBomb open data is provided within 3 ZIP files that need to be imported first. Please make sure to extract them in the 'data' subfolder below the Jupyter Notebook ipynb file. Due to the structure of the ZIP files, two additional subfolders for matches and events will be created.

Here are the additional Python libraries used within this project:
<ol>
  <li>numpy==1.21.4</li>
  <li>pandas==1.3.5</li>
  <li>matplotlib==3.8.4</li>
  <li>seaborn==0.13.2</li>
  <li>scikit-learn==1.0.1</li>
</ol>

## Results and Blog Post <a name="results"></a>

The project focused on predicting results of modern football matches by exploiting statistical analysis data of matches.</br>
The main findings of the code can be found in my blog post available [here](https://sschuhmi.github.io/2024/10/06/PredictingFootballResults.html) at GitHub pages.

## Licensing and Acknowledgements<a name="licensing"></a>

Thanks to StatsBomb for providing their open data set via GitHub. The Licensing for the data and other descriptive information can be found at the [StatsBomb Open Data Github space](https://github.com/statsbomb/open-data).

