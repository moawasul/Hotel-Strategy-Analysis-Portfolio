# Hotel Revenue Strategy & Cancellation Analysis

### Project Overview
A strategic analysis of 119,000+ hotel booking records to identify revenue leakage points and optimization opportunities. Designed to simulate the decision-making process for an OTA Strategy Analyst role.

**Tools Used:** SQL (Data Cleaning), Power BI (DAX, Data Modeling), Business Strategy.

### 📊 The Executive Dashboard
![Dashboard Screenshot]([Upload your screenshot here])

### 💡 Key Strategic Insights
1.  **High-Risk Segments:** The "Groups" market segment has a critical **60% cancellation rate**. 
    *   *Recommendation:* Implementation of non-refundable deposit policies for group blocks >10 rooms.
2.  **Seasonality Pricing:** Revenue peaks significantly in **August** ($8M+).
    *   *Recommendation:* A/B test a 10-15% ADR increase during July-August to maximize margins during high-demand windows.
3.  **Channel Risk:** Online TA bookings (Agoda/Booking.com) drive volume but have a 2x higher cancellation rate than direct bookings.

### 🛠 Technical Process
1.  **SQL Data Engineering:** 
    *   Cleaned raw CSV data, casting text fields to integers/decimals.
    *   Created `Month_Sort_Index` to fix chronological sorting issues in visualization tools.
2.  **Power BI Modeling:**
    *   Built a Star Schema model.
    *   Created DAX measures for `Cancellation Rate %` and `RevPAR`.
    *   Solved circular dependency errors using Power Query ETL steps.
