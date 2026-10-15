# fsd
# 📍 Nearby Places Finder – Christ University Central Campus

A responsive web application that helps students discover nearby places around **Christ University Central Campus, Bengaluru**, using OpenStreetMap data. The application allows users to explore nearby facilities, search for places, filter by category, and select the campus front gate or back gate as their search location.

## 🌟 Features

- **Responsive Design:** Works on desktops, tablets, and mobile devices.
- **Interactive Search:** Search for nearby places by name.
- **Category Filtering:** Filter places by categories such as cafés, shops, pharmacies, and public transport.
- **Campus Gate Selection:** Choose the front gate or back gate as the search reference point.
- **Geolocation:** Use the browser's Geolocation API to find places near the user's current location, with permission.
- **OpenStreetMap Integration:** Retrieve nearby places using the Overpass API.
- **Dynamic Place Cards:** Display place information and links to OpenStreetMap.
- **Canvas Visualization:** Draw a simple schematic representation of nearby places.
- **Error Handling:** Display loading indicators, error messages, and empty-result states.
- **Fallback Data:** Show clearly labelled sample entries if the API request fails.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Semantic webpage structure |
| Tailwind CSS | Responsive styling and layout |
| JavaScript | Interactivity and application logic |
| OpenStreetMap | Open geographic data |
| Overpass API | Retrieve nearby place information |
| Fetch API | Send HTTP requests and retrieve data |
| JSON | Process API responses |
| Geolocation API | Access the user's location |
| Canvas API | Draw a simple location schematic |
| Flexbox | Create flexible navigation and layouts |

## 📂 Project Structure

```text
nearby-places-finder/
├── index.html          # Main webpage and application logic
├── campus-hero.png     # Hero image used on the webpage
└── README.md           # Project documentation
```

> **Note:** Keep `campus-hero.png` in the same folder as `index.html`. If you use a different image filename, update the image path in the HTML file.

## 🚀 Getting Started

### Prerequisites

- A modern web browser, such as Google Chrome or Microsoft Edge.
- An internet connection to load Tailwind CSS and retrieve OpenStreetMap data.
- Visual Studio Code (recommended).
- The Live Server extension for Visual Studio Code (recommended).

### Installation and Setup

1. Clone or download this repository.

   ```bash
   git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
   ```

2. Open the project folder in Visual Studio Code.

3. Ensure that `index.html` and `campus-hero.png` are in the same folder.

4. Install the **Live Server** extension if it is not already installed.

5. Right-click `index.html` and select **Open with Live Server**.

6. Open the webpage in your browser and allow location access if you want to use the current-location feature.

## ⚙️ How It Works

1. The user selects the campus front gate, back gate, or current location.
2. JavaScript sends a request to the Overpass API using the Fetch API.
3. The API returns nearby place information in JSON format.
4. JavaScript processes the response and displays the results as place cards.
5. The user can search for a place, filter results by category, or open a place's OpenStreetMap link.

If an API request fails, the application can display sample fallback entries. These entries are clearly marked as demo data and should not be treated as verified real-world locations.

## 🖥️ Application Interface

The application includes:

- **Hero Section:** Introduces the nearby-places finder and displays the campus image.
- **Search and Filters:** Help users find relevant results.
- **Nearby Places Section:** Displays retrieved places as cards.
- **Canvas Schematic:** Provides a simple visual representation of nearby places.
- **Status Messages:** Communicate loading progress, errors, and empty results.

## 🔌 API and Data Source

**OpenStreetMap (OSM)**  
Provides open geographic data about places and facilities.

Website: https://www.openstreetmap.org/

**Overpass API**  
Queries OpenStreetMap data based on geographic coordinates and map tags.

Website: https://overpass-api.de/

The availability and completeness of results depend on OpenStreetMap coverage, API availability, search radius, and network connectivity.

## ⚠️ Limitations

- Search results depend on the information available in OpenStreetMap.
- The Overpass API may occasionally be slow, unavailable, or rate-limited.
- Campus gate coordinates are approximate and may need adjustment.
- The Canvas visualization is a schematic, not a live navigable map.
- The search feature filters the places already retrieved; it is not a global place-search or geocoding service.
- Fallback entries are demonstration data, not verified locations.
- Geolocation requires user permission and may require a secure context, such as HTTPS or localhost.

## 🔮 Future Improvements

- Add a real interactive map using Leaflet and OpenStreetMap tiles.
- Implement location-name search using a geocoding service.
- Add distance calculations and sorting by nearest place.
- Provide directions from the selected campus gate.
- Improve accessibility and keyboard navigation.
- Add caching and more robust API error handling.

## 🎓 Project Purpose

This project demonstrates the application of front-end web development concepts, responsive UI/UX design, JavaScript events, REST-style API requests, JSON processing, browser geolocation, and Canvas drawing.

It also explores ways to make OpenStreetMap data easier to discover and use through a more accessible and interactive interface.

## 📜 Credits

- Map data: [OpenStreetMap contributors](https://www.openstreetmap.org/copyright)
- Nearby place queries: [Overpass API](https://overpass-api.de/)
- Styling: [Tailwind CSS](https://tailwindcss.com/)

## 📄 License

This project is intended for educational and demonstration purposes. If you publish or redistribute it, add a suitable license and follow the attribution and licensing requirements of the data and other assets you use.
