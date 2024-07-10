# Optimal Zones for Heat-averse, Dog-owning Swimmers in Vienna

## Project Overview

This project aims to identify optimal residential zones in Vienna for individuals who dislike heat, own dogs, and enjoy swimming. By leveraging geospatial data from the City of Vienna, we created a composite score that combines heat vulnerability, proximity to dog amenities, and proximity to swimming pools. The result is a detailed interactive map that highlights the best and worst areas based on these criteria.

## Methodology

### Data Sources

- **Heat Vulnerability Index**: Obtained from the City of Vienna's open data portal, this dataset provides a heat vulnerability score for various sub-districts within Vienna.
- **Dog Amenities**: Locations of dog waste bag dispensers (HUNDESACKERLOGD) sourced from the City's geospatial data services.
- **Swimming Pools**: Locations of public swimming pools (SCHWIMMBADOGD) also sourced from the City's geospatial data services.

### Data Processing

1. **Data Collection**: Data was fetched from the City of Vienna's WFS services and other relevant sources.
2. **Geospatial Transformation**: Ensured all datasets were in the same coordinate reference system (CRS) for accurate spatial analysis.
3. **Proximity Calculation**: Calculated the distance from the centroid of each sub-district to the nearest dog amenity and swimming pool.
4. **Normalization**: Used Min-Max scaling to normalize the proximity scores and the heat vulnerability index.
5. **Composite Scoring**: Combined the normalized scores into a composite score to rank each sub-district based on the three criteria.

### Visualization

The processed data was visualized using Plotly's `choropleth_mapbox` to create an interactive map. The map features:
- A heatmap showing the composite score of each sub-district.
- Hover functionality displaying detailed information about each area.
- Color scaling adjusted to highlight the best and worst zones more effectively.

## Results

The final map reveals that areas in the city center and some outlying regions offer the best living conditions for heat-averse, dog-owning swimmers. These areas are highlighted in green, indicating lower heat vulnerability, closer proximity to dog amenities, and swimming pools. Conversely, areas marked in red represent less optimal conditions.

## Applications

### For Individuals

- **Apartment Hunting**: Prospective residents can use this map to identify neighborhoods that best meet their lifestyle needs, particularly if they are sensitive to heat, own pets, and value access to recreational facilities.

### For Businesses

- **Real Estate Investments**: Real estate companies can leverage this data to make informed decisions about property development and marketing strategies.
- **Urban Planning**: Urban planners can use these insights to enhance city amenities, targeting improvements in areas that are less optimal.
- **Service Providers**: Businesses offering pet services, recreational facilities, or climate mitigation products can identify high-demand areas to target their services.

### For Policy Makers

- **Public Health**: The City of Vienna can use this data to allocate resources effectively, improving infrastructure in vulnerable areas.
- **Environmental Planning**: Insights from the heat vulnerability index can inform climate adaptation strategies to enhance urban resilience.

## Conclusion

This project demonstrates the power of geospatial data analysis in making informed decisions about urban living and planning. The City of Vienna's extensive open data resources provide valuable insights that can influence a wide range of decisions, from personal apartment hunting to strategic business planning and public policy formulation.

## Future Work

Expanding this project could involve incorporating additional datasets such as public transport accessibility, noise pollution levels, and other amenities to create a more comprehensive analysis. Additionally, similar methodologies could be applied to other cities using their respective open data portals.

## Acknowledgements

This project utilizes data provided by the City of Vienna's open data initiative, which offers extensive resources for various geospatial and non-geospatial datasets.

---

Feel free to use and adapt this analysis for your specific needs. The City of Vienna's data repository offers numerous opportunities for further exploration and innovation in geospatial data analysis.