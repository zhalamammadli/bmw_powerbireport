# BMW 2022-2023 Cars Report 
![Cars-1](https://github.com/user-attachments/assets/7f99c758-d7fb-4547-b891-81e0015b7be0)

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
- **Power Query**: 
- For ETL (Extract, Transform, Load) processes and data cleaning.  
 - *Filtering*: Used to focus on BMW cars and remove irrelevant data.  
 - *Replacing Values*: Standardized missing data and inconsistencies like "N/A" to "null".  
 - *Renaming Columns*: Cleaned up column names to ensure consistency.
 - *Changing Format*: Corrected the formatting of various columns, including image URLs and engine types.

- **Power BI Desktop**: 
For creating the interactive report.
- *"Simple Image" Visualization*: Displayed car images based on the selected model.  
- *Cars*: Displayed relevant car information and specifications.  
- *Tile Slicers*: Used to filter cars based on key attributes such as price, engine type, and features.  
- *Tiles*: Displayed key information in a visually appealing format.  
- *Button to Clear All Parameters*: Enabled users to reset filters with a single click.  
- *Slicers*: Allowed users to select and filter data based on their preferences (e.g., price, year, engine type).

## 📈 Report Insights

This Power BI report offers a detailed, interactive view of BMW cars, allowing users to explore various car models and find the one that best suits their needs. Here are some key insights:

### Key Features:
- **Interactive Filters**: Users can filter cars based on parameters like **price**, **engine type**, **year of manufacture**, and specific features such as **child lock**, **fog lights**, and **voice control**.
- **Car Comparison**: The report allows users to compare multiple BMW models to make an informed decision.
- **Detailed Information**: Each car model includes essential details such as:
  - *Price*
  - *Engine specifications*
  - *Car dimensions*
  - *Additional equipment* (e.g., safety features, tech options)
  - *Image and visual details* to enhance user experience
- **User-Friendly Interface**: The design ensures an easy-to-navigate interface, with features like:
  - *Tile Slicers*: To quickly filter cars by attributes like price, engine, or year.
  - *"Simple Image" Visualization*: Displaying car images for a better visual comparison.
  - *Clear All Parameters Button*: Allows users to reset all filters with a single click.

### Key Takeaways:
- *Simplified Decision Making*: By providing all essential information in one place, the report helps users make faster, data-driven decisions about which BMW model is the best fit for their needs.
- *Comprehensive Insights*: Users gain detailed insights into the cars they are considering, helping them understand not only the technical specifications but also the features that matter most to them.
- *Enhanced User Experience*: The combination of interactive features and visually appealing design ensures that the process of finding the right BMW is both easy and enjoyable.
