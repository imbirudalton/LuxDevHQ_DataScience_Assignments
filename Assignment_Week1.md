# Assignment 1 
## Data Analysis Dashboard Project

### Project Title
**Jumia Product Performance Dashboard: Analyzing Pricing, Discounts, and Customer Reviews**

---

## Project Objective
The objective of this project is to design and build an interactive Excel dashboard that analyzes the performance of products listed on Jumia. Students will explore how pricing, discounts, reviews, and ratings influence product performance and customer engagement.  

The final dashboard should support data-driven decision-making in an e-commerce context.

---

## Dataset Overview
The dataset contains product-level data with the following columns:

- **Product** – Name of the product  
- **Current Price** – Current selling price in Kenyan Shillings (KSh)  
- **Old Price** – Original price before discount in Kenyan Shillings (KSh)  
- **Discount** – Discount percentage applied to the product  
- **Reviews** – Number of customer reviews  
- **Rating** – Average customer rating out of 5  

---

## Data Cleaning and Preparation
- Check for and handle missing values, especially in the **Reviews** and **Rating** columns  
- Identify and remove duplicate product entries  
- Convert price columns into numeric format by removing “KSh” (use *Text to Columns* under Data tab), commas, and text or use *Find and Replace (Ctrl + H)*  
- Ensure the **Discount** column is numeric and properly formatted as a percentage (use *Find and Replace*, `LEFT/RIGHT` functions, or *Text to Columns*)  
- Convert the **Rating** column from text format (e.g., “4.5 out of 5”) into numeric values  
- Convert negative reviews to positive  

---

## Data Enrichment
Create the following additional columns:

- **Discount Amount (KSh):** Old Price minus Current Price  

- **Rating Category:**
  - *Poor* for ratings below 3  
  - *Average* for ratings between 3 and 4.4  
  - *Excellent* for ratings of 4.5 and above  

- **Discount Category:**
  - *Low Discount* for discounts below 20%  
  - *Medium Discount* for discounts between 20% and 40%  
  - *High Discount* for discounts above 40%  

---

## Data Analysis

### Descriptive Analysis
- What is the average current price, old price, discount percentage, and rating?  
- Which product is the most expensive and which is the least expensive?  
- What is the average rating and discount by discount category?  
- How are products distributed across rating categories?  

### Trend and Relationship Analysis
- Analyze the relationship between discount percentage and number of reviews  
- Analyze the relationship between rating and number of reviews  
- Determine whether higher discounts lead to increased customer engagement  
- Determine whether higher-rated products tend to have more reviews  

### Product Performance Analysis
- Identify the top 10 products with the highest discounts  
- Identify the top 10 products with the most reviews  
- Identify the top 5 highest-rated and bottom 5 lowest-rated products  
- Compare high-discount and low-discount products based on average rating and number of reviews  

---

## Dashboard Design

### Dashboard Requirements
Create a single interactive Excel dashboard containing the following sections:

#### Overview
- Total number of products  
- Average rating  
- Average discount percentage  
- Total number of reviews  

#### Product Performance
- Top products by rating  
- Top products by number of reviews  
- Top products by discount percentage  

#### Trend Analysis
- Visualizations showing discount percentage versus reviews  
- Visualizations showing rating versus reviews  

#### Product Categories
- Breakdown of products by rating category  
- Breakdown of products by discount category  

---

## Visualization Guidelines
- Use **Pivot Tables** as the primary data source  
- Use appropriate charts such as:
  - Bar charts  
  - Column charts  
  - Pie or donut charts  
  - Scatter plots  
- Apply **conditional formatting** to highlight:
  - High discounts  
  - Low ratings  
- Include **slicers** for:
  - Rating category  
  - Discount category  
  - Price range (where applicable)
 
---

##Solution

###Data Cleaning and Preparation
<img width="1919" height="1032" alt="image" src="https://github.com/user-attachments/assets/476ab474-3be3-44c4-8e9a-90df4eab8f58" />

---

###Data Enrichment
<img width="1919" height="1032" alt="image" src="https://github.com/user-attachments/assets/7bb64c8f-07a2-422d-859b-e0b2a4f9bc88" />

---

###Data Analysis
####Descriptive Analysis

*Average current price, old price, discount percentage, and rating?*
Using Pivot Tables
<img width="1919" height="1031" alt="image" src="https://github.com/user-attachments/assets/1da9c9cb-05c3-4e76-91c3-01c272fbb96b" />

*Most expensive and the least expensive Product*
Using MIN and MAX
<img width="1919" height="1031" alt="image" src="https://github.com/user-attachments/assets/20c0bee7-38db-414d-82bc-fcb7eb5ce791" />

*Average rating and discount by discount category*
Using Pivot Tables
<img width="1919" height="1034" alt="image" src="https://github.com/user-attachments/assets/e72b2ef7-a873-4422-8249-767c5859da88" />

*Products distribution across rating categories*
Using Pivot Tables
<img width="1919" height="1032" alt="image" src="https://github.com/user-attachments/assets/087a6ee6-657c-4018-bc07-b99ef89f3ecc" />

---

####Trend and Relationship Analysis

Analyze the relationship between discount percentage and number of reviews
Using Pivot Tables
<img width="1919" height="1035" alt="image" src="https://github.com/user-attachments/assets/02111b4e-7dab-4364-ab6e-a17c4e8108e2" />

Analyze the relationship between rating and number of reviews
Using Pivot Tables
<img width="1919" height="1032" alt="image" src="https://github.com/user-attachments/assets/530065aa-02bd-4472-86de-de7d19d9e119" />

Determine whether higher discounts lead to increased customer engagement


Determine whether higher-rated products tend to have more reviews


####Product Performance Analysis


Identify the top 10 products with the highest discounts


<img width="1918" height="1027" alt="image" src="https://github.com/user-attachments/assets/8729932e-f582-4328-857f-0c9245948a9d" />


Identify the top 10 products with the most reviews


<img width="1919" height="1031" alt="image" src="https://github.com/user-attachments/assets/0643baa9-c043-4b9a-96d2-ae593ff113a4" />


Identify the top 5 highest-rated and bottom 5 lowest-rated products


<img width="1919" height="1031" alt="image" src="https://github.com/user-attachments/assets/210428eb-d2cc-4070-ba9d-4165d631c810" />


<img width="1916" height="1031" alt="image" src="https://github.com/user-attachments/assets/7fe36994-d254-4d79-a376-10ec6df48643" />



Compare high-discount and low-discount products based on average rating and number of reviews


<img width="1918" height="1029" alt="image" src="https://github.com/user-attachments/assets/7a849cb5-2fae-4e58-af94-990665ea0672" />

###Dashboard
<img width="1919" height="1032" alt="image" src="https://github.com/user-attachments/assets/467ebe72-99cc-42f3-abbb-8f4a9fdc6506" />


<img width="1919" height="1033" alt="image" src="https://github.com/user-attachments/assets/bf74c83a-383e-4bab-8041-5fd131f969ce" />





