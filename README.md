# Quote-ETL-Pipleine
This project is a Python-based ETL (Extract, Transform, Load) pipeline designed to automate the process of web data collection, cleaning, transformation, and cloud storage.
The pipeline scrapes structured data from the web using Beautiful Soup, processes it using Pandas, and stores the final cleaned dataset as a JSON file in an AWS S3 bucket.

<strong>Key Features</strong>

Web Scraping: Uses Beautiful Soup to extract data from targeted web pages.

Data Cleaning & Transformation: Employs Pandas to handle missing values, normalize fields, and format data for downstream use.

Cloud Integration: Uploads the processed dataset to an Amazon S3 bucket for scalable and secure storage.

Automation-Ready: Can be easily scheduled or extended for continuous data collection workflow




<strong>Tech Stack</strong>

Language: Python 3.x

<strong>Libraries:</strong>

pandas — data manipulation and cleaning

beautifulsoup4 — web scraping

boto3 — AWS SDK for S3 interactions

requests — for fetching webpage content



<strong>Process</strong>
1. Extract

Data is scraped from target web pages using requests and parsed with BeautifulSoup.
The script extracts relevant fields such as titles, dates, links, or numerical data.

2. Transform

The raw data is loaded into a Pandas DataFrame where cleaning operations are performed:

Handling missing or duplicate values

Converting data types

Renaming and structuring columns

Normalizing or aggregating fields

The cleaned dataset is then exported to JSON format.

3. Load

The JSON output is uploaded to an AWS S3 bucket using boto3.
This enables centralized storage and easy integration with analytics tools or downstream pipelines.
