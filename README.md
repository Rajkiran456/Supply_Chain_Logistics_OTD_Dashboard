# 🚚 Supply Chain & Logistics OTD Dashboard (Power BI)

## 📌 Executive Summary
Designed and developed an end-to-end interactive Power BI dashboard to monitor On-Time Delivery (OTD %) performance, evaluate plant-level fulfillment capabilities, and analyze carrier dynamics across supply chain operations.

## 🛠️ Data Architecture & Modeling
* **Data Model:** Implemented a Star Schema connecting `OrderList` (Fact) with `Calendar` and `WhCapacities` (Dimensions).
* **DAX Formulas:** Developed robust measures using `VAR/RETURN` structures and `DIVIDE` to avoid division-by-zero errors.
  * **Total Orders:** `COUNT(OrderList[Order ID])`
  * **OTD %:** `VAR OnTime = CALCULATE(...) RETURN DIVIDE(OnTime, TotalOrders, 0)`

## 💡 Key Business Insights
* **Delivery Performance:** Overall OTD maintained at ~98% across total processed orders.
* **Plant Bottlenecks:** Plant-wise distribution highlights top-performing fulfillment centers vs. delayed nodes.
* **Carrier Dynamic:** Interactive slicer allows immediate filtering to isolate vendor delays.

## 📸 Dashboard Preview
![Dashboard Screenshot](path-to-your-screenshot.png)
