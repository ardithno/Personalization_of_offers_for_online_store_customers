# Personalization of offers for online store customers

  ## **Introduction:**

  ### *Project description:*

    We will study the data provided by the "One Click" store. 
    Using machine learning models, we will predict the level of customer activity, 
    predict the likelihood of a decrease in purchasing activity. 
    We will highlight customer segments and develop personalized offers.
  
  ### *Project goal:*

    The main goal is to develop a model for predicting customer purchasing power. 
    Develop offers to increase purchasing power.
  
  ### *Data description:*

    The market_file.csv table contains data on customer behavior on the site, communications with the customer and their product behavior. Data by columns:
      id — customer number in the corporate database.
      Purchase activity — calculated class of purchasing activity (target feature): "decreased" or "previous level".
      Service type — service level, for example "premium" and "standard".
      Allow notification — information on whether it is possible to send the buyer additional offers about the product. The buyer gives consent to this.
      Market_active_6_months — the average monthly value of the company's marketing communications that were sent to the buyer over the past 6 months. This value shows what number of mailings, calls, ad impressions, etc. were sent to the client.
      Market_active_current_months — the number of marketing communications in the current month.
      Duration — a value that shows how many days have passed since the buyer registered on the site.
      Promotional_purchases — the average monthly share of purchases on promotion from the total number of purchases over the past 6 months.
      Popular_category — the most popular category of goods with the buyer over the past 6 months.
      Average_views_of_categories_per_visit — shows how many categories the buyer viewed on average per visit over the past month.
      Unpaid_products_pieces_quarter — the total number of unpaid items in the basket over the past 3 months.
      Service_error — the number of failures that affected the buyer during a visit to the site.
      Pages_per_visit — the average number of pages viewed by a customer during one visit to the site over the last 3 months.

    The market_money.csv table contains data on the revenue that the store receives from the customer, that is, how much the customer spent in total during the period of interaction with the site. Data by columns:
      id — customer number in the corporate database.
      Period — the name of the period during which the revenue was recorded. For example, 'current_month' or 'previous_month'.
      Revenue — the amount of revenue for the period.

    The market_time.csv table contains data on the time the customer spent on the site during the period. Data by columns:
      id — customer number in the corporate database.
      Period — the name of the period during which the total time was recorded.
      minutes — the value of time spent on the site, in minutes.

    The money.csv table contains data on the average monthly profit of the customer over the last 3 months: how much profit the store receives from sales to each customer. Column data:
      id — customer number in the corporate database.
      Profit — profit value.

### *Work plan:*

1. Data loading, general information study
2. Data preprocessing: check for abnormal values, gaps, duplicates, data types
3. Exploratory data analysis: select customers with purchasing activity for at least three months.
4. Correlation analysis: conduct a correlation analysis of features in the quantitative scale of the final table for modeling. Study multicollinearity.
5. Use of pipelines: apply all studied models using pipelines
6. Feature importance analysis: evaluate the importance of features and build an importance graph using SHAP
7. Customer segmentation: perform customer segmentation.
8. General conclusion.
