# Toronto Neighborhood Clustering

This project explores and segments neighborhoods in Toronto based on venue categories using clustering techniques. It utilizes data from Wikipedia, geospatial data, and the Foursquare API to group neighborhoods into clusters and visualize them on an interactive map.

## 🗺️ Project Objective

- Collect neighborhood-level data for Toronto.
- Retrieve geographical coordinates using geopy and CSV datasets.
- Use the Foursquare API to collect venue data.
- Analyze venue distribution by neighborhood.
- Apply **k-means clustering** to segment neighborhoods.
- Visualize the resulting clusters with **Folium**.

## 📦 Technologies Used

- **Python**
- **Pandas** for data handling
- **Geopy** for geocoding
- **Folium** for interactive maps
- **Scikit-learn** for clustering (k-means)
- **Foursquare API** for venue data
- **Matplotlib** for plotting

## 📊 Project Workflow

1. **Data Collection**
   - Scraped neighborhood data from Wikipedia.
   - Merged with latitude and longitude info from a CSV file.

2. **Data Cleaning**
   - Removed unassigned boroughs and merged duplicate postal codes.

3. **Venue Exploration**
   - Queried the Foursquare API to get nearby venues for each neighborhood.

4. **One-hot Encoding & Grouping**
   - One-hot encoded venue categories.
   - Calculated mean frequencies for each neighborhood.

5. **Clustering**
   - Applied k-means clustering to group neighborhoods based on venue similarity.

6. **Visualization**
   - Mapped clustered neighborhoods using **Folium** and color-coded clusters.

## 📍 Clustering Results

The neighborhoods in Toronto were segmented into **5 clusters**, each representing similar types of venues (e.g., coffee shops, parks, restaurants, etc.).

## 🔑 API Access

This project uses the **Foursquare API**. You will need a `CLIENT_ID` and `CLIENT_SECRET`. These credentials were omitted for privacy reasons.

## 📝 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/toronto-neighborhood-clustering.git
