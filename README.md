# Airline On Time Arrivals and Delays Throughout The United States

## Introduction

With this project, we well be analyzing data in regards to the On-Time Arrivals and Delays for Airlines located in the United States.

## Data Dictionary

| Field | Description |
| :--- | :--- |
| Year | Year of delay |
| Month | Month of delay |
| carrier | Two character designator for the carrier |
| carrier_name | Full name of Carrier |
| airport | 3 letter designator of airport |
| airport_name | Full name of airport |
| arr_flights | Total number of arriving flights for carrier/airport |
| arr_del15 | Number of arriving flights that were delayed by more than 15 minutes |
| carrier_ct | Number of arriving flights delayed due to carrier issue |
| weather_ct | Number of arriving flights delayed due to weather issue |
| nas_ct | Number of arriving flights delayed due to national air system issue |
| security_ct | Number of arriving flights delayed due to security issue |
| late_aircraft_ct | Number of arriving flights delayed due to an earlier late arrival of an aircraft |
| arr_canceled | Number of cancelled flights |
| arr_diverted | Number of diverted flights |
| arr_delay | Number of delayed minutes due to delays |
| carrier_delay | Number of delayed minutes due to carrier issues |
| weather_delay | Number of delayed minutes due to weather issues |
| nas_delay | Number of delayed minutes due to nationa air systems issues |
| security_delay | Number of delayed minutes due to security issues |
| late_aircraft_delay | Number of delayed minutes due to earlier late arrival of aircraft |

* When multiple causes are assigned to one delayed flight, each cause is prorated based on delayed minutes it is responsible for. The displayed numbers are rounded and may not add up to the total. (Distinguished with _ct)

## Carriers

| Field | Description |
| :--- | :---|
| 9E | Endeavor Air Inc. |
| AA | American Airlines |
| AS | Alaska Airlines Inc. |
| B6 | JetBlue Airways |
| DL | Delta Airlines Inc. |
| EV | ExpressJet Airlines LLC |
| F9 | Frontier Airlines Inc. |
| G4 | Allegiant Air |
| HA | Hawaiin Airlines Inc. |
| MQ | Envoy Air |
| NK | Spirit Airlines |
| OH | PSA Airlines Inc. |
| OO | SkyWest Airlines Inc. |
| QX | Horizon Air |
| UA | United Air Lines Inc. |
| WN | Southwest Airlines Co. |
| YV | Mesa Airlines Inc. |
| YX | Republic Airline |


* Start *framing* the problem -- This is Step 1 of the Data Science Workflow
   * Make a list of **what you know**
       * Multiple ways a flight can be delayed
       * Each airport can have different reasons for having delays
       * Each carrier has different reasons for delays
   * Make a list of **what you don't know**
       * What kind of weather caused delays
       * What exactly was the NAS reasons for delays
       
   * Make a list of possible problem statements
       * Are delays happening more at smaller airports or larger airports?
       * Is it more likely that one carrier will be delayed compared to another similar carrier?
       * How often was weather a factor in a delay?
       * What airlines have the highest/lowest percentage of delays?



## Important Links

* [Final Report Notebook](report.ipynb)
* [EDA Notebook](eda.ipynb)
* [Link 1](https://www.transtats.bts.gov/OT_Delay/ot_delaycause1.asp?qv52ynB=qn6n&20=E) - Source data



# Things to do
    * Change year and month to date-time format - done
    * Combine year and month into one column - done
    * Remove rows with missing values (no arrival flights) - done
    * Convert minutes delayed into integer
    * Display # of delayed flights per carrier 
    * Find carrier with most delays as a percentage of total flights
    * Find top 5 airports with most delays
    * Find top 5 carriers with least amount of delays
    * Find delays per month
    
Notes:

Think about what kind of questions you are trying to answer



Questions:
- Should year/date be the index?
- replace first row with new names