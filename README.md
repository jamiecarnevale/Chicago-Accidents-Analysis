# Chicago Accidents ML Modeling

Author: Jamie Carnevale

## Overview

Hello Chicago Traffic Safety Board! I am here to present a classifcation model that can predict the primary contributory cause of a car accidents.

## Business Understanding

Modeling for primary contributory causes of car accidents can help us identify areas in which we can make the most difference in reducing the amount of car accidents.

## Model Classification Target Groups

In order to create this model, the primary causes for accidents were binned into four different categories: reckless driving, missed or misunderstood traffic signs or rules, issue with driver or vehicle, and external variable.

Some of the subcategories that fall under these four main categories include:
- Reckless driving: following too closely, improper overtaking/passing, texting,  failing to reduce speed to avoid crash
- missed or misunderstood traffic signs or rules: disregarding yield sign, disregarding traffic signals, disregarding stop sign, failing to yield right of way
- issue with driver or vehicle: driving skills/knowledge/experience, physical condition of driver, had been drinking
- external variable: weather, animal, distraction from outside vehicle, vision obscured, road construction

![accidentsbyreasonbarchart](/images/accidentsbyreasonbarchart.png)

Even without modeling, we have some insight into what we should do to try and minimalize the amount of accidents: to find ways to decrease the amount of reckless driving.

## Confusion Matrix

While the model did a great job at correctly predicting reckless driving to be the primary cause, it also occasionally predicted the primary cause to be reckless driving when it was really another primary reason. This is likely due to the complexity of the dataset, the skewed nature of the data, and the aspect that there are often multiple causes of an accident.

![x](/images/confusionmatrix.png)

## Top Variables Affecting the Model

Here, we see the top 7 variables that helps the model classify. However, it's best to just focus on the top 3, so we can make some actionable plans that help us reduce accident rates. These top three variables include: Entering Traffic Lane From Parking, Physical Condition Impaired - Alcohol, and Accident Occurred at a Stop Sign/Flasher.

![y](/images/keyvariablesaffectingmodel.png)

Here we can see the actual distributions of the accidents when each of those variables were present vs the overall distribution. As you can see, the distributions are significantly different. For example, when the driver is impaired by alcohol, the vast majority of accidents that occur are due to them being impaired by alochol.

![z](/images/piecharts.png)


## In Sum

Based on model, the key factors that help classify the primary cause of an accident are:

- Entering Traffic Lane From Parking, Physical Condition Impaired – Alcohol, Accident Occurred at a Stop Sign/Flasher

Recommendations:
- Improve parking lot design, focus on parking lots in driver education 
- More DUI checkpoints, create programs to encourage Uber/Lyft/Taxi usage when drinking
- Improve visibility of stop signs (maintain trees and other potential visibility blockers)


