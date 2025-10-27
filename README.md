# DATA607_Week9_Assignment
This assignment pulls the latest Technology Top Stories from the New York Times API, converts the data into a tidy table in R, runs basic validation checks, and summarizes key themes found in the most recent headlines.

Week 9 – NYTimes Top Stories API (Technology)

This project demonstrates how to access the New York Times Top Stories API for the Technology section using R, convert the JSON response into a tidy data frame, conduct basic validation checks, and summarize insights from the latest tech headlines.

What This Project Does

• Connects to the NYT Top Stories API
• Retrieves the latest Technology news headlines
• Parses JSON into a tidy R data frame
• Performs basic data validation (checking columns, missing values, dates)
• (Optional) Saves results to a CSV file
• Summarizes key themes from the current tech news cycle
 
Skills Demonstrated

Area                              Skills

API Integration      - Performing HTTP GET requests - Managing authentication - Utilizing query parameters

Data Wrangling       - Parsing JSON data - Filtering and cleaning datasets - Converting data to tibbles

Data Validation      - Verifying columns - Checking for missing (NA) values - Validating date ranges

Reproducibility      - Structuring reproducible scripts using environment variables
 
How to Run This Project
1.	Clone or download this repository
2.	Open RStudio and open the .Rproj file (recommended)
3.	Install required packages (if needed):
install.packages(c("httr2","jsonlite","dplyr","tidyr","readr"))
4.	Add your NYT API key (Required)
To keep your key private, add it to your .Renviron file:
usethis::edit_r_environ()
Then add this line inside the file (replace with your own key):
NYT_API_KEY=your-key-here
Save, close, and restart R.
5.	Run the safe Rmd:
key <- Sys.getenv("NYT_API_KEY")
 

Repository Contents
File	Description
week9safe.Rmd	Safe version of assignment without API key
week9.Rproj	Project file for easy RStudio setup
nyt_topstories.csv (optional)	Output sample of tech headlines retrieved from API
README.md	You are here
 
About API Key Safety
The original Rmd with the actual API key is not included for security reasons.
Anyone using this project can add their own key to run the script.
This teaches best practice for working with APIs—never commit secrets to a public repo.
 
Summary of Insights
The most recent NYT tech headlines commonly focus on themes such as:
•	AI in education and workplace settings
•	Tech layoffs and industry job shifts
•	Crypto-related regulation and enforcement
•	Social media + tech culture news
(Your actual findings may vary based on the day the script is run.)
 
Author
Kevin Martin
CUNY School of Professional Studies – DATA 607
Fall 2025
<img width="468" height="650" alt="image" src="https://github.com/user-attachments/assets/423c1935-0d5a-463c-9f6f-eb1a5c00bc2b" />
