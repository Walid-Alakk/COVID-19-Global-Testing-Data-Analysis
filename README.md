# COVID-19-Global-Testing-Data-Analysis

### Project Overview

The COVID-19 pandemic has had a profound impact on the world, with testing being a crucial component in understanding and controlling the spread of the virus. This project focuses on analyzing global COVID-19 testing data by country to provide data-driven insights for a news channel's documentary feature story. By extracting, processing, and analyzing this data, we aim to highlight testing patterns, identify trends, and uncover significant findings that can inform public health decisions and raise awareness.

### Description

#### Why This Project is Important

1. **Informed Decision-Making**: Accurate and comprehensive data analysis allows governments, health organizations, and the public to make informed decisions regarding COVID-19 testing and management strategies.
  
2. **Global Comparison**: By comparing testing data across different countries, we can identify best practices and areas needing improvement, facilitating knowledge sharing and collaboration on a global scale.

3. **Public Awareness**: The insights derived from this analysis will be featured in a documentary, helping to educate the public about the importance of COVID-19 testing and the varying responses of different countries.

4. **Data-Driven Insights**: The project leverages advanced data processing techniques to transform raw data into meaningful information, providing a deeper understanding of the pandemic's progression and the effectiveness of testing protocols.

### Project Details

This project is divided into several key tasks, each contributing to the overall goal of extracting and analyzing global COVID-19 testing data:

1. **Data Acquisition**: Using HTTP requests to retrieve COVID-19 testing data from a public Wikipedia page.
2. **Data Extraction**: Parsing the HTML content to extract the relevant data table and converting it into a data frame.
3. **Data Pre-Processing**: Cleaning the data by removing irrelevant columns, renaming columns, and converting data types.
4. **Data Subsetting**: Extracting specific rows and columns for focused analysis.
5. **Ratio Calculation**: Computing the worldwide COVID-19 testing positive ratio to understand the global situation.
6. **Country List Generation**: Creating and sorting a list of countries that have reported their testing data.
7. **Pattern Identification**: Using regular expressions to identify countries with specific naming patterns.
8. **Country Comparison**: Selecting two countries of interest and comparing their testing data.
9. **Ratio Comparison**: Determining which of the selected countries has a higher ratio of confirmed cases to the population.
10. **Threshold Analysis**: Identifying countries with a confirmed to population ratio below a specified threshold.

### Why We Need It

The COVID-19 pandemic is an ongoing global crisis, and understanding its dynamics through data is essential. Testing data provides insights into the spread of the virus, the effectiveness of testing strategies, and the overall preparedness of countries in handling the pandemic. By analyzing this data, we can:

- **Identify Trends**: Detect emerging patterns and trends in COVID-19 testing and infection rates.
- **Improve Response**: Enhance the response strategies of countries by learning from the experiences of others.
- **Support Research**: Provide a valuable dataset for researchers studying the pandemic.
- **Inform the Public**: Educate the public on the importance of testing and the current state of the pandemic globally.

In summary, this project not only aids in understanding the current state of COVID-19 testing worldwide but also contributes to the broader effort to control and eventually overcome the pandemic through data-driven insights.



---

# Global COVID-19 Pandemic Data Analysis

## Overview
This project involves analyzing global COVID-19 testing data by country. The objective is to extract, process, and analyze data to generate insights for a news channel's documentary feature story on global COVID-19 testing. The project is carried out using R within a Jupyter Notebook environment.

## Tasks
The project is divided into 10 tasks, each involving specific steps to process and analyze the data.

### Task 1: Get a COVID-19 Pandemic Wiki Page using HTTP Request
- Use the `httr` package to send an HTTP request to the Wikipedia page containing COVID-19 testing data.
- Extract the content of the page.

### Task 2: Extract COVID-19 Testing Data Table from the Wiki HTML Page
- Use the `rvest` package to parse the HTML content.
- Extract the relevant table containing COVID-19 testing data and convert it into a data frame.

### Task 3: Pre-process and Export the Extracted Data Frame
- Clean the data frame by removing irrelevant columns, renaming columns, and converting columns into proper data types.
- Export the cleaned data frame to a CSV file.

### Task 4: Get a Subset of the Extracted Data Frame
- Read the data frame from the CSV file.
- Extract the 5th to 10th rows with only the "country" and "confirmed" columns.

### Task 5: Calculate Worldwide COVID Testing Positive Ratio
- Calculate the ratio of confirmed cases to the number of tests conducted worldwide.

### Task 6: Get a Country List Which Reported Their Testing Data
- Extract and sort the list of countries that have reported their COVID-19 testing data.

### Task 7: Identify Country Names with a Specific Pattern
- Use regular expressions to find country names that start with a specific pattern, such as "United".

### Task 8: Pick Two Countries and Review Their Testing Data
- Select two countries of interest and review their COVID-19 testing data.

### Task 9: Compare the Selected Countries' Confirmed Cases to Population Ratio
- Compare which of the selected countries has a larger ratio of confirmed cases to the population.

### Task 10: Find Countries with Confirmed to Population Ratio Less Than a Threshold
- Identify countries with a confirmed to population ratio less than a specified threshold to determine lower-risk countries.

## Installation
To run this project locally, ensure you have the following R packages installed:
- `httr`
- `rvest`

You can install these packages using the following commands in R:
```r
install.packages("httr")
install.packages("rvest")
```

