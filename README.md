# **Stat 436 HW2 – Wildfire Visualization Project**

## **Dataset Description**
The dataset used in this project is the **US Wildfire Dataset (2014–2025)** — *9.5 million spatiotemporal wildfire records (GRIDMET + IRWIN)* — sourced from Kaggle, created by **Shaurya Mathu, Shreyas Bellary Manjunath, and Alina Vereshchaka**.  
It contains detailed wildfire event information across the **continental United States**.

---

## **Data Cleaning**
To focus on real-world wildfire events, I filtered and retained **502,000 valid events**.  
After confirming that the dataset contained **no missing values**, I performed several preprocessing steps:

- Extracted **year**, **month**, and **season** from the time variable  
- Derived **state** using latitude and longitude  
- Verified spatial and temporal consistency  
- Finalized key variables:
  - **Season**
  - **Year**
  - **State**
  - **Latitude / Longitude**
  - **Solar Radiation (W/m²)**

Each row represents a real wildfire event recorded between **2014 and 2025**, including location, time, and environmental features.

---

## **Main Question**
This visualization explores the question:

> **How do wildfire patterns relate to solar radiation, seasonality, and geographic region across the United States?**

The intended audience includes:

- *Climatologists*  
- *Environmental policy researchers*  
- *Conservationists*  
- *General public interested in wildfire trends*

---

## **Interactive Elements**
The dashboard contains **two main pages**:  
### **1. Overview**
- Filters: **Season** (dropdown) and **Solar Radiation** (slider)  
- A national wildfire **map** showing spatial patterns  
- A **year histogram** (2014–2025) with brushing:
  - X-axis: years  
  - Y-axis: wildfire counts  
  - Brushing dynamically updates the map  
- Helps users see *both temporal trends and spatial distribution*

### **2. State Explorer**
- Users can select a **specific state**  
- The right panel displays:
  - A **state-level map**
  - Filtered wildfire events  
- Supports filtering by:
  - **Season**
  - **Solar Radiation**
- Useful for understanding localized patterns and regional climate effects

### **Why these variables?**
- **Year** → reveals long-term wildfire trends  
- **Season** → summarizes climate characteristics without overwhelming the interface  
- **State** → captures strong regional climate differences  
- **Solar Radiation** → a periodic variable that interacts strongly with time and space, helping reveal environmental drivers of wildfire activity  

---

## **Style & Layout**
The visualization follows a **clean and intuitive design**:

- **White background**, with black/green text accents  
- Green highlights to distinguish the two pages  
- Sliders and histograms follow a **consistent blue color scheme**  
- Maps have a **light gray background**  
- Wildfire points use a **yellow → red gradient** based on solar radiation:
  - Matches wildfire color themes  
  - Enhances visual hierarchy  
  - Improves readability and interpretability  

---

## **Unexpected Findings**
- Wildfire counts have **steadily increased** from 2014–2024 (2025 incomplete).  
- Besides California, **Florida** shows surprisingly high wildfire activity:
  - Especially during winter  
  - Florida is the **only state** with winter fires under **solar radiation > 250 W/m²**  
- Wildfires can still occur when **solar radiation < 5 W/m²**, suggesting other drivers.  
- In **Wisconsin**, wildfire peaks in **spring**, followed by winter — *not summer* —  
  indicating that **humidity may be a major contributing factor**, not just solar radiation.

---











