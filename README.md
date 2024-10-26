# Real-Time Weather Monitoring System

## Overview
This project implements a real-time data processing system to monitor weather conditions and provide summarized insights using rollups and aggregates. It retrieves data from the [OpenWeatherMap API](https://openweathermap.org/).

## Features
- Real-time weather data retrieval for major metros in India (Delhi, Mumbai, Chennai, Bangalore, Kolkata, Hyderabad).
- Daily weather summaries with average, maximum, and minimum temperatures.
- User-configurable alert thresholds for temperature conditions.
- Data visualizations for daily summaries and historical trends.

## Data Source
The system utilizes the OpenWeatherMap API. You need to sign up for a free API key to access weather data, focusing on the following parameters:
- **main**: Main weather condition (e.g., Rain, Snow, Clear)
- **temp**: Current temperature in Celsius
- **feels_like**: Perceived temperature in Celsius
- **dt**: Time of the data update (Unix timestamp)

## Getting Started

### Prerequisites
- **Node.js** (version 14 or above)
- **npm** (Node package manager)
- A database (MongoDB recommended; Docker can be used)

### Docker Setup (Optional)
To run MongoDB using Docker, use the following command:
```bash
docker run --name mongodb -d -p 27017:27017 mongo
```

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Padmajasharma/Smart-Weather-Analytics
   cd Smart-Weather-Analytics
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set your OpenWeatherMap API key in your environment or configuration file.

4. Start the application:
   ```bash
   node src/app.js
   ```

## Usage
- The application will fetch weather data every 5 minutes by default.
- User can configure thresholds for alerts based on temperature conditions.

## Testing
To ensure the functionality of the system, the following test cases are implemented:
- System Setup
- Data Retrieval
- Temperature Conversion
- Daily Weather Summary
- Alerting Thresholds

## Design Choices
- **Modular Structure**: Organized into controllers, models, and routes for better maintainability.
- **Asynchronous Data Fetching**: Utilizes async API calls to keep the application responsive.
- **User Preferences**: Supports multiple temperature units for user flexibility.

## Contributing
Contributions are welcome! Please feel free to submit a pull request or open an issue for discussion.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements
- [OpenWeatherMap API](https://openweathermap.org/)
- [Node.js](https://nodejs.org/)
```

Make sure to replace `<your-repository-url>` and `<your-repository-folder>` with the actual values. Feel free to modify any part of this README to better fit your project's details!
