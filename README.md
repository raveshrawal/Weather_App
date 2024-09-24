# Weather App

A simple Android weather application that allows users to search for the weather of any city using the OpenWeather API.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Integration](#api-integration)
- [Permissions](#permissions)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Weather App is an Android application that fetches real-time weather information for any city in the world using the OpenWeather API. The app is designed with a simple user interface where the user can input a city name and get details about the temperature, pressure, humidity, and more.

## Features

- Fetch real-time weather information using the [OpenWeather API](https://openweathermap.org/).
- Display information like temperature, feels like, maximum and minimum temperature, humidity, pressure, sea level, and ground level.
- Clean and simple UI design.
- Support for multiple cities around the world.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/raveshrawal/weather_app.git
    ```

2. Open the project in Android Studio.

3. Get your API key from [OpenWeather API](https://openweathermap.org/api) and replace `{Your API Token}` in the following line inside `MainActivity.java`:
    ```java
    url = "https://api.openweathermap.org/data/2.5/weather?q=" + city + "&appid={Your API Token}";
    ```

4. Build and run the project on an Android emulator or a physical device.

## Usage

1. On the app’s home screen, input the name of the city for which you want to fetch the weather.
2. Click the `Search` button.
3. The weather information, including temperature, humidity, and more, will be displayed in the center of the screen.

## API Integration

This app uses the [OpenWeather API](https://openweathermap.org/api) to fetch real-time weather data. You need to obtain an API key from their website.

To configure the API key:

1. Sign up on [OpenWeather](https://home.openweathermap.org/users/sign_up) and generate your API key.
2. In `MainActivity.java`, find the following line:
    ```java
    url = "https://api.openweathermap.org/data/2.5/weather?q=" + city + "&appid={Your API Token}";
    ```
3. Replace `{Your API Token}` with your actual API key.

## Permissions

This app requires the following permissions:

- `android.permission.INTERNET`: To make network requests to the OpenWeather API.

Add this permission in your `AndroidManifest.xml`:
```xml
<uses-permission android:name="android.permission.INTERNET"/>
```
## Screenshots

![image](https://github.com/user-attachments/assets/402c8af2-be25-4437-af47-aba0ec5a005c)


## Contributing

Contributions are welcome! If you'd like to improve this project, feel free to fork the repository and create a pull request.

1. Fork the project.
2. Create your feature branch: `git checkout -b feature/AmazingFeature`
3. Commit your changes: `git commit -m 'Add some AmazingFeature'`
4. Push to the branch: `git push origin feature/AmazingFeature`
5. Open a pull request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
