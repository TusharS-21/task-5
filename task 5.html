<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Weather Dashboard</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        .weather-card {
            transition: all 0.3s ease;
        }
        .weather-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        .sunny-bg {
            background: linear-gradient(135deg, #f6d365 0%, #fda085 100%);
        }
        .rainy-bg {
            background: linear-gradient(135deg, #4b79cf 0%, #283e51 100%);
        }
        .cloudy-bg {
            background: linear-gradient(135deg, #bdc3c7 0%, #2c3e50 100%);
        }
        .default-bg {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        #searchInput:focus {
            outline: none;
            box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.5);
        }
        .loader {
            border: 3px solid #f3f3f3;
            border-top: 3px solid #3498db;
            border-radius: 50%;
            width: 30px;
            height: 30px;
            animation: spin 1s linear infinite;
        }
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
    </style>
</head>
<body class="min-h-screen bg-gray-100">
    <div class="container mx-auto px-4 py-8">
        <div class="max-w-4xl mx-auto">
            <header class="text-center mb-8">
                <h1 class="text-4xl font-bold text-gray-800 mb-2">Weather Dashboard</h1>
                <p class="text-gray-600">Current weather conditions at your location</p>
            </header>

            <div class="flex flex-col md:flex-row gap-4 mb-8">
                <div class="flex-1">
                    <div class="relative">
                        <input 
                            type="text" 
                            id="searchInput" 
                            placeholder="Enter city name..." 
                            class="w-full px-4 py-2 rounded-lg border border-gray-300 focus:ring-blue-500 focus:border-blue-500"
                        >
                        <button 
                            id="searchBtn" 
                            class="absolute right-2 top-1/2 transform -translate-y-1/2 bg-blue-500 text-white px-4 py-1 rounded-md hover:bg-blue-600 transition"
                        >
                            Search
                        </button>
                    </div>
                </div>
                <div class="flex-1 flex justify-center md:justify-end items-center">
                    <button 
                        id="locationBtn"
                        class="w-full md:w-auto bg-green-500 hover:bg-green-600 text-white px-4 py-2 rounded-lg transition flex items-center justify-center gap-2"
                    >
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M5.05 4.05a7 7 0 119.9 9.9L10 18.9l-4.95-4.95a7 7 0 010-9.9zM10 11a1 1 0 100-2 1 1 0 000 2z" clip-rule="evenodd" />
                        </svg>
                        Use My Location
                    </button>
                </div>
            </div>

            <div id="currentWeather" class="rounded-xl shadow-md overflow-hidden mb-8 default-bg text-white">
                <div class="flex flex-col md:flex-row">
                    <div class="md:w-1/2 p-6 flex flex-col justify-between">
                        <div>
                            <h2 class="text-2xl font-semibold mb-2" id="currentLocation">Detecting your location...</h2>
                            <p class="text-lg mb-4" id="currentDate"></p>
                        </div>
                        <div class="flex items-center">
                            <div id="currentWeatherIcon" class="text-8xl">⏳</div>
                            <div class="ml-4">
                                <div class="text-5xl font-bold" id="currentTemp">--°</div>
                                <div class="text-xl" id="currentCondition">Loading...</div>
                            </div>
                        </div>
                    </div>
                    <div class="md:w-1/2 p-6 bg-black bg-opacity-20 flex flex-col justify-center">
                        <div class="grid grid-cols-2 gap-4">
                            <div class="bg-white bg-opacity-10 p-4 rounded-lg">
                                <div class="text-sm opacity-80">Humidity</div>
                                <div class="text-xl font-semibold" id="humidity">--%</div>
                            </div>
                            <div class="bg-white bg-opacity-10 p-4 rounded-lg">
                                <div class="text-sm opacity-80">Wind Speed</div>
                                <div class="text-xl font-semibold" id="windSpeed">-- km/h</div>
                            </div>
                            <div class="bg-white bg-opacity-10 p-4 rounded-lg">
                                <div class="text-sm opacity-80">Feels Like</div>
                                <div class="text-xl font-semibold" id="feelsLike">--°</div>
                            </div>
                            <div class="bg-white bg-opacity-10 p-4 rounded-lg">
                                <div class="text-sm opacity-80">Visibility</div>
                                <div class="text-xl font-semibold" id="visibility">-- km</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <h3 class="text-2xl font-semibold text-gray-800 mb-4">5-Day Forecast</h3>
            <div id="forecastContainer" class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-5 gap-4 mb-8">
                <!-- Forecast cards will be inserted here dynamically -->
                <div class="col-span-full flex justify-center py-10" id="loadingForecast">
                    <div class="loader"></div>
                </div>
            </div>

            <div class="bg-white rounded-lg shadow-md p-6">
                <h3 class="text-xl font-semibold text-gray-800 mb-4">About This Application</h3>
                <p class="text-gray-600 mb-4">
                    This weather dashboard provides real-time weather information using your device's location or any city you search for. 
                    The application would connect to a weather API (like OpenWeatherMap) to fetch accurate weather data.
                </p>
                <p class="text-gray-600">
                    Note: Currently displaying placeholder data. To implement this with a real API, you would need to:
                </p>
                <ul class="list-disc list-inside text-gray-600 mt-2 space-y-1">
                    <li>Sign up for a weather API service</li>
                    <li>Replace the placeholder endpoints with real API calls</li>
                    <li>Handle API responses and errors appropriately</li>
                </ul>
            </div>
        </div>
    </div>

    <script>
        // DOM Elements
        const searchInput = document.getElementById('searchInput');
        const searchBtn = document.getElementById('searchBtn');
        const locationBtn = document.getElementById('locationBtn');
        const currentLocation = document.getElementById('currentLocation');
        const currentDate = document.getElementById('currentDate');
        const currentTemp = document.getElementById('currentTemp');
        const currentCondition = document.getElementById('currentCondition');
        const currentWeatherIcon = document.getElementById('currentWeatherIcon');
        const humidity = document.getElementById('humidity');
        const windSpeed = document.getElementById('windSpeed');
        const feelsLike = document.getElementById('feelsLike');
        const visibility = document.getElementById('visibility');
        const forecastContainer = document.getElementById('forecastContainer');
        const loadingForecast = document.getElementById('loadingForecast');
        const currentWeather = document.getElementById('currentWeather');

        // Initialize with random weather data (would be replaced with API calls)
        function initWeather() {
            // Set current date
            const now = new Date();
            const options = { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric' };
            currentDate.textContent = now.toLocaleDateString('en-US', options);
            
            // Simulate API call delay
            setTimeout(() => {
                simulateWeatherData('current');
                simulateWeatherData('forecast');
            }, 1500);
        }

        // Simulate weather data (would be replaced with actual API call)
        function simulateWeatherData(type) {
            if (type === 'current') {
                const conditions = ['Sunny', 'Partly Cloudy', 'Cloudy', 'Rainy', 'Thunderstorm', 'Snowy'];
                const weather = conditions[Math.floor(Math.random() * conditions.length)];
                
                currentLocation.textContent = 'New York, US';
                currentTemp.textContent = `${Math.round(Math.random() * 20 + 15)}°C`;
                currentCondition.textContent = weather;
                humidity.textContent = `${Math.round(Math.random() * 50 + 30)}%`;
                windSpeed.textContent = `${Math.round(Math.random() * 30 + 5)} km/h`;
                feelsLike.textContent = `${Math.round(Math.random() * 20 + 10)}°C`;
                visibility.textContent = `${Math.round(Math.random() * 10 + 5)} km`;
                
                // Set weather icon
                setWeatherIcon(weather.toLowerCase());
                
                // Set background based on weather
                updateWeatherBackground(weather.toLowerCase());
                
            } else if (type === 'forecast') {
                loadingForecast.classList.add('hidden');
                
                // Generate 5-day forecast
                const days = ['Sun', 'Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat'];
                const forecastData = [];
                const now = new Date();
                
                for (let i = 1; i <= 5; i++) {
                    const nextDay = new Date(now);
                    nextDay.setDate(now.getDate() + i);
                    const dayName = days[nextDay.getDay()];
                    
                    forecastData.push({
                        day: dayName,
                        temp: `${Math.round(Math.random() * 15 + 10)}°`,
                        condition: ['Sunny', 'Partly Cloudy', 'Cloudy', 'Rainy', 'Thunderstorm', 'Snowy'][Math.floor(Math.random() * 6)],
                        icon: ['☀️', '⛅', '☁️', '🌧️', '⛈️', '❄️'][Math.floor(Math.random() * 6)]
                    });
                }
                
                // Populate forecast cards
                forecastContainer.innerHTML = '';
                forecastData.forEach(item => {
                    const forecastCard = document.createElement('div');
                    forecastCard.className = 'weather-card bg-white rounded-lg shadow-md overflow-hidden';
                    forecastCard.innerHTML = `
                        <div class="p-4 text-center">
                            <div class="font-semibold text-gray-800">${item.day}</div>
                            <div class="text-4xl my-3">${item.icon}</div>
                            <div class="text-gray-600">${item.condition}</div>
                            <div class="text-xl font-bold mt-2">${item.temp}</div>
                        </div>
                    `;
                    forecastContainer.appendChild(forecastCard);
                });
            }
        }

        // Set weather icon based on condition
        function setWeatherIcon(weather) {
            const icons = {
                'sunny': '☀️',
                'partly cloudy': '⛅',
                'cloudy': '☁️',
                'rainy': '🌧️',
                'thunderstorm': '⛈️',
                'snowy': '❄️'
            };
            currentWeatherIcon.textContent = icons[weather] || '☀️';
        }

        // Update weather background based on condition
        function updateWeatherBackground(weather) {
            // Remove all weather classes
            currentWeather.classList.remove(
                'sunny-bg', 'rainy-bg', 'cloudy-bg', 'default-bg'
            );
            
            // Add appropriate class
            if (weather.includes('sunny')) {
                currentWeather.classList.add('sunny-bg');
            } else if (weather.includes('rain') || weather.includes('thunderstorm')) {
                currentWeather.classList.add('rainy-bg');
            } else if (weather.includes('cloud')) {
                currentWeather.classList.add('cloudy-bg');
            } else {
                currentWeather.classList.add('default-bg');
            }
        }

        // Event listeners
        searchBtn.addEventListener('click', () => {
            if (searchInput.value.trim()) {
                loadingForecast.classList.remove('hidden');
                currentLocation.textContent = `Searching for ${searchInput.value}`;
                setTimeout(() => {
                    simulateWeatherData('current');
                    simulateWeatherData('forecast');
                }, 2000);
            }
        });

        locationBtn.addEventListener('click', () => {
            loadingForecast.classList.remove('hidden');
            currentLocation.textContent = 'Detecting your location...';
            
            // Simulate geolocation (in real app, this would use navigator.geolocation)
            setTimeout(() => {
                simulateWeatherData('current');
                simulateWeatherData('forecast');
            }, 2000);
        });

        // Search on Enter key
        searchInput.addEventListener('keypress', (e) => {
            if (e.key === 'Enter') {
                searchBtn.click();
            }
        });

        // Initialize
        document.addEventListener('DOMContentLoaded', initWeather);
    </script>
</body>
</html>
