# ClimSav

This repository hosts a climate model codenamed *ClimSav*, tailored for East African regions. Using advanced climate data and predictive analytics, it provides crucial insights into regional climate patterns, extreme weather events, and long-term climate trends. Designed for researchers, policymakers, and practitioners, this model aims to enhance climate resilience and support sustainable development initiatives in East Africa.
*ClimSav* is an advanced climate model built upon the insights of an existing *ClimaX*, with significant innovations tailored for East African regions. This model incorporates not only the foundational aspects of *ClimaX* but also introduces enhancements specifically designed for the region, including precipitation prediction and corresponding precipitation percentages.

## Features

- **East Africa Focus**: Adapted to provide precise climate insights and predictions specifically for East African regions.
- **Precipitation Prediction**: Includes predictions for precipitation levels along with their corresponding percentages, offering a detailed view of rainfall patterns.
- **Enhanced Spatial Resolution**: Utilizes both coarse and fine spatial resolutions to improve the accuracy and granularity of climate predictions.

## The available Data Resolutions

### 5.625° Data

The **5.625° data** refers to climate data that is spatially resolved with a grid spacing of 5.625 degrees. This means that each grid cell represents an area of approximately 5.625 degrees of latitude by 5.625 degrees of longitude. This resolution provides a coarser view of the climate, suitable for broader-scale modeling and analysis.

### 1.40625° Data

The **1.40625° data** refers to climate data with a finer spatial resolution of 1.40625 degrees. Each grid cell represents an area of approximately 1.40625 degrees of latitude by 1.40625 degrees of longitude. This higher resolution offers a more detailed view of the climate, capturing finer spatial variations and providing more accurate local climate information.

### Importance of Resolution

- **Coarse Resolution (5.625°)**: Useful for global-scale models and analyses where detailed local variations are less critical. It provides a broad overview of climate patterns and trends.
- **Fine Resolution (1.40625°)**: Essential for regional and local climate modeling where understanding specific spatial variations is important. It allows for more precise predictions and insights, particularly valuable for applications that require detailed climate information, such as regional forecasting and impact assessments.

## Stage 1
In the initial stage of the project, we will utilize existing CMIP6 datasets to train the ClimSav model. Once trained, the model will be tested with data from sensors currently being installed, as well as data extracted from Google APIs. 

We have developed a weather visualization app that will leverage ClimSav's predictions. This app will provide forecasts for 6 hours, 12 hours, 24 hours, and up to 28 days ahead. The predicted weather parameters will be evaluated through a citizen science approach, enabling broad feedback on the accuracy of our forecasts in real-world scenarios.
 




