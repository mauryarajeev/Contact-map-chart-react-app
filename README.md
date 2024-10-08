# COVID-19 Dashboard Application

This is a COVID-19 dashboard application that provides information about active cases, deaths, and recoveries related to COVID-19. It fetches data from various API endpoints to display country-specific and worldwide COVID-19 information.

### 1. Deployment link

- **URL**: [https://contact-map-chart-react-app.vercel.app/contacts)


## Getting Started

To start the application, follow these steps:

1. **Install Dependencies**: Run the following command to install all project dependencies:

    ```
    npm install
    ```

2. **Start the Application**: Launch the application by running:

    ```
    npm start
    ```

3. **Open in Your Browser**: Once the application is running, open your web browser and navigate to:

    ```
    http://localhost:3000
    ```

## API Endpoints Used

### 1. Historical Data (COVID-19 Cases, Deaths, Recoveries)

- **URL**: [https://disease.sh/v3/covid-19/historical/all?lastdays=all](https://disease.sh/v3/covid-19/historical/all?lastdays=all)

This endpoint returns historical data regarding COVID-19 cases, deaths, and recoveries. The data is presented in the following format:

```javascript
cases: {
    ['1/2/2022', 89],
    // ...
},
deaths: {
    ['1/2/2022', 89],
    // ...
},
recovered: {
    ['1/2/2022', 89],
    // ...
}```

````

 
### 2. Country-Specific COVID-19 Information
- **URL**: [https://disease.sh/v3/covid-19/countries](https://disease.sh/v3/covid-19/countries)
This endpoint returns an array of objects, each containing country-specific information regarding COVID-19. Each object includes the following details:

```
[
    {
        country: String,
        active: Number,
        deaths: Number,
        recovered: Number,
        // ...
    },
    // ...
]
 ```



## GET request return object containing world wide information regarding covid 19

## 3. URL: https://disease.sh/v3/covid-19/all

````
    {
        total:Number,
        active:Number,
        deaths:Number,
        recovered:Number
        ...
    }
    
````
    
