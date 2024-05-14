# Recruitment Analysis Dashboard

This repository highlights the Alteryx data preparation techniques I used to create a fake dataset for my Tableau dashboard project showcasing the financial aspect of the recruitment process.

The majority of the recruitment analysis currently is focussed more on the “People” aspect, the idea was to create a suite of dashboards that can provide an in-depth insight into key financial metrics, helping the clients understand the revenue, cost, and profitability associated with recruitment activities. These dashboards should also be able to help them track the current opportunities and identify gaps that can have growth potential.

![Overview](https://github.com/InsightIngenue/Recruitment-Analysis-Dashboard/assets/169789264/114bd15b-f5db-42cc-a004-e89559dc86d3)

https://github.com/InsightIngenue/Recruitment-Analysis-Dashboard/assets/169789264/1848fcb3-6d36-4ee6-a7b2-dd093356c93e

**Dashboard is available [here]**

[here]: https://public.tableau.com/views/RecruitmentAnalysis_17151917794460/Overview

## Creating the fake dataset

I first shortlisted the measures and metrics that were required in the dataset. Then used a combination of Mockaroo and Alteryx to create the fake dataset.

In Mockaroo, I created 4 different datasets having the same schemas as shown in the image below.
The four datasets had data for different periods spanning a total time period from February 2022 to April 2024.

![Mockaroo](https://github.com/InsightIngenue/Recruitment-Analysis-Dashboard/assets/169789264/86ce28ca-a8c7-4565-9629-39c43fd4691b)

In Alteryx, I used the Random % sample tool to bring in different numbers of rows from these datasets and unioned them.

![Alteryx 1](https://github.com/InsightIngenue/Recruitment-Analysis-Dashboard/assets/169789264/03bebc8a-05e2-4359-adbf-b31eb85418a1)

Then using tools from "Preparation Tool Palette", I did some basic prep to filter the data and create new fields.

![Alteryx 2](https://github.com/InsightIngenue/Recruitment-Analysis-Dashboard/assets/169789264/1f841793-5358-480b-8471-6a731af17fe5)

I then Joined the table containing a list of Account Name, Recruiters Name, Industry, Department, and Salary in the above table. After some more prep, the data was outputted using the Output tool.

![Alteryx 3](https://github.com/InsightIngenue/Recruitment-Analysis-Dashboard/assets/169789264/69365df5-8a91-4adc-85da-d0c3a4e3bb1b)

## Creating the Dashboards

In total, 3 dashboards were created covering the analysis's different aspects.

**1. Overview:** It provides a high-level summary of the financial data i.e. the key KPIs across all departments and accounts.

**2. Breakdown by department:** This Dashboard provides a detailed data analysis by departments. It highlights specific accounts to target for popular or high-profit roles, offering insights into opportunities for the team.

https://github.com/InsightIngenue/Recruitment-Analysis-Dashboard/assets/169789264/5eac00d0-c1e9-4d77-a107-f41ddac75550

**3. Account Analysis:** This Dashboard provides insights into the key metrics and trends of the selected account. It also offers an in-depth analysis to identify untapped opportunities and gaps within the account for expanding services and improving recruitment strategies.

https://github.com/InsightIngenue/Recruitment-Analysis-Dashboard/assets/169789264/96aa863a-a5c5-40e7-ab98-d1b1b3f4cb25

These Dashboards uses following tableau features and functionality:

    Dynamic Parameters
    Parameter Actions
    Drill Down set action
    Level of Detail Expressions (LODs)
    Control Visibility
    Navigation Buttons
    Annotations
    Custom Formatting
