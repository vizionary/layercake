# Layercake

A simple, serverless GeoJSON viewer that runs entirely in your browser.

## What is Layercake?

Layercake is a lightweight web application that allows you to visualize and interact with GeoJSON files directly in your browser without requiring any server-side processing. It's designed to be simple, fast, and privacy-focused - your data never leaves your computer.

## Why We Made It

We created Layercake to solve common challenges when working with geospatial data:

- **Quick Visualization**: Instantly view GeoJSON files without installing GIS software
- **Easy Comparison**: Load multiple layers and compare different datasets
- **No Server Required**: Works entirely client-side, preserving data privacy
- **Accessibility**: Available to anyone with a web browser, no technical setup needed

## Features

- Load multiple GeoJSON files via file upload or drag-and-drop
- Interactive map with pan and zoom capabilities
- Style customization (colors, point sizes, line widths)
- Layer management with visibility toggles
- Feature information display on click
- Multiple basemap options (OpenStreetMap, Satellite, Dark, Topographic)
- Feature count tracking
- Copy feature properties as JSON
- Responsive design that works on desktop and mobile devices

## How to Use Layercake

1. **Load Data**: 
   - Click "Select file(s)" to upload GeoJSON files
   - Or drag and drop GeoJSON files directly onto the map

2. **Manage Layers**:
   - Toggle layer visibility with the checkbox
   - Change layer colors with the color picker
   - Adjust point sizes and line widths with sliders
   - Click layer names to zoom to that layer
   - Remove individual layers with the × button
   - Use the "Reset Map" button to remove all layers

3. **Change Basemap**:
   - Select different map styles from the "Base Map" dropdown

4. **View Feature Information**:
   - Click on any feature to see its properties
   - Use the "Copy Properties" button to copy data as JSON

## How It Was Made

Layercake was built using:

- **HTML/CSS/JavaScript**: Core web technologies for the interface
- **Leaflet.js**: Open-source JavaScript library for interactive maps
- **No build process**: Single HTML file with embedded CSS and JavaScript for maximum portability

The application is designed to be lightweight and dependency-free, making it easy to host anywhere or run locally.

## Getting Started

Simply open `layercake.html` in any modern web browser. No installation, server, or internet connection required (except for loading basemaps).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
