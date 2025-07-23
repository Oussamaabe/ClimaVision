# ClimaVision - Interactive Weather Dashboard 🌤️

[![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Netlify](https://img.shields.io/badge/Netlify-00C7B7?style=for-the-badge&logo=netlify&logoColor=white)](https://www.netlify.com/)
[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

![ClimaVision Banner](https://via.placeholder.com/1200x400/4d6fb3/ffffff?text=ClimaVision+-+Real-time+Weather+Visualization)

ClimaVision is an interactive weather dashboard that transforms complex meteorological data into intuitive visual insights. Built with modern web technologies, it provides real-time weather forecasts, interactive charts, and a seamless user experience for exploring weather patterns.

**Live Demo:** [https://climaa-vision.netlify.app](https://climaa-vision.netlify.app)

## ✨ Key Features

- **5-Day Dynamic Forecast**  
  Hourly and daily predictions with temperature, humidity, and precipitation data
- **Interactive Data Visualization**  
  Beautiful charts for temperature trends, precipitation probability, and wind patterns
- **Real-time Weather Updates**  
  Instant refresh with current conditions for any global location
- **Intuitive Search Interface**  
  Find weather for cities worldwide with auto-suggestions
- **Responsive Design**  
  Flawless experience across mobile, tablet, and desktop devices
- **Weather Metrics Dashboard**  
  Comprehensive display of feels-like temperature, UV index, and visibility

## 🛠️ Tech Stack

**Core Framework**  
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)

**Data Management**  
![Tanstack Query](https://img.shields.io/badge/Tanstack_Query-FF4154?style=flat-square&logo=reactquery&logoColor=white)
![OpenWeatherMap API](https://img.shields.io/badge/OpenWeatherMap-7CB9E8?style=flat-square)

**UI & Styling**  
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Recharts](https://img.shields.io/badge/Recharts-FF6384?style=flat-square)

**Deployment**  
![Netlify](https://img.shields.io/badge/Netlify-00C7B7?style=flat-square&logo=netlify&logoColor=white)

## 🚀 Getting Started

### Prerequisites
- Node.js v18+
- OpenWeatherMap API key (free tier available)

### Installation
```bash
# Clone repository
git clone https://github.com/Oussamaabe/ClimaVision.git

# Navigate to project directory
cd ClimaVision

# Install dependencies
npm install

# Create environment file
echo "REACT_APP_OPENWEATHER_API_KEY=your_api_key_here" > .env

# Start development server
npm start
```

## 🌐 Live Demo

Experience ClimaVision:  
[https://climaa-vision.netlify.app](https://climaa-vision.netlify.app)

*Try searching for: Paris, New York, Tokyo, Sydney*

## 🧩 Project Structure

```
ClimaVision/
├── public/               # Static assets and HTML template
├── src/                  # Application source code
│   ├── assets/           # Images, icons, and fonts
│   ├── components/       # Reusable UI components
│   │   ├── charts/       # Data visualization components
│   │   ├── layout/       # Layout components
│   │   └── ui/           # Generic UI elements
│   ├── features/         # Application features
│   │   ├── current/      # Current weather display
│   │   ├── forecast/     # Forecast functionality
│   │   └── search/       # Location search
│   ├── hooks/            # Custom React hooks
│   ├── services/         # API services and clients
│   ├── types/            # TypeScript type definitions
│   ├── utils/            # Utility functions
│   ├── App.tsx           # Main application component
│   └── index.tsx         # Application entry point
├── .env.example          # Environment variables template
├── tsconfig.json         # TypeScript configuration
└── package.json          # Project dependencies
```

## 💡 Key Implementation Details

### Efficient Data Fetching
```typescript
// Using Tanstack Query for efficient API data management
const { data, isLoading, error } = useQuery({
  queryKey: ['weather', location],
  queryFn: () => fetchWeatherData(location),
  staleTime: 15 * 60 * 1000, // 15 minutes cache
});
```

### Responsive Chart Visualization
```jsx
// Interactive temperature chart with Recharts
<ResponsiveContainer width="100%" height={300}>
  <LineChart data={hourlyData}>
    <XAxis dataKey="time" tickFormatter={formatHour} />
    <YAxis domain={['dataMin - 2', 'dataMax + 2']} />
    <Tooltip formatter={formatTooltip} />
    <Line 
      type="monotone" 
      dataKey="temp" 
      stroke="#4d6fb3" 
      strokeWidth={2} 
      dot={{ r: 4 }} 
      activeDot={{ r: 6 }} 
    />
  </LineChart>
</ResponsiveContainer>
```

### Modern UI with Tailwind
```jsx
// Weather card component with Tailwind CSS
<div className="bg-white rounded-xl shadow-lg p-6 transition-all hover:shadow-xl">
  <div className="flex items-center justify-between">
    <div>
      <h2 className="text-2xl font-bold text-gray-800">{location}</h2>
      <p className="text-gray-600">{currentDate}</p>
    </div>
    <WeatherIcon code={weatherCode} size={64} />
  </div>
  <div className="mt-4">
    <p className="text-5xl font-bold">{temp}°C</p>
    <p className="text-gray-600 capitalize">{description}</p>
  </div>
</div>
```

## 🚀 Deployment

ClimaVision is configured for easy deployment on Netlify:

1. Push your code to a GitHub repository
2. Create a new site in Netlify and connect your repository
3. Add your OpenWeatherMap API key as environment variable
4. Deploy!

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start)

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a pull request

Please ensure your code follows the project's TypeScript style and includes appropriate tests.

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.

## ✉️ Contact

Oussama Abed - [@Oussamaabe](https://github.com/Oussamaabe)  
Project Link: [https://github.com/Oussamaabe/ClimaVision](https://github.com/Oussamaabe/ClimaVision)

---

**ClimaVision** - Crafted with React and TypeScript • Feb 2025 - April 2025  
*Real-time weather insights at your fingertips*
