---
title: "FLEET MANAGEMENT"
date: 2021-01-21T23:47:48+03:00
draft: false
description: "Manage effectively and efficiently vehicle fleets."
about: ["Manage a vehicle is something that most owners experience (except if they have hired someone to do it on their behalf). Some even enjoy it, despite that most tasks are mundane. Adding cars to form a fleet comes with an overhead."
        ,"The application keeps log of both refueling and maintenance. Uses statistics to find trends, outrliers, recommend actions based on histoirical data and predict future expences. Also reminds for upcomming activities based on flexible business logic. Maintenance requires approval prior to archiving."]
motivation: 
        ["Automating the operation allows the usage of repetitive processes, good practices, and the collection of data that can be used for business inteligence or data mining."
        ,"The application started as a Google sheets file. In this incarnation, it allows the management of multiple vehicles, provide statistical information, and visualizations."
        ,"As the interest in the product increased, I realized that the shortcomings in the platform limit the usability. Each new customer had to have its own version of the application and aggregating the information from multiple files results in an overhead. Although google sheets are available in a mobile version as well, the experience is very different compared with the desktop version."]
challenges: ["The first challenge was to build a data layer that could be used for statistical analysis of data."
            ,"The second challenge was to be able to apply statistical analysis on the whole dataset while retaining each user's data private."
            ,"The third challenge was to allow secure usage from multiple users on desktops and mobile devices."
            ,"The fourth challenge was to use architecture and design that allow changes."]
approach: ["Considering the nature of the application - a database one, I decided to use the Oracle 11g XE that comes with a preinstalled APEX and a web server, that unfortunately requires a license to use SSL."
            ,"To use SSL I deployed an Apache running on Ubuntu server 16.04, that acts as a reverse proxy and SSL offloader. The certificate was obtained from Let's Encrypt."
            ,"Power BI report is available and could be updated from a reporting server, while the later is feed from the application database.",]

#     <section id="about">
#         <div class="container">
#             <div class="row">
#                 <div class="col-lg-8 mx-auto">
#                     <h2>About the project</h2>
                    
#                         <br>
#                         <a href=""><i class="far fa-thumbs-up"></i></a>
#                         <a href="../files/FLEET-MANAGEMENT-PBI.pdf" target="_blank"><i class="fas fa-wave-square"></i></a>
#                         <a href="#graphs"><i class="fas fa-chart-pie"></i></a>
#                         <a href="#predictions"> <i class="fas fa-chart-line"></i></a>
#                     </p>
#                 </div>
#             </div>
#         </div>
#     </section>

#     <section id="motivation" class="bg-light">
#         <div class="container">
#             <div class="row">
#                 <div class="col-lg-8 mx-auto">
#                     <h2>Motivation</h2>
                    
#                     <p class="lead">
#                         Automating the operation allows the usage of repetitive processes, good practices, and the collection of data that can be used for business inteligence or data mining.
#                     </p>
                    
#                     <p class="lead">
#                         The application started as a Google sheets file. In this incarnation, it allows the management of multiple vehicles, provide statistical information, and visualizations.
#                     </p>
                    
#                     <p class="lead">
#                         As the interest in the product increased, I realized that the shortcomings in the platform limit the usability. Each new customer had to have its own version of the application and aggregating the information from multiple files results in an overhead. Although google sheets are available in a mobile version as well, the experience is very different compared with the desktop version.
#                     </p>
                    
#                     <p class="lead">
#                         The application started as a Google sheets file. In this incarnation, it allows the management of multiple vehicles, provide statistical information, and visualizations.
#                         <br>
#                         <img class="img-fluid mx-auto mb-2" src="../img/fleet_management/sheet-01.png" alt="Fleet management version 1">

#                         <br><i>Refueling log</i>

#                         <img class="img-fluid mx-auto mb-2" src="../img/fleet_management/sheet-02.png" alt="Fleet management version 1">
#                         <br><i>Maintenance log</i>
#                         <br>
#                         As the interest in the product increased, I realized that the shortcomings in the platform limit the usability.
#                         Each new customer had to have its own version of the application and aggregating the information from multiple files results in an overhead.
#                         Although google sheets are available in a mobile version as well, the experience is very different compared with the desktop version.
#                     </p>
#                 </div>
#             </div>
#         </div>
#     </section>

#     <section id="challenges">
#         <div class="container">
#             <div class="row">
#                 <div class="col-lg-8 mx-auto">
#                     <h2 id="challenges">Challenges</h2>
                    
#                     <p class="lead">
#                         The first challenge was to build a data layer that could be used for statistical analysis of data.
#                     </p>
                    
#                     <p class="lead">
#                         The second challenge was to be able to apply statistical analysis on the whole dataset while retaining each user&#39;s data private.
#                     </p>
                    
#                     <p class="lead">
#                         The third challenge was to allow secure usage from multiple users on desktops and mobile devices.
#                     </p>
                    
#                     <p class="lead">
#                         The fourth challenge was to use architecture and design that allow changes.
#                     </p>
                    
#                 </div>
#             </div>
#         </div>
#     </section>

#     <section id="approach" class="bg-light">
#         <div class="container">
#             <div class="row">
#                 <div class="col-lg-8 mx-auto">
#                     <h2>Approach</h2>
                    
#                     <p class="lead">
#                         Considering the nature of the application - a database one, I decided to use the Oracle 11g XE that comes with a preinstalled APEX and a web server, that unfortunately requires a license to use SSL.
#                     </p>
                    
#                     <p class="lead">
#                         To use SSL I deployed an Apache running on Ubuntu server 16.04, that acts as a reverse proxy and SSL offloader. The certificate was obtained from Let&#39;s Encrypt.
#                     </p>
                    
#                     <p class="lead">
#                         Power BI report is available and could be updated from a reporting server, while the later is feed from the application database.
#                     </p>
                    
#                     <a href="../files/FLEET-MANAGEMENT-PBI.pdf" target="_blank"><i class="fas fa-wave-square"></i></a>
#                 </div>
#             </div>
#         </div>
#     </section>

#     <section id="reports">
#         <div class="container">
#             <div class="row">
#                 <div class="col-lg-8 mx-auto">
#                     <h2>Reports</h2>
#                     <p class="lead">The predefined reports include:</p>
#                     <ul>
#                         <li>Vehicle log</li>
#                     </ul>
#                     <p class="lead">
#                         <i>Total cost of ownership</i>
#                         <img class="img-fluid mx-auto mb-2" src="../img/fleet_management/tco.png" alt="Total cost of ownership">
#                         <br>
#                         The report shows the mileage, fuel amount consumed, fuel and maintenance cost, and the total cost of ownership (TCO), TCO per kilometer per each car in the fleet.
#                     </p>
#                     <p class="lead">
#                         <br> <i>Refueling log</i>
#                         <img class="img-fluid mx-auto mb-2" src="../img/fleet_management/refuel_log.png" alt="Refueling log">
#                         <br>
#                         Log of all refueling events. Enrich them with categorical attributes to enable filtering by vehicle, date attributes, periods between events.
#                     </p>

#                     <p class="lead">
#                         <i>Maintenance log</i>
#                         <img class="img-fluid mx-auto mb-2" src="../img/fleet_management/maintenance_log.png" alt="Maintenance log">
#                         <br>
#                         Log of all maintenance events enriched with periods (date and mileage). Enable filtering by vehicle, date attributes, type, and periods between events.
#                     </p>
#                     <p class="lead">
#                         <i>Statistics per fuel brand</i>
#                         <img class="img-fluid mx-auto mb-2" src="../img/fleet_management/stat_suppliers.png" alt="Statistics per fuel supplier">
#                         <br>

#                     </p>
#                     <p class="lead">
#                         <i>Statistics per drive type</i>
#                         <img class="img-fluid mx-auto mb-2" src="../img/fleet_management/stat_drivetype.png" alt="Statistics per drive type">
#                         <br>
#                     </p>
#                 </div>
#             </div>
#         </div>
#     </section>

#     <section id="graphs" class="bg-light">
#         <div class="container">
#             <div class="row">
#                 <div class="col-lg-8 mx-auto">
#                     <h2>Graphs</h2>
#                     <p class="lead">Graphical visualization shows:</p>
#                     <p class="lead">
#                         <i>Histograms</i>
#                         <img class="img-fluid mx-auto mb-2" src="../img/fleet_management/fuel_amount.png" alt="Histograms">
#                         <br>Histograms to illustrate the frequency of distribution for <i>Fuel price</i>, <i>Fuel Amount</i>, and <i>Mileage</i>.
#                     </p>
#                     <p class="lead">
#                         <i>Fuel prices</i>
#                         <img class="img-fluid mx-auto mb-2" src="../img/fleet_management/fuel_prices.png" alt="Fuel prices">
#                         <br><i>Fuel price</i>, <i>range</i>, <i>min/max</i>, and <i>average</i>.
#                     </p>
#                     <p class="lead">
#                         <i>Fuel expences</i>
#                         <img class="img-fluid mx-auto mb-2" src="../img/fleet_management/fuel_expences.png" alt="Fuel expences">
#                         <br>Comparison of expenses per year, for the last 12 months, including range.
#                     </p>
#                     <p class="lead">
#                         <i>Mileage</i>
#                         <img class="img-fluid mx-auto mb-2" src="../img/fleet_management/mileage.png" alt="Total cost of ownership">
#                         <br>Various comparisons for mileage per months (consequtive), quarter, and year inclding standard deviation.
#                     </p>
#                 </div>
#             </div>
#         </div>
#     </section>

#     <section id="predictions">
#         <div class="container">
#             <div class="row">
#                 <div class="col-lg-8 mx-auto">
#                     <h2>Predictions</h2>
#                     <p class="lead">Predictions suggest actions:</p>
#                     <p class="lead">
#                         <i>Refueling prediction</i>
#                         <img class="img-fluid mx-auto mb-2" src="../img/fleet_management/refueling_predictions.png" alt="Refueling prediction">
#                         <br>Uses historical data to predict next refueling date, and expected mileage reading based on all records or a subset of the last 12 months.
#                     </p>
#                     <p class="lead">
#                         <i>Maintenace prediction</i>
#                         <img class="img-fluid mx-auto mb-2" src="../img/fleet_management/maintenance_prediction.png" alt="Maintenance prediction">
#                         <br>Predicts the next maintenance execution based on the averages for the particular item. The results are sorted by frequency of occurrences.
#                     </p>
#                     <p class="lead">
#                         <i>Maintenace classification</i>
#                         <img class="img-fluid mx-auto mb-2" src="../img/fleet_management/refueling_predictions.png" alt="Maintenace classification">
#                         <br>Historical quarterly aggregation of maintenance expenses per type and vehicle.
#                     </p>
#                 </div>
#             </div>
#         </div>
#     </section>

#     <section id="services" class="bg-light">
#         <div class="container">
#             <div class="row">
#                 <div class="col-lg-8 mx-auto">
#                     <h2>Offered Services</h2>
#                     <p class="lead">The usage is free for selected users. At the moment, you need to be invited to use the platform. The source code can be obtained under the MIT license and deployed on a customer platform.</p>
#                 </div>
#             </div>
#         </div>
#     </section>
---


