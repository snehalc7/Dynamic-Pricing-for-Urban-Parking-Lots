# Dynamic-Pricing-for-Urban-Parking-Lots

Capstone Project of Summer Analytics 2025
hosted by Consulting & Analytics Club × Pathway

---

## Objective

This project provides:

-Dynamic pricing models 
-Visualize prices across parking lots

---

## Tech Stack Used

-**Python** (Pandas, Numpy)
-**Bokeh** for visualization
-**Google Colab** for development
-**GitHub** for version control

---

## Architecture Diagram

graph TD
    A[CSV Dataset] --> B[Pathway Data Stream]
    B --> C[Feature Engineering & Preprocessing]
    C --> D1[Model 1: Linear Pricing]
    C --> D2[Model 2: Demand-Based Pricing]
    D1 --> E[Pricing Output]
    D2 --> E
    E --> F[Real-Time Bokeh Visualization]


  ---

  ## Project Architecture & Workflow


  ###1. Data Ingestion
        Historical parking lot data (CSV) is loaded, including timestamps, occupancy, queue            length, vehicle type, traffic, and special event indicators.



  ###2. Feature Engineering
        Categorical features (e.g., vehicle type, traffic condition) are mapped to numeric             values.
     New features (e.g., occupancy ratio, demand score) are computed for use in pricing models.

  ###3. Pricing Models
####      Model 1: Baseline Linear Pricing
          Calculates price as a linear function of occupancy ratio, bounded between minimum              and maximum values.

####      Model 2: Demand-Based Pricing
          Computes a weighted sum of features (occupancy, queue, traffic, special day, vehicle           type), normalizes demand, and sets price accordingly.


  ###4. Real-Time Processing
        As each new data point arrives, the selected pricing model processes it instantly,             producing a new price for the relevant parking lot.


  ###5. Visualization
        Bokeh is used to create real-time, interactive plots:
        Price vs. time for each lot and model
        Visualizations are embedded in the notebook for transparency and justification.

The notebook includes markdown explanations, assumptions, and model justifications for clarity and reproducibility.

  

