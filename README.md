# YouTube Analytics Power BI Dashboard

## Overview
This Power BI dashboard is designed to help YouTube creators and businesses make sense of their channel data. By consolidating critical metrics—revenue, watch time, engagement, and audience demographics—into one intuitive interface, it streamlines decision-making and pinpoints strategic growth areas.

## How This Tracker Helps
- **Identify Top Content**: Quickly see which videos or months drive the most engagement and revenue.  
- **Optimize Revenue Streams**: Discover which ads or monetization methods generate the largest return.  
- **Segment Audiences**: Break down performance by age groups, demographics, and genre to tailor content.  
- **Monitor Trends Over Time**: Visualize how watch time, views, and engagement evolve across different periods.  

---

## Dashboards

### 1. Revenue and Performance Dashboard


<img width="1192" alt="Screenshot 2025-02-19 at 6 45 55 PM" src="https://github.com/user-attachments/assets/07c295a0-7bed-408e-a48a-30796d32e076" />


### 2. Target Audience Analysis


<img width="1165" alt="Screenshot 2025-02-19 at 6 46 10 PM" src="https://github.com/user-attachments/assets/01502766-d600-4ebd-ab73-03ab36789962" />


### 3. Genre Distribution


<img width="1170" alt="Screenshot 2025-02-19 at 6 46 26 PM" src="https://github.com/user-attachments/assets/53ce8670-b7e7-4c39-8fe1-eee219c389ae" />

---

## Full Report

### 1. Research Statement
YouTube creators and businesses face significant challenges in effectively analyzing their data to gain actionable insights. With massive volumes of video performance metrics, audience demographics, and engagement statistics, it becomes overwhelming to identify patterns or pinpoint key opportunities for growth. This complexity often leads to difficulty in allocating resources effectively—such as deciding which type of content to produce for specific demographics or identifying the pain points that hinder channel growth. Without clear insights, creators risk missing out on optimizing their strategy, reducing engagement, and limiting their potential for revenue growth.

### 2. Proposed Solution
To address these challenges, this **YouTube Analytics Dashboard** provides a clear, actionable overview of performance metrics. It consolidates key data points—such as revenue, watch time, engagement, and audience demographics—to give both high-level and granular views of channel statistics.

**Key features include**:
- **Revenue Insights**: Total revenue, earnings breakdown, and primary revenue sources.  
- **Watch Time & Engagement**: Displays watch time, views, and subscriber growth.  
- **Revenue Forecasting**: Expected vs. actual revenue over different periods.  
- **Performance Trends**: Highlights top-performing months and content success patterns.  
- **Like/Dislike Ratios**: Quick view of audience sentiment and content reception.  
- **Target Audience Analysis**: Focus on demographic data to optimize targeting efforts.

---

### 3. Methodology

#### 3.1 Datasets Explained

1. **YouTube Channel Performance Analytics**  
   - **Link**: [Kaggle: YouTube Channel Performance Analytics](https://www.kaggle.com/datasets/positivealexey/youtube-channel-performance-analytics)  
   - **Features**: ~70 columns covering video metadata, time metrics, revenue metrics, engagement metrics, playback/impressions, viewer metrics, etc.

2. **Genre Metadata**  
   - Synthetic dataset generated for visualization (e.g., genre, classification, etc.).

3. **Target Audience Data**  
   - Another synthetic dataset (demographics, preferences, etc.).

#### 3.2 Data Cleaning and Importing
- **YouTube Channel Analytics**:  
  - Loaded into Power Query Editor.  
  - Cleaned null rows/columns, changed data types, split date/time fields, etc.
- **Target Audience Dataset**:  
  - Removed unwanted rows from RTF file conversion and null values.
- **Video Tags Dataset**:  
  - Minimal cleaning needed besides default Power Query transformations.

#### 3.3 Relationships
- Created **one-to-one** relationships by linking the `ID` field from the YouTube analytics dataset to the target audience and video tags datasets.

#### 3.4 Colour Theory
A duo-tone style blends:
- **Red (#C80000)**: Background & highlights (ties to YouTube branding).  
- **Dark Grey (#252525)**: Chart backgrounds for neutral contrast.  
- **Light Grey (#C0C0C0)**: Gridlines and axis labels.  
- **White (#FFFFFF)**: Primary text for readability.  
- **Teal/Cyan (#00E6E6), Orange (#FFA500), Pink (#FF91A4), Blue (#00A2E8)**: Accent colors for key data points and differentiation.

#### 3.5 User Experience
The dashboards split into three main sections:
1. **Main Dashboard** (High-Level Overview): Core KPIs, top-performing months, sentiment analysis, revenue breakdown.  
2. **Target Audience Dashboard**: Demographic-focused, segment-level revenue, and long-term performance patterns.  
3. **Genre Distribution Dashboard**: Genre-based performance insights, revenue breakdown, impressions, and engagement metrics.

#### 3.6 Charts Breakdown

##### 3.6.1 Overall Performance Page
1. **Key Metrics Summary**: Cards for total videos, subscribers, views, and watch hours.  
2. **Expected vs. Actual Revenue (with Watch-Time)**: Combined bar/line chart to correlate watch time with revenue spikes.  
3. **Top Performing Months**: Horizontal bar chart sorted by like rate, indicating high-engagement periods.  
4. **Like/Dislike Ratio**: Donut chart showing ~97.81% likes vs. 2.19% dislikes.  
5. **Subscriber Growth vs. Unsubscribes**: Another donut chart indicating 92.37% new subs vs. 7.63% unsubscribes.  
6. **Revenue Breakdown**: Pie chart detailing how revenue is split among various sources (e.g., YouTube Ads at 61.54%, Watch Page Ads at 33.84%).

##### 3.6.2 Target Audience Page
1. **TA-Based Line Graphs**: Plots revenue over time for adults, kids, and teens.  
2. **Average Revenue per 1000 Views**: Pie chart proportioning revenue from each audience segment.  
3. **Total Revenue Generated per TA**: Bar chart comparing total revenue across segments.

##### 3.6.3 Genre Dashboard
1. **Views Growth by Genre**: Line graph capturing trends for Gaming, Movie, Entertainment, Education, and TV.  
2. **Total Revenue by Genre**: Treemap for quick visual comparison (Gaming leads).  
3. **Impressions by Genre**: Horizontal bar chart illustrating reach/impressions for each genre.

---

### 4. Business Application and Insights

#### 4.1 Overall Channel’s Performance
- **Core KPIs**: Strong watch time and subscriber base indicate healthy channel engagement.  
- **Watch Time ↔ Revenue Correlation**: Higher watch time often yields increased revenue.  
- **Seasonal Trends**: Some months (e.g., June/November) stand out for higher engagement.  
- **Positive Sentiment**: A like ratio above 97% signals content approval.  
- **Diversify Revenue**: YouTube ads dominate, but exploring additional monetization could further boost earnings.

#### 4.2 Target Audience Based Performance
- **Teens**: Highest total revenue—valuable audience segment to focus on.  
- **Adults**: Highest revenue per 1000 views, indicating more profitable impressions.  
- **Kids**: Growing upward trend; potential new frontier for content.  
- **Targeted Strategies**: Tailor release schedules and promotions per demographic to maximize returns.

#### 4.3 Genre Based Performance
- **Gaming**: Leads in revenue and impressions; strong potential for partnerships and brand deals.  
- **Movies & Entertainment**: High revenue despite a viewership decline—ripe for content re-strategizing.  
- **Education & TV**: Smaller share, but still potential niches.  
- **Balanced Approach**: Continue leveraging top genres while investing in emerging or underperforming ones for broader reach.
