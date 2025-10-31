🏠 Belmont North Property Orientation Analysis
📘 Overview

This project analyzes residential property orientations in Belmont North, NSW, to understand how house direction influences sunlight exposure, comfort, and investment potential.
It demonstrates how real estate data can be fetched, cleaned, analyzed, and visualized using Python.

🎯 Objectives

Retrieve real-world property data via the Microburbs Sandbox API

Clean and extract address information from raw API output

Simulate property bearings and map them to compass orientations

Derive new analytical features:

Sunlight Score — measures exposure to natural light

Comfort Category — interprets livability based on orientation

Investment Potential Score — combines sunlight and energy efficiency metrics

Visualize orientation patterns and investor insights

⚙️ Tech Stack

Language: Python 3.12

Libraries: pandas, numpy, matplotlib, seaborn, requests

Optional: plotly or folium for advanced visuals

🧩 Workflow

Data Fetching:
Uses the Microburbs API (https://www.microburbs.com.au/report_generator/api/suburb/properties) to retrieve property listings for Belmont North.

Data Cleaning:
Handles truncated JSON responses and extracts usable fields like street, suburb, and state.

Orientation Assignment:
Simulates building bearings (0–360°) and converts them to cardinal directions (N, NE, E, SE, S, SW, W, NW).

Feature Engineering:

Sunlight Score: ranks orientations from best (North) to least optimal (South).

Comfort Category: groups properties into High, Moderate, or Low comfort based on sunlight.

Investment Potential: weighted combination of sunlight and energy rating.

Visualization:

Colorful bar and pie charts of orientation distributions

Comfort-level comparison plots

Investment potential chart per property

Output:
Saves BelmontNorth_Property_Orientations.csv with all computed metrics.

📊 Example Output
Street	Suburb	State	Bearing	Orientation	Sunlight_Score	Comfort_Category	Investment_Potential
17 Dulungra Avenue	Belmont North	NSW	37	North-East	4	High Comfort	4.4
46 Arlington Street	Belmont North	NSW	235	South-West	2	Low Comfort	3.1
75 Buttaba Avenue	Belmont North	NSW	72	East	3	Moderate Comfort	3.8
🌞 Key Insights

Majority of homes face North-East or South-West in Belmont North.

North/East-facing homes receive the most natural sunlight → higher comfort and resale value.

Investment Potential Score helps investors prioritize properties combining livability and energy efficiency.

🚀 How to Run
pip install pandas numpy matplotlib seaborn requests
python main.py


Or open the provided Colab Notebook and run all cells sequentially.

🧠 Future Improvements

Integrate real roof azimuth data via GIS APIs

Add Folium map visualization for property plotting

Combine with solar exposure and rental yield datasets for predictive analysis

✨ Author

Manveer Singh
📧 mssandhuu05@gmail.com
