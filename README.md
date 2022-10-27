# CapstoneReport
## Problems & Objective
Problems:
- Outdated Pricing System
- Operational Challenges under competition and covid-19

Objective:
To encourage driver retention & greater revenue generation:
- Optimized the current model
- Proposed a strategic pricing project

## Implementation & Rationale
<img src="https://github.com/shaw6741/CapstoneReport/blob/master/images/Slide7.JPG" width=80% height=80%>

<img src="https://github.com/shaw6741/CapstoneReport/blob/master/images/Slide8.JPG" width=80% height=80%>

## Methodology
<img src="https://github.com/shaw6741/CapstoneReport/blob/master/images/Slide9.JPG" width=80% height=80%>

### Clustering - define new pricing structure
The purpose of clustering was to gauge the rarity of each delivery in the data set. To this end, only
delivery-related variables were used. A delivery was assigned a rarity score based on how dissimilar
it was to the cluster it belonged to. Price adjustments were then calculated based off of the rarities. The
new prices then translated to an increase in revenue.

<img src="https://github.com/shaw6741/CapstoneReport/blob/master/images/Slide10.JPG" width=80% height=80%>

### Regression & Classification
To give the best outcomes for the drivers and customers, we maximized both the DIFOT probability
and the price.

<img src="https://github.com/shaw6741/CapstoneReport/blob/master/images/Slide11.JPG" width=80% height=80%>

__Classification for DIFOT:__
DIFOT: Delivery In Full On Time, 0 or 1

- Logistic Regression (benchmark)
- Bagging Ensemble
- XGBoost (best)

__Regression for Price:__

To predict the adjusted prices using a combination of delivery.
variables and courier variables.

- Random Forest

## Recommendation algorithm
A new recommendation system was proposed to advance the current pricing framework. The model
building process included two steps:

1. Define new pricing structures using Partitioning Around Medoids (PAM).
2. With the adjusted prices:
  - Predict DIFOT (Deliver In Full On Time) outcomes with classification models.
  - Assign price to each delivery using regression models.

This algorithm implementation would cycle through each driver and determine with the models a price and DIFOT for a new delivery.
It optimised each delivery by selecting drivers that would satisfy a delivery with DIFOT and with the “highest” price possible, therefore optimising couriers’ revenue generation and customer satisfaction.

<img src="https://github.com/shaw6741/CapstoneReport/blob/master/images/recommendation%20system%20workflow.png" width=80% height=80%>

## Projected Impact
<img src="https://github.com/shaw6741/CapstoneReport/blob/master/images/Slide12.JPG" width=80% height=80%>

## Limitations & Next Steps
<img src="https://github.com/shaw6741/CapstoneReport/blob/master/images/Slide13.JPG" width=50% height=50%>
<img src="https://github.com/shaw6741/CapstoneReport/blob/master/images/Slide15.JPG" width=50% height=50%>
