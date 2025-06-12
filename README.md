# 🌤 Weather API App

This project is a Python desktop application built with PyQt5, designed to fetch and display real-time weather data using the OpenWeatherMap API. It features a clean, user-friendly GUI and provides intuitive visual feedback through emojis representing weather conditions.

## 🚀 What I Built

Created a weather application that allows users to enter a city name and instantly retrieve the current temperature (in Fahrenheit), weather conditions, and corresponding emoji visuals.

### Main Components:

* **Graphical User Interface (GUI)**: Built using PyQt5, featuring labels, input fields, and buttons.
* **API Integration**: Connected the app to OpenWeatherMap API to fetch real-time weather data.
* **Error Handling**: Implemented robust error handling for network issues, incorrect city names, and API errors.
* **Emoji Visuals**: Added emojis to enhance user experience by visually representing weather conditions clearly and instantly.

## 🛠 How the Code Works

The application is organized into several parts:

### 1. **GUI Setup**

The GUI is created using PyQt5 widgets:

* `QLabel` for displaying text and emojis.
* `QLineEdit` for user input (city name).
* `QPushButton` for triggering the weather data retrieval.
* `QVBoxLayout` for vertically stacking GUI elements neatly.

### 2. **Weather Data Retrieval**

Upon entering a city and clicking the "Get Weather" button:

* The app constructs an HTTP GET request to OpenWeatherMap API.
* API returns JSON data containing temperature, weather conditions, and IDs.

### 3. **Data Parsing and Display**

* Temperature data is converted from Kelvin to Fahrenheit.
* Weather conditions are mapped to corresponding emojis via predefined ID ranges.
* The GUI labels are dynamically updated with temperature, emoji, and descriptive text.

### 4. **Comprehensive Error Handling**

The app gracefully handles various potential issues, including:

* HTTP errors (e.g., 404 for city not found, 401 for invalid API keys).
* Network issues (timeouts, connection errors).
* General request exceptions, providing clear and helpful feedback to the user.

## 📚 Technologies Used

* **Python 3.x**: Main programming language.
* **PyQt5**: Framework for creating the graphical user interface.
* **Requests**: HTTP library for making API calls.

## ⚡ How to Run

Follow these steps to run the application:

### Step 1: Clone the repository

```
git clone https://github.com/esarkisyan/weather-api-app.git
cd weather-api-app
```

### Step 2: Install dependencies

```
pip install PyQt5 requests
```

### Step 3: Set your API Key

* Open `main.py` and find:

```python
api_key = " "
```

* Replace the blank space with your personal API key from [OpenWeatherMap](https://openweathermap.org/api).

### Step 4: Launch the application

```
python main.py
```

## 📋 Requirements

* Python 3.x
* PyQt5
* requests

## 🎯 Key Learning Points

Completing this project taught me:

* Integrating external APIs into a Python application.
* Building responsive GUI apps using PyQt5.
* Effectively handling exceptions and errors.
* Enhancing user experience with simple UI improvements like emoji visuals.
