# Autonomous Vehicle Behavior Analysis at Urban Intersections

This project analyzes transportation behavior within the Foggy Bottom segment of the Third Generation Simulation (TGSIM) dataset, focusing on how autonomous vehicles (AVs), traditional passenger vehicles, and pedestrians interact at a busy urban intersection. The goal of the project was to evaluate the claim that AVs operate more safely and predictably than other transportation agents by studying 200 seconds of recorded trajectory data.

The analysis was completed for CIVE 202 – Civil Engineering Analysis II during Spring 2026 and used traffic simulation data provided through the USDOT TGSIM dataset. The project focused on identifying movement patterns, speed consistency, acceleration behavior, and deceleration events across multiple transportation groups. The work also included visualization of agent trajectories and lane-level movement throughout the intersection area.

---

# Project Objectives

- Compare the behavior of autonomous vehicles, passenger vehicles, and pedestrians
- Analyze acceleration and deceleration behavior near the intersection
- Measure average speeds and variability between transportation groups
- Detect disruptive behavior using hard braking and deceleration events
- Visualize movement trajectories and interaction patterns inside the intersection
- Evaluate whether AVs demonstrate more stable and predictable driving behavior

---

# Dataset Information

The project used the following dataset and support files:

- `Transformed_TGSIM_Foggy_Bottom_200sec.csv`
- `TGSIM_Data_Dictionary.xlsx`
- `Polygons.ipynb`

The dataset contains timestamped trajectory information for transportation agents moving through an urban intersection. Each observation includes:

- Agent ID
- Timestamp
- X and Y location coordinates
- Speed
- Acceleration
- Lane information
- Transportation mode classification

The data includes multiple transportation agents such as:

- Autonomous Vehicles
- Passenger Cars
- Pedestrians
- Bicycles
- Scooters
- Buses
- Trucks
- Motorcycles

---

# Methods and Analysis

Python was used for all data processing and analysis using:

- Pandas
- NumPy
- Matplotlib
- Seaborn

The workflow included:

1. Cleaning and organizing the trajectory dataset
2. Removing duplicate or incomplete records
3. Sorting trajectories by agent and time
4. Calculating movement metrics such as:
   - Speed
   - Signed acceleration
   - Jerk
   - Speed variability
5. Detecting hard deceleration events
6. Comparing behavior by lane and transportation type
7. Generating movement visualizations and statistical summaries

Polygon boundary data from the provided notebook was used to isolate activity occurring inside the intersection and nearby approach zones.

---

# Visualizations Included

The project includes several visual and statistical outputs:

- Average speed bar charts
- Signed acceleration comparisons
- Speed distribution boxplots
- Lane-by-lane speed profiles
- Hard deceleration event analysis
- Intersection trajectory movement plots
- Colored transportation path visualizations

These visualizations were used to compare stability and movement consistency between AVs and other transportation agents.

---

# Key Findings

Initial results showed that autonomous vehicles generally maintained:

- Lower speed variability
- Fewer hard deceleration events
- More stable acceleration behavior

Passenger vehicles showed higher speed variation and more aggressive braking patterns, while pedestrians maintained the slowest and most stable movement profiles overall.

## Example Initial Results

| Agent Type | Avg Speed (ft/s) | Avg Acceleration (ft/s²) | Deceleration Events | Speed Variability |
|---|---|---|---|---|
| Autonomous Vehicles | 32.5 | 1.8 | 5 | 3.2 |
| Passenger Vehicles | 35.7 | 2.6 | 12 | 6.8 |
| Pedestrians | 4.2 | 0.8 | 2 | 1.1 |

These findings suggest that autonomous vehicles may behave more consistently and predictably than traditional passenger vehicles within intersection environments.

---

# Repository Contents

- Jupyter Notebook with full analysis workflow
- Annotated code documentation
- Statistical summaries
- Graphs and visualizations
- Technical report and methods documentation
- Initial findings and comparison tables

---

# Authors

- Gabriel Goeken
- Matthew Mendenhall
- Kaleb Mangers

---

# Course Information

**CIVE 202 – Civil Engineering Analysis II**  
Spring 2026  
Civil and Environmental Engineering
