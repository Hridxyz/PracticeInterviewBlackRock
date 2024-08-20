
### **General Questions:**

1. **Q: Can you give an overview of the project?**
    - **A:** The project involved analyzing data from the T20 World Cup using a combination of web scraping, data transformation, and visualization techniques. The main goal was to build a Power BI dashboard that could help select the best players based on various performance metrics like batting average, strike rate, and bowling economy.

2. **Q: What tools and technologies did you use in this project?**
    - **A:** The project used several key tools and technologies:
        - **Web Scraping:** JavaScript and Bright Data to scrape data from ESPNcricinfo.
        - **Data Transformation:** Python and Pandas to clean and transform the data.
        - **Data Visualization:** Power BI to create interactive dashboards.
        - **Data Storage Formats:** JSON for raw data, which was later converted to CSV for analysis.

3. **Q: What were the main challenges you faced during this project?**
    - **A:** One of the main challenges was ensuring accurate data scraping, as websites like ESPNcricinfo can have complex structures and may change frequently. Another challenge was handling missing or incomplete data during the transformation process, which required careful cleaning and validation to ensure the quality of the final dataset.

### **Web Scraping Specific Questions:**

4. **Q: How did you perform web scraping for this project?**
    - **A:** We used JavaScript code within Bright Data, a tool that facilitates seamless data collection by navigating through ESPNcricinfo's website and extracting relevant match and player data. The scraped data was stored in JSON format, which was later processed for analysis.

5. **Q: Why did you choose Bright Data for web scraping?**
    - **A:** Bright Data offers a robust infrastructure for web scraping, including smart proxy networks that prevent IP blocking and ensure consistent data collection. This was particularly important for scraping large datasets from a popular site like ESPNcricinfo without interruptions.

6. **Q: What kind of data did you scrape from ESPNcricinfo?**
    - **A:** The data scraped included match results, batting and bowling summaries, and detailed player information such as batting style, bowling style, and performance statistics for each match.

### **Data Transformation and Cleaning Questions:**

7. **Q: How did you clean and transform the scraped data?**
    - **A:** The data, initially in JSON format, was transformed using Python and Pandas. This involved flattening the nested JSON structures into tables, handling missing values, creating new columns like "out/not out," and exporting the cleaned data as CSV files for further analysis.

8. **Q: Can you explain how you handled missing data?**
    - **A:** Missing data was identified during the cleaning process. For example, if a player's dismissal status was missing, it was inferred that the player was "not out." Such logical assumptions were applied, and necessary transformations were made to ensure the data was consistent and complete.

9. **Q: What were the key transformations you applied to the data?**
    - **A:** Key transformations included renaming columns for clarity, calculating additional metrics like "boundary percentage," and creating match IDs to link different datasets (e.g., match results with player performances).

### **Power BI and Data Modeling Questions:**

10. **Q: How did you use Power BI in this project?**
    - **A:** Power BI was used to create an interactive dashboard that visualized the performance of players. We imported the cleaned CSV files, established relationships between datasets, and built various visualizations like scatter plots, bar charts, and trend lines to analyze and present the data.

11. **Q: Can you describe the data modeling process in Power BI?**
    - **A:** Data modeling in Power BI involved linking fact tables, such as batting and bowling summaries, with dimension tables, like player information. Relationships were established using unique identifiers like match IDs and player names, which allowed for comprehensive analysis across different datasets.

12. **Q: What DAX measures did you create, and why?**
    - **A:** We created several DAX measures to enhance data analysis, such as:
        - **Total Runs:** Sum of all runs scored by a player.
        - **Strike Rate:** Calculated as (total runs/total balls faced) * 100.
        - **Boundary Percentage:** Percentage of runs scored from boundaries.
          These measures were crucial for creating dynamic visualizations that could filter and display data based on specific criteria.

### **Dashboard and Visualization Questions:**

13. **Q: How did you design the dashboard in Power BI?**
    - **A:** The dashboard was designed with multiple pages, each focusing on a specific player role (e.g., Power Hitters, Anchors, Fast Bowlers). Filters and slicers were used to refine player selections based on criteria like batting average and strike rate. We also included interactive elements, allowing users to explore different scenarios and player combinations.

14. **Q: What insights were you able to gain from the dashboard?**
    - **A:** The dashboard provided insights into player performance across different roles, helping to identify the best players for specific positions. For example, we could compare the strike rates and batting averages of different players to select the most effective openers or middle-order batsmen.

15. **Q: How did you ensure that the dashboard was user-friendly?**
    - **A:** We focused on clear visualizations and intuitive navigation. The use of filters, slicers, and well-organized pages made it easy for users to explore the data and find the information they needed. We also tested the dashboard with potential users to ensure it met their needs and expectations.

### **Project-Specific Questions:**

16. **Q: How did you handle linking data across different tables in Power BI?**
    - **A:** We used match IDs and player names as keys to establish relationships between tables in Power BI. This allowed us to link batting and bowling summaries with match results and player information, enabling comprehensive analysis.

17. **Q: What was the most challenging aspect of this project?**
    - **A:** The most challenging aspect was ensuring the accuracy and completeness of the data during the scraping and transformation stages. Web scraping can be error-prone, and ensuring that all relevant data was accurately captured and transformed required careful validation and testing.

18. **Q: How did you validate the accuracy of your data?**
    - **A:** We validated the data by cross-referencing the scraped data with the original source on ESPNcricinfo and by running checks in Power BI, such as comparing calculated metrics against known values (e.g., checking total runs scored by a player against match reports).

### **Reflection and Learning Questions:**

19. **Q: What did you learn from this project?**
    - **A:** This project taught me how to manage the entire data analytics pipeline, from data collection to final visualization. I gained hands-on experience with web scraping, data transformation using Pandas, and creating insightful visualizations in Power BI. It also reinforced the importance of data accuracy and the power of interactive dashboards in making data-driven decisions.

20. **Q: If you were to do this project again, what would you do differently?**
    - **A:** If I were to do this project again, I would explore using more advanced machine learning techniques to predict player performance or simulate match outcomes. Additionally, I would focus on automating more parts of the workflow, such as using APIs for data collection instead of manual web scraping.

