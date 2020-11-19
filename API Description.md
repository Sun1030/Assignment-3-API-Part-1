## Manitoba Covid Tracker API

#### Description : The Manitoba Covid Tracker API can be used to programmatically retrieve and analyze data relate to the current Covid situation in the Manitoba province.

 
Manitoba covid case breakdown by health region
##### Options: 

* GET method 1: get all covid case recoveries in Manitoba. Parameters: health regions (***optional***), to date (dd.mm.yyyy) (***optional***)

* GET method 2: get all covid cases in Manitoba. Parameters: from date (dd.mm.yyyy) (***optional***), to date (dd.mm.yyyy) (***optional***)

* GET method 3: get covid deaths and hospitalizations. Parameters: health regions

#### Sample Request

###### Get Recoveries
```
https://api.covidmanitoba.ca/recoveries/json?region=winnipeg&todate=30.08.2020
```

###### Get Covid Cases
```
https://api.covidmanitoba.ca/cases/json?region=winnipeg&fromdate=18.11.2020&todate=19.11.2020
```

#### Sample Response

```
    {
      "results":
      {
        "Health Region": "All"
        "Recovered":"89,232",
        "To date":"August 30th, 2020"
      },
       "status":"success"
    }
```

```
    {
      "results":
      {
        "Health Region": "Winnipeg"
        "Recovered":"89,232",
        "To date":"August 30th, 2020"
      },
       "status":"success"
    }
```
