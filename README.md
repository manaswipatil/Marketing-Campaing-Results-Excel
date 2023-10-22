# Marketing-Campaing-Results-Excel

***The Brief:***
Maven Marketing campaign data of 2,240 customers of Maven Marketing, including customer profiles, product preferences, campaign successes/failures, and channel performance.
Records from July 2012 - June 2014

**Following are some questions we will try to answer in this dashboard:**
- Are there any null values or outliers? How will you handle them?
- What factors are significantly related to the number of web purchases?
- Which marketing campaign was the most successful?
- What does the average customer look like?
- Which products are performing best?
- Which channels are underperforming?

***Data Cleaning and Transformation:***

- Calculated age as of 2014.
Created age groups as 18-25 - Young, 26-35 - Adult, 36-55 = "Middle Age", 55 above - "Senior".
- Check for Outliers:
There were 3 customers (ID - 11004, 1150, 7829) with birth_year - 1893, 1899, 1900 who are over 100 years old. If there are more customers then this information can be sent to data engineer team for validation, but here I have removed them from dataset
- There are 201 customers whose education is listed as 2n cycle which is equivalent to Masters degree. Hence updated those records to 'Masters' as education.
- There are customers with Marital_Status as Absurd, Alone, YOLO, so I updated their status as 'Single'.
- There were 4 customers (ID - 3955, 11110, 5555, 11181) with 0 purchases via offers, web, catalouge or store, bu they had a dollar amount in transaction columns for food catagories. removed these records from dataset.

***Dashboard Screenshot:***
![Dashboard](https://github.com/manaswipatil/Marketing-Campaing-Results-Excel/assets/50437663/f94a8024-a507-4812-bd3b-58a07818cfc3)
