# 📂 Dataset Overview – Uber Dashboard Analytics

This document provides a **detailed overview of the dataset** used in the **Uber Analytics Dashboard** project.  
The dataset represents **ride-level transactional data** for a ride-hailing platform and is suitable for **business intelligence, analytics, and dashboarding use cases**.

---

## 📌 Dataset Description

- **Domain:** Ride-Hailing / Mobility Analytics  
- **Data Type:** Structured, transactional ride data  
- **Granularity:** One row = One ride booking  
- **File Format:** Excel / CSV  
- **Usage:** Power BI dashboard, DAX KPIs, business analysis  

The dataset captures information related to **bookings, customers, vehicles, locations, ride distances, cancellations, ratings, and payment methods**.

---

## 📊 Dataset Size

| Metric | Value |
|------|------|
| Total Records | ~150,000 rides |
| Total Columns | 19 |
| Time Coverage | Daily ride data across multiple months |
| Data Quality | Clean, minimal missing values |

---

## 🧱 Column Descriptions

### 🆔 Booking & Customer Information
| Column Name | Description |
|-----------|------------|
| `Booking ID` | Unique identifier for each ride |
| `Customer ID` | Unique identifier for each customer |
| `Vehicle Type` | Type of vehicle used for the ride (Auto, Bike, Mini, Sedan, XL) |

---

### 📅 Time Information
| Column Name | Description |
|-----------|------------|
| `Date` | Date when the ride was booked |
| `Time` | Time of ride booking |

---

### 📍 Location Details
| Column Name | Description |
|-----------|------------|
| `Pickup Location` | Starting point of the ride |
| `Drop Location` | Destination point of the ride |

---

### 🚗 Ride Metrics
| Column Name | Description |
|-----------|------------|
| `Ride Distance` | Distance traveled during the ride (in km) |
| `Booking Status` | Ride outcome (Completed, Cancelled by Customer, Cancelled by Driver, Incomplete) |

---

### ❌ Cancellation Details
| Column Name | Description |
|-----------|------------|
| `Cancelled Rides by Customer` | Indicates if ride was cancelled by customer |
| `Reason for cancelling by Customer` | Customer-side cancellation reason |
| `Cancelled Rides by Driver` | Indicates if ride was cancelled by driver |
| `Reason for cancelling by Driver` | Driver-side cancellation reason |

---

### ⭐ Ratings
| Column Name | Description |
|-----------|------------|
| `Driver Ratings` | Rating given by customer to driver |
| `Customer Rating` | Rating given by driver to customer |

*(Ratings are available only for completed rides)*

---

### 💳 Payment & Revenue
| Column Name | Description |
|-----------|------------|
| `Payment Method` | Mode of payment (UPI, Cash, Card, Wallet, etc.) |
| `Revenue` | Fare amount generated from the ride |

---

## 🔍 Data Characteristics & Observations

- Cancellation-related columns contain **null values only for non-cancelled rides** (expected behavior)
- Ratings exist **only for completed rides**
- No duplicate booking IDs
- Vehicle and location fields are **categorical and high-cardinality**
- Dataset is well-suited for **aggregation, segmentation, and KPI analysis**

---

## 🎯 How the Dataset Is Used in This Project

The dataset is used to build:

- 📊 Booking & cancellation KPIs  
- 👤 Customer behavior and retention analysis  
- 📍 Location & route-level distance insights  
- 🚘 Vehicle utilization analysis  
- 💰 Revenue efficiency and contribution metrics  
- ❌ Cancellation reason diagnostics  

All transformations are performed using **Power Query**, and KPIs are created using **DAX**.

---

## 🚧 Data Limitations

- No real-time data (static historical dataset)
- No demographic information for customers
- No driver-level identifiers beyond ratings
- No surge pricing or traffic context

---

## 📌 Suitable Use Cases

- Business Intelligence dashboards  
- Power BI portfolio projects  
- Cancellation and retention analysis  
- Route and location performance analysis  
- Mobility and transportation analytics learning  

---

## 📜 Disclaimer

This dataset is used **strictly for educational, learning, and portfolio purposes**.  
It does not represent real Uber user data.

---

## 👨‍💻 Author

Prepared and analyzed by **Manthan Jadav**  
- GitHub: https://github.com/Manthan2110  
- LinkedIn: https://www.linkedin.com/in/manthanjadav/

