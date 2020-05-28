# Lab 700: Oracle Analytics for Applications (OAX) for Fusion ERP

<!-- Comment out table of contents
## Table of Contents
[Introduction](#introduction)
-->

## Introduction

-   In this lab, you will learn about how a finance team can adress analytics questions through Oracle Analytics  for Applications (OAX) for Fusion ERP.
-   Finance teams are under enormous pressure to generate more insights, faster, from their financial systems and other critical data sources. But for most organizations, far too much time is spent manually sourcing, managing, preparing, and securing data – leaving far too little time for true analysis and insight.
-   Oracle Analytics for Fusion ERP provides the fastest path to insight with your ERP data, based on its pre-built integration to your ERP Cloud, pre-built data model, and pre-built interfaces – including KPIs, dashboards, and self- service project areas that you can use to easily customize and extend your analysis. And, it’s all built on the foundation of Oracle Analytics Cloud and the self-tuning, self-scaling, self-securing Oracle Autonomous Data Warehouse.
-   This workshop is designed to give you a hands-on experience with both the pre-built elements of Oracle Analytics for Fusion ERP – with a focus on KPIs and dashboards – as well as the intuitive self-service capabilities delivered by the underlying Oracle Analytics Cloud platform.

**_To log issues_**, click here to go to the [github oracle](https://github.com/oracle/learning-library/issues/new) repository issue submission form.

### Objectives

-   Learn how to use the interface through KPI Cards, Decks, Alerts, and Analysis
-   Learn how to perform a Custom Analysis on a Pre-Built Profitability Subject Area
-   Learn how to explore a Balance Sheet Subject Area and create a Trial Balance
-   Learn how to explore an Account Payables Project and create new reports 
-   Learn how to extend analysis with external data

### Required Artifacts

-   The following lab requires an Oracle Public Cloud account. You may use your own cloud account, a cloud account that you obtained through a trial, or a training account whose details were given to you by an Oracle instructor.
-   *To access the workshop environment*, you will need internet access and a modern web browser. Your instructor will provide you with a URL for the OAX instance and you will be assigned a username and password. Please refer to your instructor's confluence page for details. 
-   The estimated time to complete this lab is 40 minutes.

### Extra Resources
-   To learn more about Oracle Analytics for Applications (OAX), feel free to explore the capabilities by clicking on this link: [OAX Getting Started Documentation](https://docs.oracle.com/en/cloud/saas/analytics/fawag/get-started-oracle-analytics-applications.html#GUID-66FF30CB-C4C4-4184-9223-DE5AE3E83C80)

## Part 1. Explore the Interface and Pre-Built Content: KPI Cards, Decks, Alerts, and Analysis

### **Step 1:** 

-   Enter the credentials you were given and click the **Sign In** button.

![](./images/1.png)

### **Step 2:** 

-   We start at the homepage, where contains KPIs and Decks that you have marked as favorites. Since this is the first time you have logged in, the screen will be blank. Let’s explore how to navigate within the application.

-   Click on the upper left **hamburger menu** icon to see the following:
-   **Decks** are how KPIs are presented and organized. 
-   **KPIs** is where you can createand edit the Key Performance Indicators library.
-   **Projects** is where you can create and edit analysis and reports.
-   **Data** is where you manage data access and workflows. 

![](./images/2a.png)

-   Click on **Decks**.

![](./images/2b.png)

### **Step 3:** 

-   Now, take a moment to review a few of the pre-built decks. From left to right, click on the following:
-   **Profit and Loss**
-   **Payables**
-   **Balance Sheet**
-   **Financial Ratios**

-   Take a moment to look at the pre- built KPIs on each deck.

![](./images/3.png)

### **Step 4:** 

-   From the **Financial Ratios** deck, click the **filter icon** on the top right.

-   **Note** that the current deck is filtered by Current Quarter by default. You can easily change the filter here to focus on a different context, such as business unit, cost center, time, etc.

-   Click the **filter icon** again to make it disappear.

![](./images/4.png)

### **Step 5:** 

-   Click on **My P&L** – a custom deck that we have created and shared with you. Every user can easily create their own custom decks with the top KPIs they want to monitor.

-   **Note** that a deck contains one or more KPI “cards.”

-   Each KPI card can be customized in numerous ways. In addition to the visualization, observe that the Revenue KPI Card contains the following:
-   An **Alert** (the top line is green – as Revenue is above target)
-   A Comparison to **Target**
-   A Comparison to **Previous Time Period**

![](./images/5.png)

### **Step 6:** 

-   On this deck, we notice that although Revenue is above target, Operating Expenses are trending up.
-   From each KPI, it’s very easy to drill into deeper insights about your finance data. Let’s drill in to OPEX to explore further.

-   Click on the **OPEX KPI card hamburger menu icon**.

-   Select **Operating Expense Analysis**.

![](./images/6.png)

### **Step 7:** 

-   This pre-built analysis provides additional visualizations to highlight and accelerate further analysis.

-   Observe the following:
-   Trailing 12 months andquarterly operating expenses are increasing.
-   The tree map visualization shows that the Call Center is the top area for expense.
-   In the bottom bar chart, we see a spike in payroll cost.

-   Finally, click on the **back arrow** at the upper left of the screen to return to the deck.

![](./images/7.png)

### **Step 8:** 

-   We’re now back on the My P&L deck, which was shared with you with “view only” access. We want to dig deeper into payroll cost, so we’ll create a new custom deck that we can customize to meet our needs:

-   Click the **hamburger menu icon** on the top right.

-   Select **Add Deck**.

![](./images/8.png)

### **Step 9:** 

-   Name your deck “Payroll Deck.” 

-   Click the **Save** button.

![](./images/9.png)

### **Step 10:** 

-   First, let’s add the **Payroll Cost KPI** to this new deck.

-   Click the **+ icon**.

![](./images/10.png)

### **Step 11:** 

-   **Scroll** through the KPI library so you can see all of the out of the box KPIs.

-   Select **Payroll Cost PL KPI**

-   **Note**: You see two Payroll Cost KPIs with very similar names, because one of them is a custom KPI. Be sure to select **Payroll Cost PL**.

-   You will see a Preview of the card, but we want to customize it before we add it to the deck.

![](./images/11a.png)

-   Click the **Customize Card** button.

![](./images/11b.png)

### **Step 12:** 

-   Note that by default, this KPI is configured as follows:
-   Target: compares against the payroll cost budget.
-   Target Value: set to % Variance from Target.

-   Now we’ll customize the KPI. Click **Show Change** checkbox.

![](./images/12a.png)

-   By default, Last Period is set to display a Qtr over Qtr comparison.

-   Click the **Last Period** value. 

![](./images/12b.png)

-   Select **Same Period Last year**.

-   The Preview updates, and we now see a new +% YoY.

![](./images/12c.png)

### **Step 13:** 

-   We can also customize the visualization itself in this KPI Card.
-   We’ll now do so by adding budget to the visualization.

-   In the **Detail Visualization** section, click **More Options** to expand it.

![](./images/13a.png)
 
-   **Scroll down** and under **Additional Data**, look for **Values**.

-   In the Values drop-down, select **Payroll Cost Budget**. We now see the budget in the visualization.

![](./images/13b.png)

-   To make the visualization easier to read,  go to the **VIsualization** box and select **Line Bar Combo**.

![](./images/13.png)

### **Step 14:** 

-   Observe how we now see actuals (blue bar) trending over budget (green line).

![](./images/14.png)

### **Step 15:** 

-   Now, click the **Conditions** link. The colored line (in this case, red) at the top of the KPI Card is an alert. The default rule is that Payroll Cost >110% is set to red (“Critical”).

-   Let’s customize the alert condition. Change the 110% value to 130% by typing in **130**%.

-   Click the **Add Card** button.

![](./images/15.png)

### **Step 16:** 

-   The KPI is now added to the deck. Payroll Cost is trending up plus over budgets. And the alert bar is showing up as yellow (“Warning”).

-   Click the **star icon** to mark as a favorite to put it on our home page.

-   Click the **maximize icon** so we can navigate to a larger card to see more information.

![](./images/16.png)

### **Step 17:** 

-   KPI Cards are designed to enable fast, immediate collaboration.

-   Click **Enter message** to create a note to the finance analyst to investigate payroll cost.

![](./images/17a.png)

-  Type the following: **Lizzy – please investigate why Payroll Cost is trending up and over budget.**

-   Click **Add Note**.

-   Notice that at the bottom of the popup window that the system recommends related metrics. In this case, the system recommends Payroll Cost Budget, Sales and Marketing, and Other Operating Expenses.

![](./images/17b.png)

### **Step 18:** 

-   Let's continue with our collaboration example. 

-   Click the **camera icon** to attach a snapshot image of the KPI card to the note you sent to Lizzy

-   Click the **back arrow** next to the Notes title.

![](./images/18.png)

### **Step 19:** 

-   Now let’s fast forward. Our business analyst, Lizzy, has completed additional analysis on this issue. She can easily share it back with us by attaching it right to the KPI. Let’s take a look at her analysis.

-   Click on the **HR Payroll and Attrition Analysis link**.

![](./images/19.png)

### **Step 20:** 

-   Our financial analyst created a detailed analysis based on both financial as well as HR workforce attrition data.
-   Review the analyst’s note: Lizzy observes that overtime pay started to increase in July, which was the same time the Call Center had a spike in attrition. You can see the spike in the lower left visualization.

-   Two additional items stand out:
-   Statistical trending and forecasting capabilities enhance several visualizations, including the projected attrition trend as well as the future impact of overtime.
-   Observe the Turnover narrative on the right was created using point and click natural language generation capabilities applied to the “Turnover by Department” visualization.

![](./images/20.png)

### **Step 21:** 

-   Let's return to the home page. 

-   Click the **Back arrow** in the upper left.

![](./images/21a.png)

-   Click **My P&L** deck.

![](./images/21b.png)

-   To recap, in this part, you:
-   Monitored business performance with pre-built KPIs and pre-built Decks
-   Drilled into deeper analysis, which is available through pre-built reports
-   Collaborated with the team – within the platform – to answer questions
-   Observed how an analyst can easily bring additional data sets – like HR data – into the platform to perform cross- functional analysis.


## Part 2. Custom Analysis on Pre-Built Profitability Subject Area

-    Oracle Analytics for Fusion ERP is designed to provide finance teams with the best of both worlds – fast, accurate, access to the latest data from your system of record, along with easy self-service analysis and customization.
-   Let's do some more exploration. Here we will introduce you to the out of the box GL profitability analysis and subject area and show you how to customize and extend to create new analysis and reports.

### **Step 1:** 

-   Starting from the My P&L deck, we’re going to drill into the out of the box Net Income Analysis.

-   Click the **Net Income KPI** card **hamburger menu icon**.

![](./images/2-1a.png)

-   Select **Net Income Analysis**

![](./images/2-1b.png)

### **Step 2:** 

-   Observe the following: 
-   Net Income for the current quarter in a waterfall viz
-   A quarterly trend for net Income, Revenue and Net Income Margin %
-   Net income details.

-   Click the **Edit button** so we can customize this analysis

![](./images/2-2.png)

### **Step 3:** 

-   Let’s take a moment to tour the self-service project.
-   On the canvas are our four familiar visualizations. Click to highlight one.

-   Observe the grammar pane on the immediate left – it is the control panel for each visualization, allowing you to modify the visualization as needed.
-   Observe the data pane on the far left. Oracle Analytics for Fusion ERP contains a pre-built data pipeline that directly imports your ERP Cloud data, as well as a pre-built data model.
-    From this data pane, you can see views of your finance data organized into constructs called subject areas. Here, we see the Financial – GL Profitability subject area. It is organized into folders containing attributes and metrics.
-    Observe at the bottom left, you see the setting pane for whatever object we select.

![](./images/2-3.png)

### **Step 4:** 

-   Now we’ll build a few visualizations with the pre-built data in this subject area.

-   Click the **+ icon** at the bottom of the screen to create a new canvas.

-   To build our first visualization, let's make a simple pivot table. In the **Data pane**, do the following:
-   Click to open the **Time** folder
-   Right Click **Fiscal Quarter**
-   Select **Pick Visualization** from the popup window
-   Select the **Pivot icon**

![](./images/2-4a.png)

-   **Drag** the **Data pane** wider so you can see better.

-   Click the **Balancing Segment Hierarchy** folder to open.

-   Double Click **Balancing Segment Level 30 Description**.

-   Scroll down the **data pane**.

![](./images/2-4b.png)

-   Click **Facts – Ledger Currency folder** to open.

-   Click **Profit and Loss (LC)** subfolder to open.

-   Double Click **Net Income**.

-   And it’s as simple as that to create your first visualization – slicing and dicing net income by different dimensions.

![](./images/2-4c.png)

### **Step 5:** 

-   We’ll create a second visualization by duplicating this pivot table.

-   On the upper right of the pivot table visualization, click the hamburger menu icon

-   Hover over **Edit**

-   Click on Duplicate Visualization to add a duplicate to the canvas.

![](./images/2-5.png)

### **Step 6:** 

-   Select the right pivot table visualization if not selected already

-   Click the **Visualization Type icon**.

-   Select **Area icon** from the dropdown list.

![](./images/2-6.png)

### **Step 7:** 

-   Your new “Area” visualization will now look like this. You can see that the combination of the table and the visualization helps tell the story more clearly.
-   **Note**: If your new visualization looks different from what is shown, double-check the fields on the grammar pane and adjust it as necessary.

![](./images/2-7.png)

### **Step 8:** 

-   We’ll now further customize this visualization by adding data labels.

-   With **# Net Income selected**, scroll down to the bottom left settings panel.

-   Click on the **#** menu, and make the following modifications:
-   Data Label: Select **Auto**
-   Font: Select **Auto** and click the **bold icon**
-   Number Format: Select **Number**
-   Decimal: Select **None**
-   Abbreviate: Select **On**

![](./images/2-8.png)

### **Step 9:** 

-   Now your visualization is much more readable with the data values. Let’s create another visualization.

-   On the upper right of the area visualization, click the **hamburger menu icon**

-   Hover over **Edit**

-   Click on **Duplicate Visualization**

![](./images/2-9.png)

### **Step 10:** 

-   Let's reorganize the visualizations on the canvas.

-   Click on one of the area visualizations and drag it above the pivot table. Watch for the blue bar to show before releasing your mouse.

![](./images/2-10.png)

### **Step 11:** 

-   Select the visualization you just dragged to the top (the visualization will be outlined in blue when it is selected).

-   In the grammar pane on the left, remove **Fiscal Quarter** by clicking the **x**.

![](./images/2-11.png)

### **Step 12:** 

-   Let's change the visualization type.

-   In the grammar pane on the left, click **Area**.

-   Select **Donut** from the dropdown list.

![](./images/2-12.png)

### **Step 13:** 

-   Scroll up the Data pane. 

-   Open the **Time** folder.

-   Click and drag **Fiscal Year** to the **Trellis Columns** area in the grammar pane.

![](./images/2-13.png)

### **Step 14:** 

-   The visualization now compares net income by regional segments across fiscal years.

![](./images/2-14.png)

### **Step 15:** 

-   We’ll next create a text narrative description of the area visualization. First let’s duplicate the area visualization. 

-   On the Upper right of the Area visualization, click the **hamburger menu icon**

-   Hover over **Edit**

-   Click **Duplicate Visualization** to add a duplicate to the canvas.

![](./images/2-15.png)

### **Step 16:** 

-   Select the new duplicate Area visualization if not selected already

-   Click the **Visualization Type** icon.

-   Select **Language Narrative icon** from the dropdown list.

![](./images/2-16.png)

### **Step 17:** 

-  A generated narrative describing the Area visualization will appear on the left.

![](./images/2-17.png)


## Part 3. Explore Balance Sheet Subject Area and Create Trial Balance

### **Step 1:** 

-   At the bottom of your screen, click the **+** icon to create a new canvas.

![](./images/3-1.png)

### **Step 2:** 

-   We are going to build a visualization using the Financial – Balance Sheet subject area.

-   Click the **Financials – GL Profitability** to collapse it.

-   Click **Financials – GL Balance Sheet** to expand it.

![](./images/3-2.png)

### **Step 3:** 

-   In the data pane, click the **Facts – Ledger Currency** folder to open it.

-   Click the **GL Balance (LC)** subfolder to open it.

-   Select the following while holding the ctrl key (cmd key for mac users)
-   **# Activity Amount**
-   **# Opening Amount**
-   **# Closing Amount**
-   **# Debit Amount**
-   **# Credit Amount**

-   After selecting them all, right click to then do the following:
-   Select **Pick Visualization**
-   Select **Pivot**

![](./images/3-3.png)

### **Step 4:** 

-   Your pivot table will appear on the canvas. Let’s continue to build this pivot table.

-   In the Data pane, click **Balancing Segment Hierarchy**folder to open it

-   Double Click **Balancing Segment Level 30 Description**

![](./images/3-4.png)

### **Step 5:** 

-   Click **Natural Account Hierarchy** folder to open it.

-   Drag **Natural Account Level 30 Description** to Rows below **Balancing Segment Level 30 Name** (in the grammar pane).

![](./images/3-5a.png)

-   Drag **Natural Account Level 29 Description** to Rows below **Natural Account Level 30 Description** (in the grammar pane).

![](./images/3-5b.png)

### **Step 6:** 

-   Your trial balance report should look similarly to the image below.

-   In the upper right hand corner of the screen, click the **Save As** icon.
-   Name the project **Net Income Analysis <last name>** and click the **Save** button.

-   **Note**: If you see a generating thumbnail message, click **Skip** to ignore.

![](./images/3-6.png)


## Part 4. Explore Account Payables Project and Create New Reports

### **Step 1:** 

-   Let’s navigate to the Home page

-   Select the **hamburger menu icon** on the top left.

-   Click **Home**.

![](./images/4-1.png)

### **Step 2:** 

-   Below the Get Started banner, you will see shortcuts to pre-built analyses. 

-   Click **Projects and Reports**

-  Click **Modified** and Select **Name**

![](./images/4-2.png)

### **Step 3:** 

-   Click **AP Analysis – Lab**

![](./images/4-3.png)

### **Step 4:** 

-   This project contains analyses across two subject areas, AP Invoices and AP Balances. Visualizations include:
-   AP Balances quarterly trend.
-   Top 10 suppliers with AP Balances.
-   Trailing 12 months for AP invoice transactions.

-   Click the **+ icon** at the bottom of the screen to create a new canvas.

![](./images/4-4.png)

### **Step 5:** 

-   In the data pane:, click **Financials – AP Balances** to collapse it.

-   Click **Financials – AP Invoices** to expand it.

-   Click **Facts – Ledger Currency** folder to open it.
-   Then, double click **Invoices Amount**

-   Click **Invoice Details** folder to open it.
-   Then, click **Payment Terms** folder to open it.
-   Then, double click **Payment Terms Name**.

![](./images/4-5.png)


### **Step 6:** 

-   Your visualization should look like the following bar chart: Invoice Amount by Payment Terms. 
-   Let’s refine by supplier.

-   Click **Supplier** folder to open it

-   Then, double click **Supplier Name** to automatically add it to your visualization.

![](./images/4-6.png)

### **Step 7:** 

-   In the grammar pane, click **Auto Visualization (Bar)**

-   Select the **Stacked bar icon** from the dropdown list

![](./images/4-7.png)

### **Step 8:** 

-   We’ll now zero in on our top ten suppliers.

-   In the grammar pane, drag **Invoice Amount** from
**Values** to the **Filter**.

![](./images/4-8.png)

### **Step 9:** 

-   Disregard the pop-up window, and instead, at the bottom of the grammar pane, in Filters, click **Invoice Amount**

![](./images/4-9a.png)

-   Hover over **Filter Type**

-   Click **Top Bottom N**

![](./images/4-9b.png)

### **Step 10:** 

-   A popup window will appear with a default set to 10, which we will accept.

-   Click anywhere on the visualization to make the popup window disappear.

-   Now we see Invoice Amount by Payment Terms for our 10 top suppliers. We see a possible supplier candidate in the Net 30 to ask for longer payment terms.

![](./images/4-10.png)

### **Step 11:** 

-   Let’s create another visualization. But this time, we’ll try out one of the shortcut features – directly searching for attributes and metrics that we are already familiar with.
-   In the data pane, click the **magnifying glass icon**

![](./images/4-11.png)

### **Step 12:** 

-   In the search box, type **Invoices Amount**
-   Select **Invoices Amount** from **Financials – AP Invoices Facts – Ledger Currency** from the popup list

![](./images/4-12a.png)

-   Then, in the search box, type **Invoices Count**
-   Select **Invoices Count** from **Financials – AP Invoices Facts – Ledger Currency** from the popup list

![](./images/4-12b.png)

-   Finally, again in the search box, type **Invoiced Fiscal Quarter**
-   Select **Invoiced Fiscal Quarter** from **Financials – AP Invoices Date** from the popup list

![](./images/4-12c.png)

-   Then, select **Create Visual**.

![](./images/4-12d.png)

### **Step 13:** 

-   Your visualizations will look similarly to the images below. We’ll now make a series of tweaks to make them easier to read.

-   In the grammar pane, click **Area**

-   Select the **Combo icon** from the dropdown list

![](./images/4-13.png)

### **Step 14:** 

-   In the grammar pane, in the Color section, click on **# Invoices Count**

-   Drag it to the **Values (Y-Axis)** section

-   Drop it on the blue line that appears below **# Invoices Amount**

![](./images/4-14.png)

### **Step 15:** 

-   In the grammar pane, right click **# Invoices Amount**

-   Select **Bar**

![](./images/4-15.png)

### **Step 16:** 

-   In the grammar pane, right click **# Invoices Count**

-   Select **Y2 Axis**

![](./images/4-16.png)

### **Step 17:** 

-   Now we see the invoice transaction trend by quarterly. Let’s click to add a statistical forecast.

-   On the upper right of the visualization, click the **hamburger menu icon**

-   Then, hover over **Add Statistics**

-   Click **Forecast**

![](./images/4-17.png)

### **Step 18:** 

-   Your visualization should look like the following, displaying a new three quarter forecast.

![](./images/4-18.png )



## Part 5. Extend Analysis with External Data

### **Step 1:** 

-   Click the **+ icon** at the bottom of the screen to create a new canvas.

![](./images/5-1.png)

### **Step 2:** 

-   Click the **+ icon** on the top of the data pane.

-   Select **Add Data Set** in the popup window.

![](./images/5-2a.png)

-   Click the **Create Data Set** button.

![](./images/5-2b.png)

-   Click **Drop data file here** or **click to browse**.

-   Select the **dun_bradstreet_ratings.xlsx** excel file you downloaded previously.

-   Click the **Open** button.

![](./images/5-2c.png)

### **Step 3:** 

-   Observe the column definitions in the dun and bradstreet ratings file.
-   The PAYDEX score measures a business’s past payment performance essentially the credit rating.
-   The Supplier Evaluation Risk (SER) Rating helps predict the chance a supplier will become inactive or shut down in the next 12 months.

-   Click the **Add** button

![](./images/5-3.png)

### **Step 4:** 

-   Click the **Data Diagram** tab at the bottom of the window.

![](./images/5-4.png)

### **Step 5:** 

-   The system automatically joins fields with the same name.

-   Click the **blue bubble “1”** on the join line to examine how the new spreadsheet is joined to the pre-built subject area data.

-   Observe that it matched on supplier name. If there was no automatic match then you could add the match manually.

-   Click the **Cancel** button.

![](./images/5-5a.png)

-   In the upper right of the screen, click the **Visualize** link.

![](./images/5-5b.png)


### **Step 6:** 

-   Let’s create a visualization that uses data from both the subject area and the excel file.

-   In the data pane, click the **Supplier** folder to expand it
-   Double click **Supplier Name**

![](./images/5-6a.png)
 
-   Click **Facts – Ledger Currency** folder to expand it.
-   Double Click **Invoice Amount**

![](./images/5-6b.png)

-   Click **dun_broadstreet_ratings** folder to expand it.
-   Double Click **SER Rating**

![](./images/5-6c.png)

### **Step 7:** 

-   The system automatically creates a scatter chart in which each bubble represents a supplier. A SER Rating of closer to 10 indicates high risk. Let’s add PAYDEX into the scatter.

-   In the data pane, double click **PAYDEX** from the **dun_broadstreet_ratings** folder so that PAYDEX is added to the visualization as the bubble color

![](./images/5-7.png)

### **Step 8:** 

-   Let’s add Invoice count into the scatter.

-   In the data pane, double click the **Invoices Count from the Facts – Ledger Currency** folder so that **Invoices Count** is added to the visualization as the bubble size

![](./images/5-8.png)

### **Step 9:** 

-   Let’s filter for just the top 10 suppliers.

-   In the grammar pane, click on **# Invoices Amount** and drag to the **Filters** section. Disregard the popup window.

![](./images/5-9a.png)

-   In the **Filters** section of the grammar pane, click **Invoice Amount** in the filter.

![](./images/5-9b.png)

-   Hover over **Filter Type**.
-   Select **Top Bottom N**.

![](./images/5-9c.png)

### **Step 10:** 

-   A popup window appears. The default is 10, which we will accept.

-   Click anywhere on the visualization to close the popup window.

-   Your visualization should look similarly to the following image.

![](./images/5-10.png)

### **Step 11:** 

-   Let’s add data labels to the visualization.

-   At the bottom left settings panel, Click the **#** menu.

-   For the Data Label, select **Auto**

![](./images/5-11.png)

### **Step 12:** 

-   The visualization helps to identify a supplier that we may introduce some risk, and may require deeper analysis.

-   Click **Save As**.

-   Name your project **Net Income Analysis <your initials>**

-   Click the **Save** button

-   **Note**: If you see a generating thumbnail message, click **Skip** to ignore.

![](./images/5-12.png)



## Summary

-   In this lab, you explored Oracle Analytics for Applications (OAX) for Fusion ERP. You navigated the Interface and pre-built content through KPI Cards, Decks, Alerts, and Analysis. You also performed a Custom Analysis on a Pre-Built Profitability Subject Area, explored a Balance Sheet Subject Area and created a Trial Balance. Additionally, you also explored an Account Payables Project and created new reports while extending analysis with external data.

-   Congratulations on completing this additional bonus lab!


[Back to top](#introduction)