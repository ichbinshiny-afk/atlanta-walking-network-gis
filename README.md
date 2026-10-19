# Atlanta Walking Network (Colab)

A beginner GIS/Python project that downloads Atlanta's walking street network with OSMnx, exports the road edges as an ESRI Shapefile, and plots them over a census geography layer with GeoPandas and Matplotlib.

## Notebook

Open `Untitled0.ipynb` in Google Colab or Jupyter.

## Input data

The visualization section expects the Atlanta census block-group Shapefile at `/content/tl_2025_13_bg.shp`. Upload the complete Shapefile set (`.shp`, `.shx`, `.dbf`, `.prj`, and related files) to Colab, or update the path in the notebook. The walking network is fetched from OpenStreetMap when the first section runs.

## Notes

- The notebook installs OSMnx, GeoPandas, Matplotlib, and Pillow.
- It checks/reprojects the census layer to the walking network CRS before plotting.
- This is an introductory data acquisition, format conversion, and visualization project; it does not calculate network centrality or other advanced network metrics.
