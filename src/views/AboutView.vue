<template>
  <div class="weather-container" :style="{ backgroundImage: 'url(' + backgroundImage + ')' }">
    <h1>Weather Information</h1>
    <div>
      <input v-model="city" @keyup.enter="fetchWeather" type="text" placeholder="Enter city name" class="search-input" />
      <button @click="fetchWeather" class="search-button">Search</button>
    </div>
    <div v-if="weatherData" class="weather-info">
      <p><strong>Location:</strong> {{ weatherData.name }}</p>
      <p><strong>Temperature:</strong> {{ kelvinToCelsius(weatherData.main.temp) }}°C</p>
      <p><strong>Weather:</strong> {{ weatherData.weather[0].description }}</p>
      <p><strong>Humidity:</strong> {{ weatherData.main.humidity }}%</p>
      <p><strong>Wind Speed:</strong> {{ weatherData.wind.speed }} m/s</p>
      <img v-bind:src="'http://openweathermap.org/img/w/' + weatherData.weather[0].icon + '.png'" alt="Weather icon" />
    </div>
    <div v-else-if="error">
      <p>Error: {{ error }}</p>
    </div>
    <div v-else>
      <p>Loading weather data...</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'WeatherComponent',
  data() {
    return {
      city: '',
      weatherData: null,
      error: null,
      backgroundImage: ''
    }
  },
  methods: {
    kelvinToCelsius(kelvin) {
      return (kelvin - 273.15).toFixed(2)
    },
    async fetchWeather() {
      const apiKey = '9366909a0b127f05b3f2dc4cb3d32580'

      if (!this.city) {
        this.error = 'Please enter a city name.'
        return
      }

      try {
        const response = await fetch(
          `https://api.openweathermap.org/data/2.5/weather?q=${this.city}&appid=${apiKey}`
        )

        if (!response.ok) {
          throw new Error('City not found.')
        }

        const data = await response.json()
        this.weatherData = data
        this.error = null
        this.setBackgroundImage(data.weather[0].main)
      } catch (error) {
        this.error = error.message
        this.weatherData = null
        console.error('Error fetching weather:', error)
      }
    },
    setBackgroundImage(condition) {
      if (condition === 'Clear') {
        this.backgroundImage = '/src/assets/images/sunny.jpg'
      } else if (condition === 'Rain') {
        this.backgroundImage = '/src/assets/images/rainy.avif'
      } else if (condition === 'Clouds') {
        this.backgroundImage = '/src/assets/images/cloudy.avif'
      } else if (condition === 'Snow') {
        this.backgroundImage = '/src/assets/images/snowy.jpg'
      } else if (condition === 'Thunderstorm') {
        this.backgroundImage = '/src/assets/images/thunderstorm.jpg'
      } else {
        this.backgroundImage = '/src/assets/images/default.jpg'
      }
    }
  }
}
</script>

<style scoped>
.weather-container {
  text-align: center;

  padding: 0;
  background-size: cover;
  background-position: top center;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: white;
  transition: background-image 0.3s ease;
  background-attachment: fixed;
}

h1 {
  font-size: 3rem;
  margin-bottom: 20px;
}

.search-input {
  padding: 10px;
  margin-right: 10px;
  font-size: 16px;
  margin-bottom: 20px;
}

.search-button {
  padding: 10px 20px;
  font-size: 16px;
  cursor: pointer;
  margin-bottom: 20px;
}

.weather-info {
  background-color: white;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  max-width: 500px;
  margin-top: 20px;
  color: #333;
}

.weather-info p {
  font-size: 1.2rem;
  margin: 10px 0;
}

strong {
  font-weight: bold;
}

.error-message {
  color: red;
}

img {
  margin-top: 10px;
  width: 100px;
  margin-bottom: 20px;
}
</style>
