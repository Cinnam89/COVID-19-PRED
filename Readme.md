# COVID-19 Prediction

This repo aims to do an analysis on COVID-19 spreading patterns based on worldwide data.

## Raw - Data Sources

1. As base data for `COVID-19` in our analysis we're using [Johns Hopkins repository](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_daily_reports). This data is stored into the [Covid Folder](./data/raw/covid/), where we replicate the content from the dialy reports. Don't panic, the data itself is downloaded by the script [main.py](./main.py) whenever it's run. We just maintain a copy here in our repo.

2. As `population density` data we're fetching the latest data available from [World Population Review](https://worldpopulationreview.com/countries/). Since this data is annual, we're keeping it stored in the repo without any change in [Population Density Folder](./data/raw/popden/).

3. As `temperature` data, we're fetching the data from ...

4. As `population risk` we have collected the information that we can find regarding the presence of `ACE2` cells in the human body depending of the population. Please refer to the [Medium story]() for more info about it, and find the raw information in the `Weighted Risk CSV` in the [Raw Population Risk Folder](https://github.com/alvmarrod/COVID-19-PRED/tree/master/data/raw/poprisk).

5. As `governments countermeasures` data, we've collected them from different sources. Since this is the most subjective part, there has not been any data transformation, but directly features that will be in the next section. Please, find it in this [separate readme](./data/raw/govme/Readme.md), due to the large number of countries.

## Features - Model Data

1. `COVID-19` data has been processed and saved from [Raw Covid Folder](./data/raw/covid/) to [Feature Covid Folder](./data/features/covid/).

2. The `population density` data has been processed and saved from [Raw Population Density Folder](./data/raw/popden/) to [Feature Population Density Folder](./data/features/popden/).

3. ...

4. The `weighted population risk` that we have calculated has been processed as well and saved from [Raw Population Risk Folder](https://github.com/alvmarrod/COVID-19-PRED/tree/master/data/raw/poprisk) into the [Features Population Risk Folder](https://github.com/alvmarrod/COVID-19-PRED/tree/master/data/features/poprisk).

5. The `governments measures` that we have collected and directly put into a feature, under our own criteria (that you can find in our [Medium story]()), has been placed directly in the [Features Governments Measures Folder](./data/features/govme/).

## Dependencies

* Pandas
* Numpy
* Matplotlib
* [tqdm](https://github.com/tqdm/tqdm)

## Thanks to

As you may find out going through the project, I would like to thanks to [Pablo G.](), whose effort in collecting needed data made it possible for the project to happen. Specifically:

* The `Weighted Risk` that he has calculated as we specify in the [Medium story](), and that is available in [Raw Population Risk Folder](https://github.com/alvmarrod/COVID-19-PRED/tree/master/data/raw/poprisk).
* The `Governments Measures` that you can find in [Gov. Measures Readme](./data/raw/govme/Readme.md)
