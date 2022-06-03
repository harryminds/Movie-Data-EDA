# Movie Data Analysis

#### Author: Mike Roth

![](img/movieproduction.png)

# Project Overview

This project analyzes data from [imdb.com](https://imdb.com/) to make recommendations for what movies to produce for a new movie studio. Analysis of the dataset shows that certain movies and genres are more profitable than others and a new studio can use this analysis to plan and produce movies in order to make a profit.

![](img/MicrosoftLogo.png)

## Business Problem

Microsoft sees all the big companies creating original video content and they want to get in on the fun. They have decided to create a new movie studio, but they don’t know anything about creating movies. We are charged with exploring what types of films are currently doing the best at the box office. We must then translate those findings into actionable insights that the head of Microsoft's new movie studio can use to help decide what type of films to create.

## Data

[Imdb.com](https://imdb.com/) has the largest resource of movie data publicly available on the internet. IMDB provides some easily accessible and formatted datasets that contain basic information for analyzing movies. While this dataset is robust, it does not contain the budget and box office information that we need to determine profitability. We decided to create our own dataset of movie information by scraping the database with python. We decided not to choose the whole dataset of movie data available from IMDB, but instead a subset of the data relevant to the business problem. We selected films that were made between 2010 and 2021, that were produced in the US, and were longer than one hour. Further, we will clean the data to include only titles that contain budget and box office information, as not every title on IMDB contains these features.

## Methods

Using descriptive analysis, this project uses the budget and box office data scraped from IMDB.com to create new features. The most used features that were created are ROI (Return of Investment) and Profit. They were calculated as follows.

ROI = worldwide_box_office / budget  * 100 percent

Profit = worldwide_box_office - budget

We compared these features to datasets of genres, studios, and budgets.

## Results

We can see that the top genres for **Mean ROI** are: **Mystery, Horror, and Thriller**. This is not very surprising as horror and mystery movies often have low budgets with much larger profits.

And when it comes to **Gross Profit**, we see the top genres are **Adventure, Animation, and Sci-Fi**.

![mean_roi_and_profit_by_genre](/img/mean_roi_and_profit_by_genre.png)

The top genres for **Mean ROI** are: **Mystery, Horror, and Thriller**. This is not very surprising as horror and mystery movies often have low budgets with much larger profits.

And when it comes to **Gross Profit**, we see the top genres are **Adventure, Animation, and Sci-Fi**.



![budget_vs_roi_by_Studio](/img/budget_vs_roi_by_Studio.png)![budget_vs_profit_by_Studio](/img/budget_vs_profit_by_Studio.png)

We see in the top graph for **ROI vs Budget**, a studio like **New Line Cinema has the highest ROI** and a mean budget on the lower end in this range of studios. New Line Cinema produces hits movies in genres that have high ROI.

In the middle graph for **Mean Profit per Movie vs Budget**, we see that **Marvel Studios leads in both profit and budget**. Marvel focuses on superheros, action, sci-fi, adventure films that produce high profits.



![budget_vs_roi_and_profit](/img/budget_vs_roi_and_profit.png)We can see in the left graph (**Budget vs ROI**) that **a very low budget can sometimes lead to very high ROI**. In general, the less money spent, the higher the ROI.

Although in the right graph (**Budget vs Profit**) , we see that **the more money spent the higher the total profit**. This may seem to contradict the previous graph, but actually if a studio is looking for the greatest profit, we can see **there is a clear relationship between high profits and high budgets.**



# Conclusions

### Our analysis leads to the following main conclusions:

### Genre Profitability

- The most profitable genres are **Horror, Mystery, Thriller, Adventure, Animation, and Sci-Fi.**. Horror and Mystery are the most profitable in terms of ROI percentage, and Adventure and Fantasy create the largest gross profit

### Studio Profitability

- The **most profitable movies** are from studios focusing on producing **less genres**. While most studios were profitable overall, the studios with the highest mean profit per movie, decided to focus on a smaller set of profitable genres, rather than diversify the number of genres produced. There are two directions a studio like Microsoft should choose to take. To focus on producing movies in genres that have high returns or movies that have high profits.

### Budget Profitability

- **Spend less, and make more, or spend more and make A LOT more.** While genres like Horror and Mystery may cost less and have a higher return, the studios that spent more money per movie, made the most gross profit. Also, movie genres that may require a higher budget to produce (Adventure, Animation, Sci-Fi) also created the most gross profit.

**If Microsoft were to create a movie studio, they should consider the investment they choose to make in production. With a high budget, they can choose to produce films that have much higher profits. If they choose to spend less, they should focus on the movies with the highst returns.**
