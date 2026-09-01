# 🌿 Sukkah Scene & Sun Tracker
A specialized Blender script designed to automatically generate a 3D Sukkah structure and calculate realistic solar positions based on real-world coordinates, dates, and times.
## 🚀 Features
- Interactive Control Panel: A custom UI in the 3D Viewport (N-Panel) allows you to adjust dimensions and time settings in real-time.
- Dynamic Sun Tracking: Automatically updates the "Physical Sun" position based on the Latitude, Month, Day, and Time of day.
- Customizable Geometry: Easily adjust:
    - Wall Height: Change the height of the Sukkah walls.
    - Dimensions: Modify Width and Length of the floor area.
    - Schach Density: Control the percentage of "Schach" (the overhead covering) to simulate different roof styles.
- Automatic Scene Setup: On execution, the script automatically creates:
    - A high-quality floor.
    - Four structured walls.
    - A Sun light source.
    - 3D text labels for dimensions and measurements.
- One-Click Reset: A "Reset to Defaults" button to quickly restore the scene to standard settings.
## 🛠️ Installation & Usage
1. Prerequisites:
    - Blender (3.0 or higher recommended).
2. Installation:
    - Copy the script provided in this repository.
    - Open Blender and go to the Scripting workspace.
    - Click New, paste the code, and click Run Script.
3. Navigation:
    - Once the script is running, look for the "Sukkah" tab in the Sidebar (press `N` in the 3D Viewport to open the sidebar).
    - Use the Sukkah Master Controls panel to adjust the scene.
    - Click "Calculate Sun & Update Sukkah" to refresh the lighting after changing time or location.
## ⚙️ Parameters Guide
| Property | Description | Default |
| --- | --- | --- |
| Wall Height | Sets the height of the side walls in meters. | 3.0m |
| Width / Length | Defines the footprint of the Sukkah floor. | 3.0m x 3.0m |
| Schach Holes % | Adjusts the density of the roof material. | 50% |
| Latitude | Sets the geographic location (e.g., 31.77 for Israel). | 31.77 |
| Month / Day | Sets the specific date for solar calculation. | Oct 15 |
| Time of Day | Sets the hour of the day (in 24h format). | 14:00 |
## 🏗️ Technical Details
The script utilizes Blender's `bpy` API to create custom properties on the Scene level. It links the UI sliders directly to the calculation functions, ensuring that moving a slider immediately updates the sun's position and the mesh dimensions.
## 📝 License
This project is open-source and available for personal and community use.


### Suggestions for improvement (Optional):
If you want to make the README even better, you could add a "Screenshots" section showing:
1. The "Sukkah Master Controls" panel in the N-panel.
2. A "Before and After" shot showing how the sun's shadow changes when you move the "Time of Day" slider.