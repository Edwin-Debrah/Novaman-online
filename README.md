
# Project Background
Novaman online is a global e-commerce company that specialize in sale of electronics, gaming products, and lifestyle technology since it's establishment in 2018.

The company keeps data of sales over time, purchase and shipping dates, marketing channels and regions where these revenues are coming from, which have been underutilized for sometime now. This project is to uncover insights that will help drive business ideas

Insights and recommendations are provided on the following key areas:

- **Revenue trends:** evaluation of revenue trends across years and months, by region and also marketing channels
- **Product performace:** which products drove the most sales, and influenced sales trends the most
- **Marketing channels effectiveness:** analysis on the most effective marketing channels
- **Region contribution:** which region had the most sales during the years under review

The tables and pivot tables used for the analysis [link].

An interactive Power BI dashboard used to report and explore sales trends can be found here [link].



# Data Structure & Initial Checks

Novaman online main database structure as seen below consists of two tables: orders and region, with a total row count of 22,056 records. A description of each table is as follows:

<img width="1001" height="449" alt="ERD" src="https://github.com/user-attachments/assets/478cfce9-5660-4b0d-9502-2ee1cb52e8e7" />


# Executive Summary

### Overview of Findings

The analysis showed that 2020 was Novaman online's peak revenue year, mainly driven by pandemic-related demand and also cultural and lifestyle, with sales surging in September  and December 2020 before declining in early 2021 as markets normalized post pandemic. Playstation 5, Nintendo Switch and 27in gaming monitors were the main revenue drivers, particularly through direct website purchases. Finally, North America was the most influencial region, considering their long established culture in gaming among most youth, mirroring overall company revenue trends and reinforcing its importance for future product and marketing startegies.

<img width="1100" height="607" alt="Overview" src="https://github.com/user-attachments/assets/5659de6f-026f-46a0-8af0-a67a5abf6332" />


# Insights Deep Dive
### Revenue trends:

* Pandemic Surge (2020): Total sales more than doubled during the pandemic, rising from $1.5M in 2019 to $4M in 2020. The peak months were September ($456,871, 1,496 units) and December ($549,435, 1,671 units). For comparison, the previous monthly high was $180,769 in December 2019.

* Post-Pandemic Decline (2021): Sales began falling in early 2021 due to supply chain shortages, the fade of pandemic-driven demand, and economic pressures such as tighter budgets, uncertainty, and shifting consumer behavior as restrictions eased and people spent more time outside.

* Price & Demand Shift: For top products like the 27in Gaming Monitor, the average price rose from $426 (Sept 2020) to $432 (Jan 2021). This price increase, driven by higher supply costs or strong holiday demand which is evident in Sep 2019 to Jan 2020 also , coincided with a drop in unit sales from 326 (Sep 2020) to 207 (Jan 2021).
  
<img width="1136" height="637" alt="Revenue" src="https://github.com/user-attachments/assets/b4ff6f29-9869-472d-9bfd-da580ff4e377" />

### Product performance:

* Top Products Driving Revenue: The three best performers were the 27in Gaming Monitor ($1.9M, 4,723 units), Nintendo Switch ($1.6M, 10,386 units), and Sony PlayStation 5 ($1.5M, 977 units). Other products had minimal impact on overall trends, except Lenovo laptops, which followed a similar pattern as the top 3 best performing products and also the total revenue trend but at lower revenue levels.

* Pandemic Demand Concentration: Sales growth was concentrated in gaming consoles (PS5, Nintendo Switch) as stay-at-home lifestyles boosted demand.

* Broader Use Cases: Gaming monitors also performed strongly, benefiting not only from gaming but also from remote work and online learning. This explains why Lenovo laptops ranked 4th in performance.

* Revenue Sensitivity: Since these top products drove most of total revenue, any fluctuation in their sales directly impacted overall performance. All peaked in September–December 2020 and declined in early 2021, contributing to the overall sales slowdown.
  
<img width="1124" height="625" alt="Product" src="https://github.com/user-attachments/assets/d7248276-efd2-4a0f-b132-0c7047013282" />


### Marketing channel effectiveness:

* Dominant Marketing Channel: Direct website purchases were the most effective channel, accounting for 84.7% of total revenue. Their performance mirrored overall sales trends, peaking in September and December 2020, then declining in early 2021.

* Consumer Behavior Shift: Heavy reliance on direct purchases was driven by stock shortages and scalper scams during lockdowns, making consumers trust official websites over ads, email, or social media promotions.

* Secondary Channel: Email marketing ranked second with 9.94% of total revenue, but it had little influence on sales trends. All other channels remained flat with no significant impact during peaks or declines.

  <img width="1126" height="619" alt="Marketing" src="https://github.com/user-attachments/assets/1567515d-2c73-432f-a03b-dfd5175e629f" />

### Region Contribution:

* Regional Leader: North America (NA) was the top revenue contributor with $3.2M, followed by the Middle East & Asia ($1.8M).

* Purchasing Power: Higher household spending in the U.S. and Canada was fueled by government stimulus checks during the pandemic, boosting overall sales in the region.

* Cultural Influence: NA’s strong console and PC gaming culture and widespread remote work adoption drove demand for products like the PS5, Nintendo Switch, and gaming    monitors, making them top performers.

* Trend Alignment: Sales in NA mirrored overall trends, peaking in September and December 2020 before declining in early 2021, showing the region’s heavy influence on total revenue patterns.
[Visualization specific to category 4]

<img width="1131" height="628" alt="Region" src="https://github.com/user-attachments/assets/2cda0b43-4e94-4a2c-bbf5-664ddcbe58d7" />


# Recommendations:

Based on the insights and findings above, we would recommend the team to consider the following: 

* Stock up and strengthen supply chain resilience ahead of peak months (Sept–Dec) to avoid shortages and lost sales, also the finance team can introduce promotions, bundles, or loyalty rewards in Q1 to reduce the steep drop in sales after the holidays while also monitoring external economic indicators (inflation, consumer budgets) and adjust pricing and inventory strategies accordingly
  
* Focus resources (marketing, inventory, supplier negotiations) on high-performing items like the 27in Gaming Monitor, Nintendo Switch, and PS5 since they drive most revenue and also diversify portfolio by exploring complementary products (e.g., gaming accessories, remote work gear) to reduce over-reliance on just three core products.  

* Continue investing in direct marketing channels with smoother checkout, trust signals (anti-scalper policies, verified stock), and exclusive deals and also since email and social media had low impact, redesign campaigns to be more personalized, gamified, or bundled with loyalty perks to increase effectiveness in other marketing channels as well. 

* Maintain strong supply and marketing focus in NA, where cultural and financial factors support high demand while also Build targeted campaigns in Middle East & Asia, where revenue contribution is significant but could grow further with localized marketing and partnerships. For NA, continue prioritizing consoles and gaming monitors; for Asia/Middle East, explore laptops and mobile-friendly gaming devices, aligning with market needs.


# Assumptions and Caveats:

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

* Missing values for marketing channels so they were named null
  
* Some products didn't have USD_price so I used average price from similar products
  
* Some products was shipped before purchase dates, which I assumed to be an error so I left them as they didn't influence the goal of our analysis
