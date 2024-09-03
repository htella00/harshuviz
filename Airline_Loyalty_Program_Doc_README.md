# Airlines_Loyalty_Program-Dashboard

## Problem Statement

You've been hired as the Marketing Analyst for Northern Lights Air (A fictious Canadian Airline) and they're looking to boost enrollment for their royalty program. NLA ran a promotion from
Feb 1st - Apr 30th 2018, offering 1.5x loyalty card points to new members for flights booked through the remainder of the year.
The task is to analyze loyalty program enrollments, cancellations and flights booked and share your findings with the leadership

### Steps Followed 

- Step 1 : Loaded Data from the data source, in my case it is the Maven Analytics website.
- Step 2 : Explored and QA the data and ensured the column headers and data types are accurate.
- Step 3 : Added columns to the Customer Loyalty History Table to Calculate the enrollment start of Month and Cancellation of Months
- Step 4 : Added columns to Customer Flight Activity to calculate the flight booked at the start of the month, also added a binary column to Customer Loyalty to flag if a Customer has cancelled
- Step 5 : Built a data model to connect the Calendar, Customer Loyalty History and Customer Flight Activity tables at the "start of month" fields
- Step 6 : Created DAX measures to calculate total enrollments.
- Step 7 : Created measures to calculate total cancellations and net loyalty members (new canceled)
- Step 8 : Created measures to calculate the running total of net loyalty members over time
- Step 9 : Created measures to calculate flights booked by loyalty members (based on start of month) and flights booked by loyalty members the previous year
- Step 10 : Finally, Added appropriate visualizations to show the patterns and trends

### Findings 
- Based on the analysis we can summarize the promotion's impact to the leadership in terms of enrollment volume and loyalty flights booked by looking at the year over year trend from 2017 to 2018, we can observe that the trend is increasing, one of the main drivers of that in 2018 is the Promotion Activity.
- If we look at the standard enrollment type in Jul 2018, there are around 3000 enrollments but we also include the 2018 promotion as well, there are 9000 enrollments year over year during the peak period
- Therefore we can say in terms of the promotion effectiveness it did have the desired effect and when we come out the promotion period at the end of April and we see an increase in volume and loyalty member flights booked and it is driven by the increase in the Loyalty Member Signups during the promotion period.

![Screenshot 2024-09-03 123952](https://github.com/user-attachments/assets/bebbf733-e02c-4b1a-a344-f305bf20b898)
![Screenshot 2024-09-03 124108](https://github.com/user-attachments/assets/18853650-6bee-4834-8e79-3fd80f038803)

### Recommendations
- Based on the Findings, we can consider repeating the promotion in future years, or extending the promotion period slightly, to capture even more enrollments. We might also explore offering the promotion during other high-traffic periods to see if similar trends hold.
- We can develop retention strategies, such as personalized offers or exclusive member benefits, to keep newly enrolled members engaged and prevent cancellations after the promotion ends.
- Test other promotional strategies, such as offering bonus points for certain flight routes, seasonal promotions, or tiered rewards based on member activity. Conduct A/B testing to determine which types of promotions are most effective.
- Continue monitoring loyalty member activity and flight bookings throughout the year and into the next to assess the sustained impact of the promotion. Use this data to refine future promotions and loyalty strategies.

### Snapshot of the Final Dashboard
![Screenshot 2024-09-03 125545](https://github.com/user-attachments/assets/10302989-57b0-4f76-9733-9ed65d418707)
