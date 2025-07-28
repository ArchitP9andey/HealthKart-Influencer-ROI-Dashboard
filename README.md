# 📊 HealthKart Influencer ROI Dashboard

This Power BI dashboard analyzes influencer marketing campaigns run by HealthKart for brands like MuscleBlaze, HKVitals, and Gritzo. It measures campaign performance, return on ad spend (ROAS), ROI, and helps identify the most effective influencers and personas.

## 🔍 Features
- Performance tracking of influencers and posts
- ROAS, ROI, Revenue per Post, Revenue per Follower metrics
- Payout model analysis (Post vs Order based)
- Filtering by platform, product, brand, gender, category
- Top/Bottom influencer visuals
- Persona insights by category/gender
- Export functionality (PDF/CSV)

## 📂 Data Sources (Simulated)
- `influencers`: ID, Name, Category, Gender, Followers, Platform
- `posts`: Influencer_ID, Platform, Date, Reach, Likes, Comments
- `tracking_data`: Campaign, Product, Orders, Revenue
- `payouts`: Basis, Rate, Orders, Total_Payout (calculated)

## 📐 Key Measures (DAX)
- `Total Revenue = SUM(tracking_data[Revenue])`
- `Total Ad Spend = SUM(payouts[Total_Payout])`
- `ROAS = DIVIDE([Total Revenue], [Total Ad Spend])`
- `ROI = DIVIDE([Total Revenue] - [Total Ad Spend], [Total Ad Spend])`
- `Revenue per Post`, `Revenue per Follower`, `Cost per Order` included

## 🛠 Tools Used
- Power BI Desktop
- DAX
- Simulated Excel datasets

## 📝 Documentation & Summary
- Full documentation included (metrics, modeling, assumptions)
- Insights Summary PDF covers key findings

## ✅ Outcomes
- Identified top-performing influencers by ROAS
- Evaluated cost-efficiency with deeper metrics
- Defined best personas for future targeting

---

Would you like me to export the documentation and README into downloadable `.pdf` or `.md` files?
