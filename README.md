# Clustering - Airline Passenger Segmentation
## ✈ PROBLEM STATEMENT
As competition intensifies in the airline industry, understanding and segmenting passengers has become essential to maximize revenue. Passenger segmentation enables airlines to identify and the needs and preferenses of different groups, thus, the airlines can personalize their marketing, pricing, and service accordingly [1](https://fastercapital.com/content/Passenger-Segmentation--Customizing-Offerings-to-Maximize-RASM.html).

## 🎯 OBJECTIVES
This project aims to :
1. Perform clustering for airline passenger segmentation using **RFM analysis**
2. Derive actionable insights for each segment group

## 📊 DATASET OVERVIEW
Dataset was given by Dibimbing.id team which you can find it in this repository

Features Overview :
| **Column Name**       | **Description**                                        |
|-------------------------|--------------------------------------------------------|
| `MEMBER_NO`            | Member ID                                              |
| `FFP_DATE`             | Frequent flyer program join date                      |
| `FIRST_FLIGHT_DATE`    | First flight date                                     |
| `GENDER`               | Gender                                                |
| `FFP_TIER`             | Membership class                                      |
| `WORK_CITY`            | City of origin                                        |
| `WORK_PROVINCE`        | Province of origin                                    |
| `WORK_COUNTRY`         | Country of origin                                     |
| `AGE`                  | Customer's age                                        |
| `LOAD_TIME`            | Data collection date                                 |
| `FLIGHT_COUNT`         | Number of flights                                     |
| `BP_SUM`               | Planned trips                                         |
| `SUM_YR_1`             | Total credits/points in the first year               |
| `SUM_YR_2`             | Total credits/points in the second year              |
| `SEG_KM_SUM`           | Total flight distances for finished trips (km)       |
| `LAST_FLIGHT_DATE`     | Last flight date                                      |
| `LAST_TO_END`          | Time from last flight to observation window end      |
| `AVG_INTERVAL`         | Average time interval between flights                |
| `MAX_INTERVAL`         | Maximum time interval between flights in observation window |
| `EXCHANGE_COUNT`       | Number of points exchanges                           |
| `avg_discount`         | Average discount rate                                |
| `Points_Sum`           | Total cumulative points                              |
| `Point_NotFlight`      | Number of non-flight point changes                   |

## 🔎 KEY FINDINGS
### Passenger Clusters
<img width="840" height="545" alt="image" src="https://github.com/user-attachments/assets/e0eff7a4-b583-4587-a69b-e170cc2c02e6" />

**Insights** :
* **Cluster 0 (Lost - New Joiners)**  

Passengers in this cluster recently joined the program, but have not used flights for a long time (436 days); low frequency and monetary; indicates low initial engagement or potential early churn.


* **Cluster 1 (The Champions)**

Although this cluster ranked second for membership duration, passengers have the highest frequency and monetary as well as have used flights more recently.

* **Cluster 2 (Need Attention)**

Longest membership duration; low frequency and monetary; have used flights recently; likely infrequent travelers or those who only fly occasionally.


* **Cluster 3 (Recent Passengers - Potential Loyalist)**  

Passengers in this clustes just joined the program more recently, thus, these passengers still have low values of frequency and monetary. However, since their overall behavioral patterns are similar to those in Cluster 2—who have been members for the longest time—this suggests that this passenger can be considered as potential loyalist

## 🛄FUTURE IMPROVEMENT
Since this project experimented on using LRMFC model which is a modified RFM model, future experiments could try applying the traditional RFM model instead. With fewer features, the RFM model might result in better cluster separation and simpler interpretation.


