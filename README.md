# Global Terrorism (Exploratory Data Analysis)
  This repository contains files for Global Terrorism Exploratory Data Analysis.

## Overview -
  - This Project is exploratory data analysis of [Global Terrorism Database](https://www.kaggle.com/START-UMD/gtd) (GTD) and more about the [data](https://www.start.umd.edu/gtd/), it's collection methodology, definitions, and coding schema can be found [here](https://start.umd.edu/gtd/downloads/Codebook.pdf).
  - Here I tried to find out How relevant is the definiton of Terrorism to this data? I tried to gain understanding of how terrorism spread across globe, it's relevant details, though knowing philosophical thought behind these incident would not be possible without domain expertise.
  - This project has also been converted to [Dashboard](https://terrorismglobal.herokuapp.com/) for users to interact and compare the results for more details.
  
## Data Set Information -
  * Geography: Worldwide
  * Time period: 1970-2017, except 1993
  * Unit of analysis: Attacks and Casualities
  * Variables: >100 variables on location, tactics, perpetrators, targets, and outcomes but used around <ins>30 parameters as most of them has more than *80% missing values*</ins>.
  * Sources: Unclassified media articles (<ins>Note: Please interpret changes over time with caution. Global patterns are driven by diverse trends in particular regions, and data collection is influenced by fluctuations in access to media coverage over both time and place.</ins>)

## How Data looks? (After some cleaning [first 5 rows])
  |    |   year |   month |   day |   extended | country_txt        | region_txt                  | province   | city          |   latitude |   longitude |   vicinity |   crit1 |   crit2 |   crit3 |   doubtterr |   multiple |   success |   suicide | attacktype                     | target_type                 |   targsubtype1 | target_subtype                                  | target_entity                                                 | nationality        | group               |   individual | weapon_type   | weapon_subtype                    |   killed |   wounded |   property |   hostages/kidnapping |   cross_border |   ideological_international | Date                |   week | day_name   |   weekday |   is_weekend |   casualities |   casualities_median |
|---:|-------:|--------:|------:|-----------:|:-------------------|:----------------------------|:-----------|:--------------|-----------:|------------:|-----------:|--------:|--------:|--------:|------------:|-----------:|----------:|----------:|:-------------------------------|:----------------------------|---------------:|:------------------------------------------------|:--------------------------------------------------------------|:-------------------|:--------------------|-------------:|:--------------|:----------------------------------|---------:|----------:|-----------:|----------------------:|---------------:|----------------------------:|:--------------------|-------:|:-----------|----------:|-------------:|--------------:|---------------------:|
|  0 |   1970 |       7 |     2 |          0 | Dominican Republic | Central America & Caribbean | nan        | Santo Domingo |    18.4568 |    -69.9512 |          0 |       1 |       1 |       1 |           0 |          0 |         1 |         0 | Assassination                  | Private Citizens & Property |             68 | Named Civilian                                  | Julio Guzman                                                  | Dominican Republic | MANO-D              |            0 | Unknown       | nan                               |        1 |         0 |          0 |                     0 |              0 |                           0 | 1970-07-02 00:00:00 |     27 | Thursday   |         3 |            0 |             1 |                    1 |
|  1 |   1970 |       1 |     1 |          0 | United States      | North America               | Illinois   | Cairo         |    37.0051 |    -89.1763 |          0 |       1 |       1 |       1 |           0 |          0 |         1 |         0 | Armed Assault                  | Police                      |             22 | Police Building (headquarters, station, school) | Cairo Police Headquarters                                     | United States      | Black Nationalists  |            0 | Firearms      | Unknown Gun Type                  |        0 |         0 |          1 |                     0 |             -9 |                          -9 | 1970-01-01 00:00:00 |      1 | Thursday   |         3 |            0 |             0 |                    0 |
|  2 |   1970 |       1 |     2 |          0 | Uruguay            | South America               | Montevideo | Montevideo    |   -34.8912 |    -56.1872 |          0 |       1 |       1 |       1 |           0 |          0 |         0 |         0 | Assassination                  | Police                      |             25 | Police Security Forces/Officers                 | Juan Maria de Lucah/Chief of Directorate of info. and intell. | Uruguay            | Tupamaros (Uruguay) |            0 | Firearms      | Automatic or Semi-Automatic Rifle |        0 |         0 |          0 |                     0 |              0 |                           0 | 1970-01-02 00:00:00 |      1 | Friday     |         4 |            0 |             0 |                    0 |
|  3 |   1970 |       1 |     2 |          0 | United States      | North America               | California | Oakland       |    37.7919 |   -122.226  |          0 |       1 |       1 |       1 |           1 |          0 |         1 |         0 | Bombing/Explosion              | Utilities                   |            107 | Electricity                                     | Edes Substation                                               | United States      | Unknown             |            0 | Explosives    | Unknown Explosive Type            |        0 |         0 |          1 |                     0 |             -9 |                          -9 | 1970-01-02 00:00:00 |      1 | Friday     |         4 |            0 |             0 |                    0 |
|  4 |   1970 |       1 |     2 |          0 | United States      | North America               | Wisconsin  | Madison       |    43.0766 |    -89.4125 |          0 |       1 |       1 |       1 |           0 |          0 |         1 |         0 | Facility/Infrastructure Attack | Military                    |             28 | Military Recruiting Station/Academy             | R.O.T.C. offices at University of Wisconsin, Madison          | United States      | New Year's Gang     |            0 | Incendiary    | Molotov Cocktail/Petrol Bomb      |        0 |         0 |          1 |                     0 |              0 |                           0 | 1970-01-02 00:00:00 |      1 | Friday     |         4 |            0 |             0 |                    0 |

## Some Explortory Data Analysis Results -
  - Most affected Countries:
    ![Image](https://github.com/matsujju/Global-Terrorism-EDA/blob/master/images/Most%20Affected%20countries.png)
   
  - Ratio of Terror Attacks and People Killed:
    ![Image](https://github.com/matsujju/Global-Terrorism-EDA/blob/master/images/Attack%20Vs%20killed.png)
    
  - How the casualities look over the Map of Iraq?
    ![Image](https://github.com/matsujju/Global-Terrorism-EDA/blob/master/images/Satellite%20overview%20of%20Iraq.png)
  
  - More Details about Iraq:
    ![Image](https://github.com/matsujju/Global-Terrorism-EDA/blob/master/images/Country%20Analysis%20of%20Iraq.png)
    
  - How different Regions are affected over the years?
    ![Image](https://github.com/matsujju/Global-Terrorism-EDA/blob/master/images/How%20Regions%20are%20affected.png)
    
  - Weapons used in different regions:
    ![Image](https://github.com/matsujju/Global-Terrorism-EDA/blob/master/images/Weapons%20used%20in%20Regions.png)
    
  - Motivation behind these Attacks:
    ![Image](https://github.com/matsujju/Global-Terrorism-EDA/blob/master/images/terror_word_cloud.png)

## Libraries used -
  - [Pandas](https://pandas.pydata.org/) : Used for exploring and manipulating dataset
  - [Numpy](https://numpy.org/doc/stable/reference/index.html) : Working with arrays
  - [Seaborn](https://seaborn.pydata.org/) and [Matplotlib](https://matplotlib.org/) : Visualization library for plotting graphs (2-D static plots)
  - [Plotly](https://plotly.com/python/) : Interactive visualization library for Graphs 
 

