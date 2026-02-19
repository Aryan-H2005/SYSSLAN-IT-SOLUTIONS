# Train Route Dataset Analysis - Level 1 

## Project Overview

This project involves a foundational analysis of a comprehensive railway dataset. The goal of Level 1 is to perform a "Data Health Check" and generate a structural overview of the train routes, schedules, and station distributions.

## Dataset Description
The primary dataset, Dataset1.csv, contains historical or scheduled train route information. Each row represents a specific stop for a train.

## Tasks Completed
### 1.1 Summary of the Dataset

Total Records: 186,074 entries.

Total Columns: 12.

Insights: The dataset is a flat-file representation of thousands of unique train journeys across a vast geographical network.

### 1.2 Train-wise Route Mapping
The data was transformed from a per-stop format to a per-train format. This allowed for the identification of:

1. Origin Station: The station where SN = 1.

2. Destination Station: The station with the highest SN or Distance for a given Train_No.

3. Stop Count: Total number of halts per journey.

### 1.3 Descriptive Statistics
Basic statistical analysis was performed on key numerical features:

1. Distance: Analysis of travel spans (ranging from short shuttles to long-distance expresses over 4,000 km).

2. Network Density: Average number of stops per train is approximately 16.7, though some "All-Stop" locals reach up to 118 stops.

### 1.4 Data Cleaning & Integrity Audit

1. Null Value Check: 0 missing values found across all columns.

2. Logical Consistency: A check was performed to ensure that Distance always increases as SN increases. No logical inconsistencies were detected.

3. Time Format: Validated that arrival and departure times follow the standard 24-hour clock.

## Key Findings 
1. Dataset Size: Large-scale (186k+ rows).

2. Train Count: 11,113 unique train services are represented.

3. Longest Route: 4,260 km.Highest Halts: 118 stations in a single journey.

## Tools Used
1. Python: Primary language for processing.

2. Pandas: Used for data manipulation and aggregation.

3. Descriptive Stats: Used for the foundational audit.
