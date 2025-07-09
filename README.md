# Dynamic-Pricing-for-Urban-Parking-Lots

Capstone Project of Summer Analytics 2025
hosted by Consulting & Analytics Club × Pathway

---

## Objective<br/>

This project provides:<br/>

-Dynamic pricing models<br/>

-Visualize prices across parking lots<br/>

---

## Tech Stack Used <br/>

-**Python** (Pandas, Numpy) <br/>

-**Bokeh** for visualization <br/>

-**Google Colab** for development <br/>

-**GitHub** for version control <br/>

---

## Architecture Diagram




  ---

  ## Project Architecture & Workflow <br/>


  ### 1. Data Ingestion<br/>
        Historical parking lot data (CSV) is loaded, including timestamps, occupancy, queuelength, vehicle type, traffic, and special event indicators.<br/>



  ### 2. Feature Engineering  <br/>
  Categorical features (e.g., vehicle type, traffic condition) are mapped to numeric values.<br/>
  New features (e.g., occupancy ratio, demand score) are computed for use in pricing models.<br/>

  ### 3. Pricing Models<br/>
####      Model 1: Baseline Linear Pricing<br/>
  Calculates price as a linear function of occupancy ratio, bounded between minimum and maximum values.<br/>

####      Model 2: Demand-Based Pricing<br/>
   Computes a weighted sum of features (occupancy, queue, traffic, special day, vehicle type), normalizes demand, and sets price accordingly.<br/>

  ### 4. Real-Time Processing<br/>
   As each new data point arrives, the selected pricing model processes it instantly,producing a new price for the relevant parking lot.< br / >


  ### 5. Visualization<br/>
   Bokeh is used to create real-time, interactive plots:<br/>
   Price vs. time for each lot and model<br/>
   Visualizations are embedded in the notebook for transparency and justification.<br/>

The notebook includes markdown explanations, assumptions, and model justifications for clarity and reproducibility.<br/>

---

## Author :
### Snehal Choudhary

  

