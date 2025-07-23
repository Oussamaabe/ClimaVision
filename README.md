# ClimaVision - Weather Visualization Platform 🌦️

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/Oussamaabe/ClimaVision?style=social)](https://github.com/Oussamaabe/ClimaVision/stargazers)
[![Open Issues](https://img.shields.io/github/issues/Oussamaabe/ClimaVision)](https://github.com/Oussamaabe/ClimaVision/issues)

ClimaVision is an advanced weather visualization platform that transforms complex meteorological data into intuitive visual insights. Designed for both casual users and weather enthusiasts, it provides hyperlocal forecasts, historical trends, and climate analytics through an elegant interface.

## 🌟 Key Features

- **Real-time Weather Visualization**  
  Interactive maps with multiple layers (temperature, precipitation, wind)
- **Hyperlocal Forecasts**  
  Precise 7-day predictions for any global location
- **Historical Climate Analysis**  
  Compare weather patterns across different time periods
- **Severe Weather Alerts**  
  Customizable notifications for extreme conditions
- **Multi-device Responsiveness**  
  Seamless experience across mobile, tablet and desktop
- **Data Export Capabilities**  
  Download weather reports in CSV/JSON formats

## 🛠️ Tech Stack

**Frontend**  
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Redux](https://img.shields.io/badge/Redux-593D88?style=for-the-badge&logo=redux&logoColor=white)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white)
![Leaflet](https://img.shields.io/badge/Leaflet-199900?style=for-the-badge&logo=leaflet&logoColor=white)

**Backend**  
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)

**Data & APIs**  
![OpenWeatherMap API](https://img.shields.io/badge/OpenWeatherMap-7CB9E8?style=for-the-badge)
![WeatherAPI](https://img.shields.io/badge/WeatherAPI-009688?style=for-the-badge)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)

**DevOps**  
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

## 🚀 Getting Started

### Prerequisites
- Node.js v16+
- MongoDB Atlas account
- API keys from [OpenWeatherMap](https://openweathermap.org/api) and [WeatherAPI](https://www.weatherapi.com/)

### Installation
```bash
# Clone repository
git clone https://github.com/Oussamaabe/ClimaVision.git

# Install dependencies
cd ClimaVision
npm install

# Configure environment variables
cp .env.example .env

# Fill in your API keys in .env file
OPENWEATHER_API_KEY=your_key
WEATHERAPI_KEY=your_key

# Start development server
npm run dev
```

## 📸 Application Preview

| Dashboard Overview | Interactive Map | Historical Analysis |
|--------------------|-----------------|---------------------|
| ![Dashboard](https://via.placeholder.com/300x200/4d6fb3/ffffff?text=Dashboard+View) | ![Map View](https://via.placeholder.com/300x200/4d6fb3/ffffff?text=Interactive+Map) | ![Historical View](https://via.placeholder.com/300x200/4d6fb3/ffffff?text=Historical+Analysis) |

## 🌐 Live Demo

Experience ClimaVision: [https://climavision.app](https://climaa-vision.netlify.app/)  

## 🧩 Project Structure

```
ClimaVision/
├── client/               # Frontend application
│   ├── public/           # Static assets
│   ├── src/              # React components
│       ├── components/   # Reusable UI components
│       ├── features/     # Redux slices and API services
│       ├── layouts/      # Page layouts
│       ├── pages/        # Application views
│       ├── utils/        # Helper functions
│
├── server/               # Backend application
│   ├── config/           # Configuration files
│   ├── controllers/      # Route controllers
│   ├── middleware/       # Custom middleware
│   ├── models/           # MongoDB models
│   ├── routes/           # API endpoints
│   ├── services/         # Business logic
│   ├── utils/            # Utility functions
│
├── .github/              # CI/CD workflows
├── docker/               # Docker configurations
└── docs/                 # Project documentation
```

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a pull request

See our [Contribution Guidelines](CONTRIBUTING.md) for more details.

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.

## ✉️ Contact

Project Maintainer: [Oussama Belfakir](https://github.com/Oussamaabe)  

Project Link: [https://github.com/Oussamaabe/ClimaVision](https://github.com/Oussamaabe/ClimaVision)

---

**Made by Oussama Belfakir**  
*Weather intelligence for a changing world*
