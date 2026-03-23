# 📊 Logistics & Supply Chain Analysis Dashboard

## 📌 Project Overview

This Power BI project analyzes logistics and supply chain performance
focusing on delivery efficiency, delays, and cost optimization. The
dashboard provides actionable insights to improve operational
performance and decision-making.

------------------------------------------------------------------------

## 🎯 Objectives

-   Analyze delivery performance across regions and cities\
-   Identify delayed shipments and their patterns\
-   Monitor average delivery time\
-   Track overall delivery costs

------------------------------------------------------------------------

## 📂 Dataset Description

The dataset contains shipment-level data with the following fields:

-   ShipmentID -- Unique shipment identifier\
-   OrderDate -- Order placed date\
-   DeliveryDate -- Actual delivery date\
-   ExpectedDate -- Expected delivery date\
-   OriginCity -- Shipment origin\
-   DestinationCity -- Shipment destination\
-   Region -- Delivery region (North, South, East, West)\
-   Distance_km -- Distance covered\
-   Cost_USD -- Delivery cost\
-   DeliveryStatus -- On-time / Delayed / Cancelled\
-   DeliveryTime_Days -- Delivery duration

------------------------------------------------------------------------

## 📊 Key Performance Indicators (KPIs)

-   📦 Total Shipments: 300\
-   💰 Total Cost: 322.98K\
-   ⏱ On-Time Delivery %: 0.47\
-   🚚 Avg Delivery Time: 5.63 days

------------------------------------------------------------------------

## 📈 Dashboard Features

### 🔹 KPI Cards

Displays key metrics for quick insights: - Total Shipments\
- Total Cost\
- On-Time %\
- Average Delivery Time

### 🔹 Line Chart

-   Shows monthly trends of shipments and delivery time

### 🔹 Bar Chart

-   Displays average delivery time by region

### 🔹 Donut Chart

-   Shows shipment distribution by delivery status

### 🔹 Heatmap (Matrix)

-   City-to-city shipment performance analysis

### 🔹 Table with Conditional Formatting

-   Highlights delayed shipments (\>2 days) in red\
-   On-time shipments in green

------------------------------------------------------------------------

## 🧮 DAX Measures

**Total Shipments**

    COUNT(ShipmentID)

**On-Time Delivery %**

    DIVIDE(
        CALCULATE(COUNT(ShipmentID), DeliveryStatus = "On-time"),
        COUNT(ShipmentID)
    )

**Average Delivery Time**

    AVERAGE(DeliveryTime_Days)

**Total Cost**

    SUM(Cost_USD)

------------------------------------------------------------------------

## 🎛 Filters (Slicers)

-   Order Date\
-   Delivery Status\
-   Region

------------------------------------------------------------------------

## 💡 Key Insights

-   East region shows relatively higher delays\
-   Some routes consistently experience delivery delays\
-   On-time delivery rate is below optimal levels\
-   High-cost shipments are linked with longer distances

------------------------------------------------------------------------

## 🚀 Conclusion

The dashboard helps stakeholders identify inefficiencies in delivery
operations and take data-driven actions to improve logistics
performance, reduce delays, and optimize costs.

------------------------------------------------------------------------

## 📁 Deliverables

-   Power BI Dashboard (.pbix)\
-   DAX Measures\
-   Insights Report
