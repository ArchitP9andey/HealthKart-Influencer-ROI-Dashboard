👋 Overview
This Power BI dashboard analyzes influencer marketing campaigns for HealthKart brands (e.g., MuscleBlaze, HKVitals, Gritzo). The goal is to measure campaign performance, track payouts, and evaluate ROI and ROAS.

📁 Simulated Datasets
Influencers

Fields: ID, Name, Gender, Category, Followers, Platform

Posts

Fields: Influencer_ID, Platform, Date, Reach, Likes, Comments, Caption, URL

Tracking Data

Fields: Source, Campaign, Influencer_ID, User_ID, Product, Date, Orders, Revenue

Payouts

Fields: Influencer_ID, Basis (Post/Order), Rate, Orders, Total_Payout

📊 Features Implemented
✅ Performance KPIs
✅ Top/Bottom Influencers by ROAS/ROI
✅ Product-wise revenue breakdown
✅ Best persona detection (based on gender & category)
✅ Payout tracking
✅ Filters: Brand, Product, Influencer Category, Platform
✅ Export-ready visuals

🧠 Key Measures (DAX)
dax
Copy
Edit
ROAS = DIVIDE([Revenue], [Ad Spend])
ROI = DIVIDE([Revenue] - [Ad Spend], [Ad Spend])
Incremental ROAS = [ROAS] - [Baseline ROAS] // if defined
📌 Assumptions
Simulated data reflects realistic influencer metrics.

Ad Spend is either derived per post or per influencer.

Revenue is linked to tracking_data.

No organic traffic is considered in incremental analysis.

🚀 Tools Used
Power BI

DAX

Simulated CSV tables (merged via relationships)

🧾 Insights Summary (PDF Highlights)
This would be a 1-pager summary PDF. Here's the content to include:

Influencer Campaign Insights – HealthKart
📈 Campaign Performance
Total Revenue: ₹ 1000000

Total Ad Spend: ₹ 745000

Overall ROAS: 1.85 (approx)

ROI: 180%

🌟 Top 5 Influencers (By ROAS)
Rahul_Fit (6.2X)

Priya_HealthYT (5.9X)

Fitness_King (5.2X)


⚠️ Bottom 5 Influencers (By ROI)
These influencers generated low returns despite high payout:

@FashionGurlz: ROI = -35%

@TechTipsYT: ROI = 0.8X

🧬 Best Performing Personas
Category: Fitness Professionals (Avg ROAS: 4.5X)

Gender: Male Influencers (Avg Revenue per post: ₹25,000)

📦 Product Revenue Treemap
MuscleBlaze Whey Gold: ₹4.2L

HKVitals Omega: ₹3.1L

Gritzo Supermilk: ₹2.7L

💸 Payout Model Insights
80% influencers paid per post

Order-based payouts had higher ROI overall

Top 10 influencers accounted for 65% of total revenue

