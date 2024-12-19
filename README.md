# BMW 2022-2023 Cars Report 

#### Link of report: https://app.powerbi.com/reportEmbed?reportId=b82b19ac-f117-4feb-954b-b67e557f1329&autoAuth=true&ctid=9f2eb1a9-d1e7-4d23-bbd6-7c54fca48a30
#### Link of project on novypro.com website: https://www.novypro.com/project/which-bmw-fits-you

## 🔍Problem Statement

Finding the perfect car for your needs can be overwhelming, especially when you have to check models and specifications one by one. This time-consuming process makes it difficult to compare features like price, engine type, and other key parameters efficiently.

Additionally, different buyers have unique needs—some may prioritize child lock for family safety, others might need fog lights for better visibility, or voice control for enhanced convenience.

This report solves these challenges with an interactive Power BI dashboard. Users can filter cars based on their preferences and instantly view detailed information about their chosen model, including essential features like child lock, fog lights, voice control, and more. It’s a fast and simple way to find the perfect car for your lifestyle. 


### Key Objectives:
**Simplify Car Selection**

Provide an intuitive platform for users to quickly filter and find the perfect BMW based on their preferences, such as price, engine type, and additional features like child lock, fog lights, or voice control.

**Save Time and Effort**

Streamline the car-buying process by allowing users to compare multiple BMW models at once, eliminating the need to check each car individually.

**Provide Detailed Information**

Offer comprehensive insights on each BMW model, including key specifications, images, pricing, and unique features, helping users make an informed decision tailored to their specific needs.


## 📅Data Overview
Dataset: [New Cars USA 2022/23 dataset](https://www.kaggle.com/datasets/tymekurban/new-cars-usa-202223-dataset?resource=download) from Kaggle.

**Description of the dataset:**
The data was scraped from ccarprice.com and meticulously cleaned. 
It includes:
- Over 2,500 unique cars (only those with price information).
- Almost 80 columns of data covering:
- Technical details such as drivetrain, power, and torque.
- Additional information like body type, car dimensions, equipment, and photo URLs.

I imported the dataset into Power BI for analysis and visualization.
![Screenshot 2024-12-19 160012](https://github.com/user-attachments/assets/0956560b-9619-4709-afdb-c5a721ffc550)

## 🧹 Data Cleaning Story  

The original dataset from Kaggle was far from perfect and required significant preprocessing before any meaningful analysis could be performed. One of the biggest challenges was dealing with inconsistent and incomplete data:

### Steps Taken:
- **Filtering for BMW**: The dataset included multiple car brands, but I focused solely on **BMW** to ensure the analysis was relevant.  
- **Handling Missing Values**: A lot of missing data was present, which I replaced with **null** values. Many entries also had "N/A" written inconsistently as "NA," so I standardized this.  
- **Correcting Formatting Issues**: Several columns had incorrect formatting, which I cleaned up to ensure consistency.  
- **Image URL Formatting**: I updated the formatting of image URLs to correctly link to the images of the cars.  
- **Engine Types**: I added missing engine type names from external sources and standardized engine names, ensuring uniformity across the dataset.  
- **Index Column**: I removed the original index column and added my own, as the dataset was now focused on just **60 BMW cars**.  
- **Year of Manufacture**: I added a **Year of Manufacture** column to better represent the timeline of the cars.

## 🛠️ Tools Used  
- **Power Query**: For ETL (Extract, Transform, Load) processes and data cleaning.  
- **Power BI Desktop**: For creating the interactive report.



