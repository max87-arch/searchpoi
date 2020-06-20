# Search Poi using Overpass API
This repository contains the searchpoi python package.
This package allow you to find closest Point of Interests around a Point.

## Getting Started

Before proceeding, you need to install the package.

```bash
pip3 install searchpoi
```

Now, you can use the package as follow:
```python
from searchpoi import SearchPoi

poi = SearchPoi("Salt Lake City")
lat = 40.758701
lon = -111.876183
distance_of_buffer = 1 #km

summary_closest_points = poi.closest(lon, lat, distance_of_buffer)

print(poi.gdf) # this attribute contains the geopandas dataframe with Points of interest and their geometry
```

## License
This code is release under [MIT License](LICENSE).