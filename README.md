# 📍 Distance Finder Map Application

A modern, interactive web application that helps users calculate distances between their current location and various destinations. Built with **HTML5**, **Leaflet.js**, and **OpenStreetMap**.

## 🚀 Features

- **Real-time Location Tracking**: Automatically detects your current position using the browser's Geolocation API.
- **Interactive Map**: Visualizes your location, destination, and the route between them.
- **Quick Destinations**: One-click distance calculation to common landmarks:
  - 🍽️ Restaurants
  - 🏥 Hospitals
  - ✈️ Airports
  - 🌳 Parks
- **Custom Destinations**: Enter any coordinates (Latitude/Longitude) to calculate the distance to a specific spot.
- **Smart Calculations**:
  - Straight-line distance (km & miles)
  - Estimated driving distance & time
  - Estimated walking distance & time
- **Visual Feedback**: Color-coded markers and route lines for clear visualization.

## 🛠️ Technologies Used

- **HTML5/CSS3**: Core structure and responsive styling.
- **JavaScript (ES6+)**: Logic for distance calculations and UI interactivity.
- **Leaflet.js**: Open-source JavaScript library for mobile-friendly interactive maps.
- **OpenStreetMap**: Free, editable map data source.

## 📋 How to Use

1. **Allow Location Access**: When prompted, allow the browser to access your location.
2. **Choose a Destination**:
   - Click one of the **Quick Destination** buttons (e.g., "Nearest Restaurant").
   - OR enter custom coordinates in the **Custom Destination** section.
3. **View Results**:
   - The map will draw a route line.
   - The results panel will show the exact distance and estimated travel times.
4. **Clear/Reset**: Use the "Clear Route" button to start over or "Get My Current Location" to refresh your position.

## 🧮 How it Works

The application uses the **Haversine Formula** to calculate the great-circle distance between two points on a sphere given their longitudes and latitudes.

```javascript
// Simplified Haversine Formula
a = sin²(Δφ/2) + cos φ1 ⋅ cos φ2 ⋅ sin²(Δλ/2)
c = 2 ⋅ atan2( √a, √(1−a) )
d = R ⋅ c
```

## 📝 License

This project is open source and available for personal and educational use.
