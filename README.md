# Shiny App for Interactive Educational Tools Using R

## Live Demo

You can explore the interactive app here:  
**[https://quantpsych.shinyapps.io/coding/](https://quantpsych.shinyapps.io/coding/)**

--

## Project Purpose

This project demonstrates how **Shiny**, combined with the **learnr** package, can be used to create interactive educational tools in R. While this app uses **exploratory data analysis (EDA)** as an example topic, the primary focus is to showcase how Shiny can support self-guided learning through embedded code execution, interactive exercises, and real-time feedback.

The framework is adaptable and can be used to build training modules across various domains, including statistics, data science, and public health.

--

## What This App Demonstrates

- Live R code execution within an interactive environment  
- Hands-on coding exercises with auto-evaluation  
- Built-in multiple-choice and open-ended questions  
- Integration of external datasets to support real-world examples  
- A modular structure that can be repurposed for diverse educational use cases

--

## Example Topic: Exploratory Data Analysis (EDA)

This particular version of the app introduces basic descriptive statistics—mean, median, minimum, and maximum—through simple vectors and a COVID-19 mortality dataset grouped by ethnic groups. Learners progress from basic function usage to a data-driven analysis task that summarizes group-level mortality rates.

Although EDA is used as the instructional focus here, the same interactive format can be applied to many other subjects.

--

## R Libraries Used
  
- learnr  
- dplyr  
- readxl

--

## Educational Value

This project illustrates how Shiny can be used to:

- Develop interactive tutorials or training modules  
- Support applied learning through active coding  
- Deliver self-paced, reproducible learning environments  
- Enhance understanding of data concepts through structured tasks and real examples

--

## How to Run

1. Install the required R packages:

    ```r
    install.packages(c("shiny", "learnr", "dplyr", "readxl"))
    ```

2. Open the `.Rmd` file in RStudio and run the tutorial:

    ```r
    rmarkdown::run("teachr.Rmd")
    ```

    Make sure the dataset `COVID19_data.xlsx` is located in a `data/` folder within your working directory.

--

## File Structure

```text
project-directory/
├── teachr.Rmd                   # Main tutorial file
└── data/
    └── COVID19_data.xlsx        # Dataset used for the challenge section
