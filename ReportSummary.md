# BeverageSalesReport
Overview:  
     For this project, I worked with a dataset that shows how different beverages were sold in different regions. The goal was to analyze sales trends ,better understand how much was sold, where it was sold, and which types of drinks made the most money.  The                motivation behind this project stems from a personal interest in data visualization and dashboard creation. As someone who enjoys transforming raw data into clear and engaging reports, I saw this as an opportunity to apply and demonstrate my skills. The final report      includes nine visuals that help explain the data in a clear and simple way. These visuals show top car brands, sales by month, and other helpful insights. 

Data Structure: 
      The dataset I worked with is large, containing over 9 million rows and 11 columns. Each row represents a single beverage order, and the columns store important details about each sale.

     Here’s a breakdown of the columns in the dataset:

      Order Number: A unique number given to each order

     Customer ID: An ID used to track which customer placed the order

    Customer Type: Shows whether the customer is a new or returning customer, or part of a specific group

    Product: The name of the beverage that was sold

    Category: Groups the product into types like soda, juice, energy drink, etc.

    Unit Price: The price for one item

    Quantity: How many units were purchased in the order

    Discount: The discount applied to the item, usually shown as a decimal (like 0.10 for 10%)

    Total Price: The final cost after applying the discount

    Region: The geographic area where the order was placed (like North, South, East, West)

    Order Date: The date the order was placed

    This data structure makes it possible to analyze sales from many angles — like by customer, product, category, or region. It also supports deeper analysis like total revenue, discount savings, and sales trends over time.

Data Model:
  For this project, I used a star schema data model to organize the information. The main table is called the Sales table, which is the fact table. This table contains the core data about each beverage sale — like the order number, product sold, quantity, unit price,      discount, and total price. It also includes columns that connect to other tables through relationships.

   In addition to the fact table, I created several dimension tables to help organize and analyze the data:

   Product Table: Contains a list of all products with their names and categories

   Region Table: Lists all the regions where sales took place

    Category Table: Stores different product categories like soda, juice, or water

    Customer Type Table: Breaks customers into types 

   Date Table: A calendar table that helps analyze sales by year, month, or day

   Each dimension table is linked to the Sales table using a key (such as Product or Region), which allows me to slice and filter the sales data easily in Power BI. This setup makes it easier to build dashboards and perform analysis by different parts of the business.


Findings:  
    After analyzing the beverage sales data, I discovered several interesting insights:

  February had the lowest sales of the year. This could be due to seasonal changes or fewer events and holidays during that month.

   The beverage that brought in the most money was Veuve, with over $200 million in revenue. This shows it was a top-selling or premium product.

   Across all sales, customers saved a total of $96 million through discounts. This shows that discounts played a big role in pricing and customer attraction.

   When comparing customer types, business customers generated the most revenue compared to other customer types. This may be because businesses tend to place larger or more frequent orders.

   Sales were evenly split among the four main beverage categories — water, juice, alcohol, and soda. This shows a balanced customer interest across all types of drinks.

   These findings help give a better understanding of product performance, customer behavior, and seasonal trends, which are useful for business decision-making.

Data Preperation:
  Before analyzing the data, I spent time preparing and cleaning it to make sure everything was accurate and easy to work with. First, I removed any unwanted columns that weren’t useful for the analysis to keep the data clean and focused. I also extracted specific parts   of text from some columns, like pulling out category names or customer types from longer text values.

  I replaced certain values to make them more readable or consistent — for example, turning short codes into full names. I also renamed columns to make them easier to understand and work with in visualizations. In some cases, I had to change the format of columns, such    as converting text to dates or numbers so they could be used in charts and calculations.

  Finally, I created a separate date table to help with time-based analysis, like tracking sales by month or year. This made it easier to build visuals that show trends over time and helped connect the data model together.
