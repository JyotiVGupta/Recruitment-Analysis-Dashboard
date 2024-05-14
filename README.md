# Recruitment Analysis Dashboard

This repository highlights the Alteryx data preparation techniques I used to create a fake dataset for my Tableau dashboard project showcasing the financial aspect of the recruitment process.

The majority of the recruitment analysis currently is focussed more on the “People” aspect, the idea was to create a suite of dashboards that can provide an in-depth insight into key financial metrics, helping the clients understand the revenue, cost, and profitability associated with recruitment activities. These dashboards should also be able to help them track the current opportunities and identify gaps that can have growth potential.

![Overview](https://github.com/InsightIngenue/Recruitment-Analysis-Dashboard/assets/169789264/dbabfd49-b4e1-4086-a34b-65feda2129f1)

https://github.com/InsightIngenue/Recruitment-Analysis-Dashboard/assets/169789264/75ea4d83-d1d2-4bde-968b-2977c1d5697c

**Dashboard is available [here]**

[here]: https://public.tableau.com/views/RecruitmentAnalysis_17151917794460/Overview

## Creating the fake dataset

I first shortlisted the measures and metrics that were required in the dataset. Then used a combination of Mockaroo and Alteryx to create the fake dataset.

In Mockaroo, I created 4 different datasets having the same schemas as shown in the image below.
The four datasets had data for different periods spanning a total time period from February 2022 to April 2024.

![Mockaroo](https://github.com/InsightIngenue/Recruitment-Analysis-Dashboard/assets/169789264/39dd4fc5-6658-4ecd-a872-56308220e2e4)

In Alteryx, I used the Random % sample tool to bring in different numbers of rows from these datasets and unioned them.

![Alteryx 1](https://github.com/InsightIngenue/Recruitment-Analysis-Dashboard/assets/169789264/cd56a1a2-789e-4bac-acef-08171b00d614)

Then using tools from "Preparation Tool Palette", I did some basic prep to filter the data and create new fields.

![Alteryx 2](https://github.com/InsightIngenue/Recruitment-Analysis-Dashboard/assets/169789264/7dd4ed68-de88-4699-99ec-1f319cc053da)

I then Joined the table containing a list of Account Name, Recruiters Name, Industry, Department, and Salary in the above table. After some more prep, the data was outputted using the Output tool.

![Alteryx 3](https://github.com/InsightIngenue/Recruitment-Analysis-Dashboard/assets/169789264/2e943738-462a-42d8-926b-a41818848df3)

## Creating the Dashboards

In total, 3 dashboards were created covering the analysis's different aspects.

**1. Overview:** It provides a high-level summary of the financial data i.e. the key KPIs across all departments and accounts.

**2. Breakdown by department:** This Dashboard provides a detailed data analysis by departments. It highlights specific accounts to target for popular or high-profit roles, offering insights into opportunities for the team.

https://github.com/InsightIngenue/Recruitment-Analysis-Dashboard/assets/169789264/513b7f54-6989-4922-9d61-f1abdd041271

**3. Account Analysis:** This Dashboard provides insights into the key metrics and trends of the selected account. It also offers an in-depth analysis to identify untapped opportunities and gaps within the account for expanding services and improving recruitment strategies.

https://github.com/InsightIngenue/Recruitment-Analysis-Dashboard/assets/169789264/4a28fe79-5ae9-447d-acbb-ca17f5a4dd7d

These Dashboards uses following tableau features and functionality:

    Dynamic Parameters
    Parameter Actions
    Drill Down set action
    Level of Detail Expressions (LODs)
    Control Visibility
    Navigation Buttons
    Annotations
    Custom Formatting
