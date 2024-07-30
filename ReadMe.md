# Module 11 Challenge: Mars News and Weather 

## Overview

The purpose of the module 11 challenge is practice extracting information via  Splinter and Beautiful Soup.There are two main parts to the challenge: 
    1. Scraping titles and preview text from Mars news articles. 
    2. Scraping and analyzing Mars Weather data 
    
###Part 1: Scrape Titles and Preview Text from Mars News
    1. Open the Jupyter Notebook named part_1_mars_news.ipynb.
    2. Use automated browsing with Splinter to visit the Mars news site and inspect the page to identify which elements to scrape.
    3. Create a BeautifulSoup object and use it to extract text elements from the website.
    4. Extract the titles and preview text of the news articles and store them in a list of dictionaries.
    5. Print the list in your notebook.
    6. Optionally, export the scraped data to a JSON file.
###Part 2: Scrape and Analyze Mars Weather Data
    1. Open the Jupyter Notebook named part_2_mars_weather.ipynb.
    2. Use automated browsing to visit the Mars Temperature Data Site and inspect the page to identify which elements to scrape.
    3. Create a BeautifulSoup object and use it to scrape the data in the HTML table.
    4. Assemble the scraped data into a Pandas DataFrame with the correct column headings.
    5. Convert the data to the appropriate data types.
    6. Analyze the dataset using Pandas functions to answer the following questions:
        a. How many months exist on Mars?
        b. How many Martian days' worth of data exist in the scraped dataset?
        c. What are the coldest and the warmest months on Mars?
        d. Which months have the lowest and the highest atmospheric pressure on Mars?
        e. About how many terrestrial days exist in a Martian year?
   7. Export the DataFrame to a CSV file.

## Files
- 'mars_challenge'(https://github.com/jackthomas1430/mars_challenge.git) :The main repo for this challenge.
-'mars_scrapping_analysis': Directory containing all files for the module 11 challenge 
    -part_1_mars_news.ipynb: Jupyter notebook containing code to scrape Mars news titles and preview text.
    -part_2_mars_weather.ipynb: Jupyter notebook containing code to scrape and analyze Mars weather data.
    - 'starter_code': contains two jupyter notebooks to use as starter code for the analysis 
    - 'Results': directory containing exported data and images of the results 
        -'mars_news.json': Mars News data exported in JSON format
        -'mars_weather.csv': Mars Weather data saved to csv
    
## Instructions
1. Install the following Python libraries if they are not already installed:
    -pip install splinter
    -pip install beautifulsoup4
    -pip install pandas
    -pip install matplotlib
2. Clone the repository to your local device using git clone (https://github.com/jackthomas1430/mars_challenge.git)
3. Open the Jupyter Notebook named part_1_mars_news.ipynb and run to scrape titles and preview text from Mars News
4. Open the Jupyter Notebook named part_2_mars_weather.ipynb and run to scrape and analyze Mars Weather Data

##Results/Analysis: 
1. Number of months on Mars
    ![number_of_months](mars_challenge/mars_scrapping_analysis /Results/number_of_months.png)
2. Number of Martian days of data
    1867
3. Average minimum daily temperature by month
    ![avg_temp_mars](mars_challenge/mars_scrapping_analysis /Results/avg_temp_mars.png)
    ![avg_temp_plot](mars_challenge/mars_scrapping_analysis /Results/avg_min_temp.png)
4. Identify the coldest and hottest months in Curiosity's location
    ![coldest_warmest_month](mars_challenge/mars_scrapping_analysis /Results/coldest_warmest_month.png)
    The coldest month on Mars is month 3 with an average minimum temperature of -83.31°C.
    The warmest month on Mars is month 8 with an average minimum temperature of -68.38°C. 
4. Average atmospheric pressure by month
    ![avg_pressure](mars_challenge/mars_scrapping_analysis /Results/avg_pressure_month.png)
    ![avg_pressure_plot](mars_challenge/mars_scrapping_analysis /Results/avg_pressure_plot.png)
    Atmospheric pressure is, on average, lowest in the sixth month and highest in the ninth.
5. Visualization of the daily minimum temperature over time to estimate the length of a Martian year
    ![terrestrial_days](mars_challenge/mars_scrapping_analysis /Results/terrestrial_days.png)
    A year on Mars appears to be about 675 days.
     
##Acknowledgements
    Xpert Learning Assistant was used to answer detailed questions, and assist in debugging.For more information about the Xpert Learning Assistant, visit [EdX Xpert Learning Assistant](https://www.edx.org/). 
    
##References
- [Beautiful Soup Documentation — Beautiful Soup 4.4.0 documentation](https://beautiful-soup-4.readthedocs.io/en/latest/)
- [CSS Selectors](https://beautiful-soup-4.readthedocs.io/en/latest/#css-selectors)
- [HTML Tags](https://www.w3schools.com/tags/)
-The Mars News websiteLinks to an external site. is operated by edX Boot Camps LLC for educational purposes only. The news article titles, summaries, dates, and images were scraped from NASA's Mars NewsLinks to an external site. website in November 2022. Images are used according to the JPL Image Use PolicyLinks to an external site., courtesy NASA/JPL-Caltech.

