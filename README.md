# South Florida Venue Clustering (Data Science Capstone)

A data science capstone project that clusters South Florida neighborhoods by
venue type, in the style of the IBM Data Science Professional Certificate's
Applied Data Science Capstone.

## Approach

1. Build a zip code / neighborhood dataset for South Florida cities, geocoded
   with `geopy`/`geocoder`.
2. Pull nearby venue data for each neighborhood from the Foursquare Places API.
3. One-hot encode venue categories and group by neighborhood to find the
   top-10 most common venue types per area.
4. Cluster neighborhoods with K-Means based on venue-category frequency.
5. Visualize the resulting clusters on an interactive map with Folium.

## Contents

- `XinGuanCapstone.ipynb`, `XinGuanFinalProj.ipynb` — main analysis notebooks
- `CanadaPostCode*.ipynb` — geocoding utility notebooks (adapted from the
  course's Toronto example before being applied to South Florida)
- `SouthFloridaCommonVenueAnalysis.pptx` — presentation summary
- `report.txt` — written report

## Stack

Python, pandas, numpy, geopy/geocoder, Foursquare Places API,
scikit-learn (K-Means), Folium
