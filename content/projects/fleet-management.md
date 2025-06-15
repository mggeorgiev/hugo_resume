---
title: "FLEET MANAGEMENT"
date: 2021-01-21T23:47:48+03:00
draft: false
description: "Manage effectively and efficiently vehicle fleets."
about:
  - "Managing a vehicle is a common experience for most owners, unless they have hired someone to handle it on their behalf. Some even enjoy it, despite the fact that most tasks are mundane. Expanding to a fleet introduces additional overhead."
  - "The application logs both refueling and maintenance, leveraging statistics to identify trends, outliers, and recommend actions based on historical data. It also predicts future expenses and reminds users of upcoming activities based on flexible business logic. Maintenance requires approval before being archived."

motivation:
  - "Automating the operation enables repetitive processes, good practices, and the collection of data for business intelligence and data mining."
  - "The application started as a Google Sheets file. In its current form, it allows for the management of multiple vehicles, providing statistical insights and visualizations."
  - "![Fleet management version 1](../../img/fleet_management/sheet-01.png)"
  - "*Refueling log*"
  - "![Fleet management version 1](../../img/fleet_management/sheet-02.png)"
  - "*Maintenance log*"
  - "As interest in the product increased, I realized that platform shortcomings were limiting usability. Each new customer required a separate version of the application, and aggregating information from multiple files created overhead."
  - "Although Google Sheets is available in a mobile version, the experience differs significantly from the desktop version."
challenges: 
  - "The **first** challenge was to build a data layer that could be used for statistical analysis of data."
  - "The **second** challenge was to be able to apply statistical analysis on the whole dataset while retaining each user's data private."
  - "The **third** challenge was to allow secure usage from multiple users on desktops and mobile devices."
  - "The **fourth** challenge was to use architecture and design that allow changes."
approach:
  - "Considering the nature of the application - a database one, I decided to use the Oracle 11g XE that comes with a preinstalled APEX and a web server, that unfortunately requires a license to use SSL."
  - "To use SSL I deployed an Apache running on Ubuntu server 16.04, that acts as a reverse proxy and SSL offloader. The certificate was obtained from Let's Encrypt."
  - "Power BI report [📄](../../files/FLEET-MANAGEMENT-PBI.pdf) is available and could be updated from a reporting server, while the later is feed from the application database."
markdown_title: "Reports and Graphs"
markdown:
  - "**The predefined reports include**:"
  - "Vehicle"
  - "Total cost of ownership ![Total cost of ownership](../../img/fleet_management/tco.png) <br> *The report shows the mileage, fuel amount consumed, fuel and maintenance cost, and the total cost of ownership (TCO), TCO per kilometer per each car in the fleet*."
  - "Refueling log ![Refueling log](../../img/fleet_management/refuel_log.png) <br> 
  *Log of all refueling events. Enrich them with categorical attributes to enable filtering by vehicle, date attributes, periods between events*."
  - "Maintenance log ![Maintenance log](../../img/fleet_management/maintenance_log.png) <br>
  *Log of all maintenance events enriched with periods (date and mileage). Enable filtering by vehicle, date attributes, type, and periods between events*."
  - "Statistics per fuel brand ![Statistics per fuel brand](../../img/fleet_management/stat_suppliers.png)"
  - "Statistics per drive type ![Statistics per drive type](../../img/fleet_management/stat_drivetype.png)"
  - "**Graphical visualization shows**:"
  - "Histograms ![Histograms](../../img/fleet_management/fuel_amount.png) <br> 
 *Histograms to illustrate the frequency of distribution for **Fuel price**, **Fuel Amount**, and **Mileage**.*"
  - "Fuel prices ![Fuel prices](../../img/fleet_management/fuel_prices.png) <br> 
 ***Fuel price**, **range**, **min/max**, and **average**.*"
  - "Fuel expences ![Fuel expences](../../img/fleet_management/fuel_expences.png) <br> 
 *Comparison of expenses per year, for the last 12 months, including range.*"
  - "Mileage ![Mileage](../../img/fleet_management/mileage.png) <br> 
 *Various comparisons for mileage per months (consequtive), quarter, and year inclding standard deviation.*"
  - "**Predictions**:"
  - "Predictions suggest actions:"
  - "- **Refueling prediction** ![Refueling prediction](../../img/fleet_management/refueling_predictions.png) <br> Uses historical data to predict next refueling date, and expected mileage reading based on all records or a subset of the last 12 months."
  - "- **Maintenace prediction** ![Maintenace prediction](../../img/fleet_management/maintenance_prediction.png) <br> Predicts the next maintenance execution based on the averages for the particular item. The results are sorted by frequency of occurrences."
  - "- **Maintenace classification** ![Maintenace classification](../../img/fleet_management/maintenance_prediction.png) <br> Historical quarterly aggregation of maintenance expenses per type and vehicle."
---


