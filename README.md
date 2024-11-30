# land-cover-classifications-for-Kenya


The code demonstrates how to visualize land cover classifications for Kenya using the MODIS Land Cover dataset (MODIS/006/MCD12Q1) and provides a legend for interpreting the map. Here's the step-by-step explanation:

1. Dataset Loading and Filtering
Dataset: The MODIS/006/MCD12Q1 dataset is loaded, representing global land cover types.
Year Filter: The dataset is filtered to select data for the year 2016.
Kenya Boundary: A boundary of Kenya is extracted from the global country boundaries dataset (USDOS/LSIB_SIMPLE/2017) and used to clip the dataset, isolating land cover data for Kenya.
2. Visualization Parameters
The LC_Type1 band of the MODIS dataset is visualized. This band contains land cover classifications coded as integers (1–17), each representing a distinct land cover type (e.g., forests, grasslands, urban areas).
A color palette is defined to represent these classifications visually. Each classification is associated with a unique color.
3. Map Layer Setup
The clipped land cover dataset is added as a map layer, showing Kenya's land cover.
Kenya's boundary is outlined in red for geographic context.
The map is centered on Kenya with an appropriate zoom level, and the TERRAIN basemap is used for added context.
4. Legend Creation
Panel Setup: A UI panel is created and styled to display the legend at the bottom-right corner of the map.
Class Information: An array (igbpClasses) is defined, containing the land cover class codes, descriptions, and corresponding colors.
Dynamic Entry Generation: Each entry in the igbpClasses array is processed to create:
A color box matching the class color.
A description label for the land cover type.
Both are added to the legend panel.
5. Adding the Legend
The legend is added to the map using Map.add(legend), allowing users to interpret the color-coded land cover map easily.
Output
Kenya Land Cover Map:

A color-coded map showing the distribution of various land cover types across Kenya.
Interactive Legend:

A panel in the bottom-right corner displaying a color key with land cover classifications and their names.


![Capture](https://github.com/user-attachments/assets/e0f50b21-08e7-4c2e-9b76-02c99572a9a5)

