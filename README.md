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

### Core Features
- Load multiple GeoJSON files via file upload or drag-and-drop
- Interactive map with pan and zoom capabilities
- Style customization (colors, point sizes, line widths)
- Layer management with visibility toggles
- Feature information display on click
- Multiple basemap options (OpenStreetMap, Satellite, Dark, Topographic)
- Feature count tracking
- Copy feature properties as JSON
- Responsive design that works on desktop and mobile devices

### Advanced Features
- **Table View**: Browse and search feature properties in a tabular format
- **Feature Selection**: Select features in the table and highlight them on the map
- **Import/Export**: Import GeoJSON from text, clipboard, or URL; export selected layers
- **Large File Handling**: Smart handling of large files with sampling options
- **Dark/Light Mode**: Toggle between dark and light themes
- **Layer Editing**: Rename layers, adjust styling, and view layer statistics
- **Feature Details**: Examine individual features with detailed property views
- **Copy to New Layer**: Create new layers from selected features
- **Smart Filtering**: Filter features by layer or search across all properties
- **Layer Duplication**: Create copies of existing layers
- **Context Menu**: Right-click on features in the table for additional options

## Example Data

The repository includes several example GeoJSON files in the `examples` directory that you can use to test Layercake:

- `africa.geojson` - Boundary data for the African continent
- `ne_10m_reefs.geojson` - Global reef locations at 1:10m scale
- `ne_50m_populated_places.geojson` - Major populated places around the world
- `ne_50m_urban_areas.geojson` - Urban area boundaries at 1:50m scale

These files are from public domain sources:
- Africa data from [geojson-regions](https://github.com/AshKyd/geojson-regions)
- Natural Earth data from [geojson.xyz](https://geojson.xyz/)

## How to Use Layercake

### Map View
1. **Load Data**: 
   - Click "Select file(s)" to upload GeoJSON files
   - Or drag and drop GeoJSON files directly onto the map
   - Try with the example files in the `examples` directory

2. **Manage Layers**:
   - Toggle layer visibility with the checkbox
   - Change layer colors with the color picker
   - Adjust point sizes and line widths with sliders
   - Click layer names to zoom to that layer
   - Click the pencil icon to edit layer properties
   - Remove individual layers with the × button
   - Use the "Reset Map" button to remove all layers

3. **Change Basemap**:
   - Select different map styles from the "Base Map" dropdown

4. **View Feature Information**:
   - Click on any feature to see its properties
   - Use the "Copy Properties" button to copy data as JSON

5. **Theme Toggle**:
   - Switch between dark and light modes using the toggle in the top-right corner

### Table View
1. **Browse Features**:
   - View all features in a tabular format
   - Filter by layer using the dropdown
   - Search across all properties
   - Click on rows to highlight features on the map
   - Right-click on rows to access the context menu

2. **Select Features**:
   - Use checkboxes to select individual features
   - Use "Select All" or "Select None" buttons
   - Click "Map Selected" to highlight selected features on the map
   - Click "Copy to New Layer" to create a new layer from selected features

3. **Reset Filters**:
   - Clear all search and layer filters with the "Reset Filters" button

### I/O View
1. **Import GeoJSON**:
   - Paste GeoJSON text directly
   - Import from clipboard
   - Fetch from a URL
   - Upload files via drag and drop

2. **Export GeoJSON**:
   - Select layers to export
   - Choose between merged or separate files
   - Toggle pretty printing for formatted JSON
   - Copy to clipboard or download as files

## Performance Features
- Virtualized table for handling large datasets efficiently
- Smart sampling for extremely large files
- Warning dialogs for potentially problematic files
- Optimized rendering for smooth performance
- Memory-efficient handling of large feature collections

## How It Was Made

Layercake was built using:

- **HTML/CSS/JavaScript**: Core web technologies for the interface
- **Leaflet.js**: Open-source JavaScript library for interactive maps
- **No build process**: Single HTML file with embedded CSS and JavaScript for maximum portability

The application is designed to be lightweight and dependency-free, making it easy to host anywhere or run locally.

## Getting Started

Simply open `layercake.html` in any modern web browser. No installation, server, or internet connection required (except for loading basemaps).

## Contributing

Want to help make Layercake better? Check out our [development roadmap](TODO.md) and pick something that looks interesting. 

No need to be an expert - we welcome contributions from everyone.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
