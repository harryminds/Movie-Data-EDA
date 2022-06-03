# Movie Data Analysis

## Project for Phase 1 / Data Science at the Flatiron School

### Notebook by Mike Roth

![](/Users/michaelroth/Documents/Flatiron/Projects/dsc-phase-1-project-v2-4/img/movieproduction.png)


# Project Overview

This project analyzes data from [imdb.com](https://imdb.com/) to make recommendations for what movies to produce for a new movie studio. Analysis of the dataset shows that certain movies and genres are more profitable than others and a new studio can use this analysis to plan and produce movies in order to make a profit.

![](/Users/michaelroth/Documents/Flatiron/Projects/dsc-phase-1-project-v2-4/img/MicrosoftLogo.png)

## Business Problem

Microsoft sees all the big companies creating original video content and they want to get in on the fun. They have decided to create a new movie studio, but they don’t know anything about creating movies. We are charged with exploring what types of films are currently doing the best at the box office. We must then translate those findings into actionable insights that the head of Microsoft's new movie studio can use to help decide what type of films to create.

![img](http://localhost:8888/notebooks/img/MicrosoftLogo.png)

## Data

[Imdb.com](https://imdb.com/) has the largest resource of movie data publicly available on the internet. IMDB provides some easily accessible and formatted datasets that contain basic information for analyzing movies. While this dataset is robust, it does not contain the budget and box office information that we need to determine profitability. We decided to create our own dataset of movie information by scraping the database with python. We decided not to choose the whole dataset of movie data available from IMDB, but instead a subset of the data relevant to the business problem. We selected films that were made between 2010 and 2021, that were produced in the US, and were longer than one hour. Further, we will clean the data to include only titles that contain budget and box office information, as not every title on IMDB contains these features.

## Methods

Using descriptive analysis, this project uses the budget and box office data scraped from IMDB.com to create new features. The most used features that were created are ROI (Return of Investment) and Profit. They were calculated as follows.

ROI = worldwide_box_office / budget  * 100 percent

Profit = worldwide_box_office - budget

We compared these features to datasets of genres, studios, and budgets.

## Results

![genre_pairs_roi_and_profit](/Users/michaelroth/Documents/Flatiron/Projects/dsc-phase-1-project-v2-4/figures/genre_pairs_roi_and_profit.png)
