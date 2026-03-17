# Project Overview

### Goal
This project analyzes NYC Taxi data to identify actionable, data-driven strategies for reducing traffic congestion.

### Problem
NYC's transit system faces significant congestion, particularly in Manhattan. Not only does this waste people's time, it also increases carbon emissions and accidents. This analysis explores how shifts in transportation modes, pricing, and technology can alleviate these issues.

### Methodology
1. **Data Exploration**: Analyzing hundreds of thousands of trip records to find patterns in distance, speed, and time of day.
2. **Inefficient Zone Mapping**: Identifying the specific zones and routes that act as bottlenecks.
3. **Policy Simulation**: Modeling the impact of dynamic congestion surcharges and carpooling.
# Table of Contents

1. Project Overview
2. Loading the Data
3. Cleaning the Data
4. Initial Analysis
5. Trip Distance Optimization
6. Congestion vs. Time of Day
7. Dynamic Pricing Simulation
8. Inefficient Zone Mapping
9. Carpooling Simulation
10. Summary

This analysis of NYC taxi data revealed several actionable strategies to reduce traffic congestion.

**Key Findings:**

1.  **Inefficient Short Trips**: A significant portion of taxi trips (56.52% under 2 miles) are inefficient due to low average speeds (e.g., 7.85 mph for trips under 1 mile), which are comparable to bikes & scooters. These short trips are less common in warmer months due to better weather.

2.  **Peak Hour Congestion**: Median average speeds drop substantially during 10 AM - 6 PM, indicating peak congestion.

3.  **Congestion Hotspots**: Several Manhattan zones (e.g., Garment District, Midtown Center, Times Sq) are identified as persistent congestion bottlenecks, with very low median taxi speeds. Many of the slowest specific routes are within or between these central Manhattan zones.
4.  **Carpooling Potential**: A large majority of taxi trips (78%) carry only one passenger. While simple carpooling for same-route, same-time trips yielded minimal impact (0.52% reduction), a more advanced "on-the-way" model, matching short trips with long trips, demonstrated a substantial potential for a 25.20% reduction in total trips.

**Recommendations:**

1. **Incentivize scooter & bike travel:** Instead of inefficient, short trips, bikes & scooters provide a quick, energy efficient way to commute short distances.  This would especially optimize summer months when traffic is already at its lowest. In colder months, when people prefer taxis, it could still create a difference, though other methods may be preferred.
2. **Dynamic pricing:** A dynamic pricing model could encourage people to use other forms of transport during peak hours. We suggest a $10 surcharge for trips starting between 8am and 8pm. This is especially effective because it leads to a larger percieved increase in shorter, cheaper trips. A simulation at different price elasticities showed that it could reduce trips under 1 mile by up to 7% and overall trips by about 5%.
3. **Carpooling App:** Develop app-based carpooling that matches shorter rides along the routes of longer, journeys, without significant detours. Our simulation found that matching long & short rides together could lead to a 25% reduction in taxi trips, though it does assume all passengers are comfortable carpooling. It also assumes roads form grids, which isn't true in all scenarios. Overall, the simulation could be made more realistic by using real map data from NYC and route planning, but it shows the potential of carpooling.
