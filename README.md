# CAT9 React Weather

A weather application that displays the current weather and hourly forecasts based on your current geolocation.

Based on [react-weather-standard](https://github.com/drminnaar/react-weather-standard)

Live demo **[cat9 Weather](http://demo.christrees.com/react-weather/)** for live demo of [react-weather](https://github.com/christrees/react-weather).

The weather application is composed of the following components:

* Header - A heading that displays application title

* WeatherDashboard - The primary (root) component that manages state for all underlying components. It is also responsibly for connecting to and retrieving data from a weather and geolocation service.

* CurrentWeatherDisplay - Displays weather information for the current point in time based on current location.

* HourlyWeatherDisplay - Displays a 24 hour weather forecast in the form of a scrollable carousel.

* HourlyWeatherForecastCard  - Displays weather summary for a given hour

The following services are used to obtain weather and location data:

* WeatherService - A wrapper that is responsible for integrating with the [OpenWeather Api]. It provides an interface that allows one to obtain current weather, daily forecast, and hourly forecast information.

* GeolocationService - A wrapper that is responsible for integrating with the [Google Geolocation API]. It provide an interface that allows one to obtain the current GPS coordinates. These coordinates are used by the _WeatherService_ to obtain weather information.

Features:

* Display current weather
* Display 24 hour weather forecast

This project also demonstrates:

* a typcial React project layout structure
* babel setup and configuration
* webpack setup and configuration
  * dotenv setup included
* Third party React component integration using _'[React Owl Carousel 2]'_
* eslint setup and configuration
* SCSS setup and configuration
* [OpenWeather API] integration
* [Google Geolocation API] integration

---

## Developed With

* [Visual Studio Code](https://code.visualstudio.com/) - A source code editor developed by Microsoft for Windows, Linux and macOS. It includes support for debugging, embedded Git control, syntax highlighting, intelligent code completion, snippets, and code refactoring
* [Node.js](https://nodejs.org/en/) - Javascript runtime
* [React](https://reactjs.org/) - A javascript library for building user interfaces
* [Babel](https://babeljs.io/) - A transpiler for javascript
* [Webpack](https://webpack.js.org/) - A module bundler
* [SCSS](http://sass-lang.com/) - A css metalanguage
* [Bootstrap 4](https://getbootstrap.com/) - Bootstrap is an open source toolkit for developing with HTML, CSS, and JS
* [Axios](https://github.com/axios/axios) - Promise based HTTP client for the browser and node.js
* [OpenWeather API] - Provides weather information
* [Google Geolocation API] - Provides geolocation information
* [React Owl Carousel 2] - A third party react carousel component
* [Surge] - Static web publishing for Front-End Developers

---

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

The following software is required to be installed on your system:

* Node 8.x
* Npm 3.x

Type the following commands in the terminal to verify your node and npm versions

```bash
node -v
npm -v
```

### Install

Follow the following steps to get development environment running.

* Clone _'react-weather'_ repository from GitHub

  ```bash
  git clone https://github.com/christrees/react-weather.git
  ```

   _OR USING SSH_

  ```bash
  git clone git@github.com:christrees/react-weather.git
  ```

* Install node modules

   ```bash
   cd react-weather
   npm install
   ```

Before continuing, the following steps are required:

1. Get API keys

   * OpenWeather API

     Have a look at [OpenWeather API](http://openweathermap.org/api)

     Get an API key [here](http://openweathermap.org/appid)

   * Google Geolocation API

     Have a look at [Google Geolocation API]

     Get an API key [here](https://developers.google.com/maps/documentation/geolocation/get-api-key)

1. Setup envrionment variables

   One is required to setup a few envrionment variables that are used by the _WeatherService_ and _GeolocationService_ to authenticate against external API's.

   Please follow the following steps:

   * Add _'.env'_ file

     Create a file called _'.env'_ at the root of the application

   * Add environment variables to _'.env'_ file

     GOOGLE_GEOLOCATION_API_KEY=YOUR_API_KEY_GOES_HERE
     OPEN_WEATHER_API_KEY=YOUR_API_KEY_GOES_HERE

   For more information about _'.env'_, please visit [dotenv-webpack](https://www.npmjs.com/package/dotenv-webpack)

### Build

* Build application

  This command will also run ESLint as part of build process.

  ```bash
  npm run build
  ```

* Build application and start watching for changes

  This command will also run ESLint as part of build process.

  ```bash
  npm run build:watch
  ```

### Run ESlint

* Lint project using ESLint

  ```bash
  npm run lint
  ```

* Lint project using ESLint, and autofix

  ```bash
  npm run lint:fix
  ```

### Run

* Run start

  This will run the _'serve'_ npm task

  ```bash
  npm start
  ```

* Run webpack dev server

  ```bash
  npm run serve:dev
  ```

* Alternatively run live-server (simple development http server with live reload capability)

  ```bash
  npm run serve
  ```

---

## Versioning

[SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/drminnaar/react-weather-standard/tags).

## Authors

* **Douglas Minnaar** - *Initial work* - [drminnaar](https://github.com/drminnaar)
* **Chris Trees** - *minor api and ui mods* - [christrees](https://github.com/christrees)

[OpenWeather API]: http://openweathermap.org
[Google Geolocation API]: https://developers.google.com/maps/documentation/geolocation/intro
[Surge]: https://surge.sh/
[React Owl Carousel 2]: https://github.com/florinn/react-owl-carousel2
[react-starter]: https://github.com/drminnaar/react-starter
[react-clicker]: https://github.com/drminnaar/react-clicker
[react-clock-basic]: https://github.com/drminnaar/react-clock-basic
[react-timer-basic]: https://github.com/drminnaar/react-timer-basic
[react-timer-advanced]: https://github.com/drminnaar/react-timer-advanced
[react-masterminds]: https://github.com/drminnaar/react-masterminds
[react-movie-cards]: https://github.com/drminnaar/react-movie-cards
[react-calculator-standard]: https://github.com/drminnaar/react-calculator-standard
[react-bitcoin-monitor]: https://github.com/drminnaar/react-bitcoin-monitor
[react-weather-standard]: https://github.com/drminnaar/react-weather-standard