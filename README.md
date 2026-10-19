# Atlanta Walking Network (Colab)

A beginner GIS/Python project that downloads Atlanta's walking street network with OSMnx, exports the road edges as an ESRI Shapefile, and plots them over a census geography layer with GeoPandas and Matplotlib.

## Projects

- **Atlanta walking network:** Open `Untitled0.ipynb` in Google Colab or Jupyter.
- **Kyung Hee study cafe map:** See [the interactive map source](gyeonghee-cafe-guide.html) and [feature/setup notes](CAFE_GUIDE.md).

## Input data for the Colab notebook

The visualization section expects the Atlanta census block-group Shapefile at `/content/tl_2025_13_bg.shp`. Upload the complete Shapefile set (`.shp`, `.shx`, `.dbf`, `.prj`, and related files) to Colab, or update the path in the notebook. The walking network is fetched from OpenStreetMap when the first section runs.

## Notes

- The notebook installs OSMnx, GeoPandas, Matplotlib, and Pillow.
- It checks/reprojects the census layer to the walking network CRS before plotting.
- The notebook demonstrates data acquisition, format conversion, and visualization; it does not calculate network centrality or other advanced network metrics.
- The cafe map uses the Tmap Vector JS SDK and pedestrian-routing API. Insert your own restricted Tmap key locally before running it; the public HTML contains placeholders only.
