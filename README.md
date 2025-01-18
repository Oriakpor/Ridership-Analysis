# MTA-Daily-Ridership-Analysis
The MTA daily ridership dataset provides systemwide ridership and traffic estimates for the Metropolitan Transportation Authority's (MTA) different services beginning March 1st, 2020, and provides a percentage comparison against pre-pandemic figures.

# Project Objectives:
The project objectives are to determine:
- What was the share of traffic by service before the pandemic? Did it change?
- Which service saw the biggest drop-off in traffic? Has it recovered?
- Which service was the fastest to recover?
- When are all the services estimated to return to pre-pandemic levels?

# Data Source
The MTA Daily Ridership data was obtained from Maven Analytics:
- [https://mavenanalytics.io/data-playground]

# Tool used for Analysis:
- Python

# Results:
## 1a. share of traffic pre-pandemic (%) is:
- Subways: % of Comparable Pre-Pandemic Day                (55.46)
- Buses: % of Comparable Pre-Pandemic Day                  (54.69)
- LIRR: % of Comparable Pre-Pandemic Day                   (59.13)
- Metro-North: % of Comparable Pre-Pandemic Day            (51.08)
- Access-A-Ride: % of Comparable Pre-Pandemic Day          (86.17)
- Bridges and Tunnels: % of Comparable Pre-Pandemic Day    (93.38)
- Bridges and Tunnels: % of Comparable Pre-Pandemic Day    (93.38)

![Bar-chart showing the Pre-pandemic traffic share](https://github.com/user-attachments/assets/ee535280-914c-4c14-ada8-ee69a42a5a56)


### Post-pandemic estimated_ridership share is: 
- Subways: Total Estimated Ridership                  (4280447795)
- Buses: Total Estimated Ridership                    (1717716966)
- LIRR: Total Estimated Ridership                      (231947958)
- Metro-North: Total Estimated Ridership               (195999394)
- Access-A-Ride: Total Scheduled Trips                  (37432255)
- Bridges and Tunnels: Total Traffic                  (1459658489)
- Staten Island Railway: Total Estimated Ridership       (7556480)

![Bar-chart showing the Post-pandemic traffic share](https://github.com/user-attachments/assets/21e12a66-a333-4f94-8e87-405a5a168531)


## 1b. However, looking at the estimated ridership and pre-pandemic share of traiffic, we notice that the estimated ridership are not given in percentages. Hence, we'll have to calculate it's percentage and make comparison between both to get the change. Using this approach, we obtained the following(from pre-pandemic to post-pandemic):
- Subways: 55.46% to 44.54%
- Buses: 54.69% to 45.37%
- LIRR: 59.13% to 40.87%
- Metro-North: 51.08% to 48.92%
- Bridges and Tunnels: 93.38% to 6.62%
- Staten Island Railway: 37.82% to 62.19%


![Bar-chart showing the change in traffic share](https://github.com/user-attachments/assets/e2024800-4f36-4fdd-a64b-3a85c56f1866)

### Note: The drop (change) in post-pandemic traffic shares makes sense given the significant shifts in behavior, Infrastructure, and societal norms caused by the pandemic. Many of these changes—such as remote work, safety concerns, and shifts in travel patterns—are logical and expected consequences of a global disruption like COVID-19.

## 2a. Service with the biggest drop off is: Bridges and Tunnels: 93.38% to 6.62%
## 2b. By extracting the recent data-points and compare them to traffic shares at pre-pandemic levels, we obtained the following recovery levels:
- Subways: Subway has a recovery level of 70%. This indicates that while usage has rebounded, it remains 30% below pre-pandemic levels.
- Buses: Buses has a recovery level of 58%. This indicates it remains 42% below pre-pandemic levels.
- LIRR: This has a recovery level of 82%, which indicates a rebound but still 18% pre-pandemic levels.
- Metro-North: Metro-North has a recovery level of 76%, indicating a rebound still below 24% below pre-pandemic levels.
- Access-A-Ride: This has recovery level of 126%, indicating it has recovered and exceeded pre-pandemic levels.
- Bridges and Tunnel:  Bridges and Tunnel -- the service that got the biggest drop off has a recovery of 103%.
- Staten Island Railway: Staten Island Railway has a recovery level of 42%, indicating a rebound 58% below pre-pandemic levels. This is the service showing the weakest recovery.

### In conclusion, the service with biggest drop off has fully recovered and exceeded pre-pandemic levels.

# 3. The service that was the fastest to recover is: Bridges and Tunnels.
![Recovery Trends overtime](https://github.com/user-attachments/assets/41d79a4f-322a-4726-935e-9d54521656b3)

# 4. Using Linear Regression analysis to predict the date of recovery, the following Estimated Date of Recovery for the services were obtained:
- Subways: % of Comparable Pre-Pandemic Day is: 2026-04-14
- Buses: % of Comparable Pre-Pandemic Day is: 2028-06-20
- LIRR: % of Comparable Pre-Pandemic Day is: 2024-12-02
- Metro-North: % of Comparable Pre-Pandemic Day is: 2025-05-28
- Access-A-Ride: % of Comparable Pre-Pandemic Day is: 2023-05-13
- Bridges and Tunnels: % of Comparable Pre-Pandemic Day is: 2023-06-17


# Recommendations
## 1. Services with Weak Recovery Levels should be a priority
### a. Staten Island Railway shows the weakest recovery (42% recovery):
- Efforts should focus on increasing service reliability and frequency.
- Addressing safety or accessibility concerns that may discourage users.
- Improve marketing campaigns to promote the service.

### b. Buses has a 58% recovery, despite being an essential service:
- Improve bus schedules and reducing wait times.

## 2.  Maintain and Strengthen Services with High Recovery Levels
### a. Bridges and Tunnels (103% recovery):
- Maintainance of infrastructure, monitor and manage congestion to avoid overuse.
- Use flexible toll rates to manage peak-hour demand.

### b. Access-A-Ride (126% recovery):
- Expand fleet capacity to meet rising demand.
- Introduce technological booking systems to improve efficiency.
- Ensure equitable access for all eligible riders.

## 3. Focus on Medium-Recovery Services with Strong Potential
### a. LIRR (82% recovery) and Metro-North (76% recovery): Both are the busiest and second busiest commuters railroad in North America respectively.
- Introduce promotional fares to attract riders.
- Invest in modernized infrastructuree, such as updated stations to improve quality of service

### b. Subways (70% recovery):
- Improve safety measures, such as cleanliness and surveillance, to attract riders who may be deterred on health grounds.
- Adopt online payment systems to streamline access.

### 4. Recovery dates, as estimated using linear regression, indicate that services like LIRR (2024-12-02) and Metro-North (2025-05-28) are on track to recover sooner than others such as Buses (2028-06-20).
- Continuously monitor ridership data to spot changes in recovery trends.
- Allocation of more resources to services that show slower recovery dates.







  



