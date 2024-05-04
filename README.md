# Weather API Integration using Spring Boot Java

This project integrates the Weather API from Rapid API into a Spring Boot Java application to provide weather forecast information for any city. It exposes RESTful APIs with JSON response and uses header-based authentication with random client ID and client secret.

## APIs

### 1. Get Weather Forecast Summary by Location Name
- Endpoint: `/api/weather/summary/{city}`
- Description: Retrieves the weather forecast summary for a specific city.
- API Method: `RapidApiGetForecastSummaryByLocationName`
- [API Documentation](http://localhost:8080/auth/forecast)


## Authentication
- Method: Header-based authentication
- Headers:
  - `X-Client-ID`: Random client ID
  - `X-Client-Secret`: Random client secret

## Setup Instructions
1. Clone the repository:


2. Open the project in your preferred IDE (e.g., IntelliJ IDEA, Eclipse).

3. Configure Rapid API Key:
- Sign up on Rapid API and obtain your API key for the Weather API.
- Open `src/main/resources/application.properties`.
- Set your API key:
  ```properties
  weather.api.key=your-api-key
  ```

4. Run the Application:
- Build and run the `WeatherApiApplication.java` file in your IDE.
- The API will start on `http://localhost:8080`.

## Usage
- Send GET requests to the specified endpoints to retrieve weather forecast information.
- Include headers `X-Client-ID` and `X-Client-Secret` with random values for authentication.

## Contributing
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/new-feature`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add new feature'`).
5. Push to the branch (`git push origin feature/new-feature`).
6. Create a new Pull Request.


