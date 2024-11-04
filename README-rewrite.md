# Software Job Market Insights iOS App

## Project Overview
**Final Project Proposal**  
CMPSC 475: Applications Programming  
Penn State University  
Fall 2024

## Problem Statement

Software professionals often struggle to make informed decisions about job locations due to the complexity of factors affecting total compensation, cost of living, and career advancement opportunities. While raw data which characterize each of these topics individually exist, it is difficult to visualize their interconnectedness.

## Solution Overview

The Software Job Market Insights iOS app will provide interactive visualizations in order to help software professionals analyze and compare job markets across the United States. The app will combine a map view, a list view, a company / city details view, and a comparison view. 

## Key Features

### 1. Interactive Job Market Map

The map offers four visualization modes for displaying markers across the United States:

#### A. Software Developer Income + Expenses by City
- Markers colored based on average total compensation
- Optional toggle to include cost of living adjustments
- Interactive comparison between raw and adjusted salaries

#### B. Quantity of Software Jobs by City
- Markers colored based on total number of available positions
- Heat map visualization of job density by region

#### C. Company Job Location
- Markers based on company-specific average compensation
- Features include:
  - Company search functionality
  - Filtering by major tech employers (Apple, Google, etc.)
  - Salary range visualization

#### D. Weighted Market Score
- Comprehensive ranking based on:
  - Total job availability
  - Average compensation
  - Employer diversity
  - Cost of living adjustments
- Customizable weighting of factors

<div align="center">
<table>
<tr>
<td width="50%">
  <img src="images/job-market-map.png" width="100%">
  <p align="center"><i>Interactive Job Market Map Sample</i></p>
</td>
<td width="50%">
  <img src="images/job-market-map-annotation.png" width="100%">
  <p align="center"><i>Sample Annotation Displayed on Tap</i></p>
</td>
</tr>
</table>
</div>

### 2. Navigation List 
This list is parallel to the above map, showing the rankings in a list format instead of a keyed map. The list view will include additional advanced filters suitable to a list format:

#### A. Income & Expenses Filters
- Minimum base salary threshold
- Maximum cost of living index
- Minimum disposable income after expenses

#### B. Job Quantity Filters
- Minimum number of available positions
- Job density per capita
- Job level distribution (entry/mid/senior)

#### C. Company-Specific Filters
- Company size (startup/midsize/enterprise)
- Employees in specific cities

#### D. Weighted Score Filters
- Minimum composite score threshold
- Custom weight presets

<div align="center">
<table>
<tr>
<td width="50%">
  <img src="images/city-list.png" width="100%">
  <p align="center"><i>Interactive Job Market Map Sample</i></p>
</td>
</tr>
</table>
</div>

### 3. Comparison View

The comparison view is accessible through interactions in both the map and list views. Users can:
- Tap on map annotations or list items to add locations/companies to the comparison queue
- View detailed comparisons of up to 4 items simultaneously
- Access comparison data through a menu that appears on selection
- Add or remove items from the comparison queue as needed
- Lists all data on a city or company (depending on mode) such as company size, average salary, quantity of jobs in city, etc.
- Will be able to function as a single company or city details view if it is the only item in the comparison queue

## Technical Implementation

### Data Sources
- Company Hiring Data, Locations of Positions, Mean Salaries of Positions
  - https://www.kaggle.com/code/nileshthonte/levels-fyi-salary-dataset-eda-and-modelling/input
- Software Developer Income & Expenses per City
  - https://www.kaggle.com/datasets/thedevastator/u-s-software-developer-salaries/data
- Quantity of Software Developer Jobs by City
  - https://data.bls.gov/oes/#/occGeo/One%20occupation%20for%20multiple%20geographical%20areas

### Frameworks

- MapKit
- UIKit
- Core Data

### Navigation
```
Tabs
    │
    ├── Map View (Main Tab)
    │   ├── Filter Controls
    │   └── City Detail View or Company Detail View depending on mode
    │
    ├── List View (Second Tab)
    │   ├── Sorting Controls
    │   └── Filter Controls
    │
    └── Comparison View (Third Tab)
        ├── Comparison Queue (up to 4 items)
        ├── Detailed Metrics Grid
        └── Add/Remove Items Controls
```

### Development Timeline

- Nov. 3 to Nov. 12: (Model + Data Schema)
  - Model configuration
  - Setup universal identifiers of cities and locations to coalesce different schemas from different data sources
- Nov. 10 to Nov. 17: (Map View Main)
  - Map View Configuration
  - Mode selection on Map View for Salary, Company, Quantity with color keys
- Nov. 17 to Nov. 24: (Additional Map View and Model View Config)
  -  Annotation on Map View configuration
  -  Create functionality for comparison queue in model view
  -  Add ability to add and remove from comparison queue in annotation on map view
- Nov. 24 to Dec. 1: (List View)
  - List View Configuration
  - Mode selection on List View for Salary, Company, Quantity
  - Advanced Filters on List View
- Dec. 1 to Dec. 8: (Comparison View)
  - Comparison View Implementation
- Dec. 8 to Dec. 15: (Miscellaneous)
  - Testing
  - Cosmetic and Aesthetic Configurations
  - Proper configuraiton for different device layouts and sizes
