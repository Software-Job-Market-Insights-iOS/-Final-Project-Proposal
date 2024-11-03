# Software Job Market Insights iOS App

## Project Overview
**Final Project Proposal**  
CMPSC 475: Applications Programming  
Penn State University  
Fall 2024

## Problem Statement

Software professionals often struggle to make informed decisions about job locations due to the complexity of factors affecting total compensation, cost of living, and career advancement opportunities. While raw data which characterize each of these topics individually exist, it is difficult to visualize their interconnectedness.

## Solution Overview

*UNFINISHED*

The Software Job Market Insights iOS app will provide interactive visualizations in order to help software professionals analyze and compare job markets across the United States. The app will combine...

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

This list is parallel to the above map, showing the rankings in a list format instead of a keyed map.

<div align="center">
<table>
<tr>
<td width="50%">
  <img src="images/city-list.png" width="100%">
  <p align="center"><i>Interactive Job Market Map Sample</i></p>
</td>
<td width="50%">
  <img src="images/job-market-map-annotation.png" width="100%">
  <p align="center"><i>Sample Annotation Displayed on Tap</i></p>
</td>
</tr>
</table>
</div>

#### 3. Comparison View

In 

### Technical Implementation

#### Data Sources
- Company Hiring Data, Locations of Positions, Mean Salaries of Positions
  - https://www.kaggle.com/code/nileshthonte/levels-fyi-salary-dataset-eda-and-modelling/input
- Software Developer Income & Expenses per City
  - https://www.kaggle.com/datasets/thedevastator/u-s-software-developer-salaries/data
- Quantity of Software Developer Jobs by City
  - https://data.bls.gov/oes/#/occGeo/One%20occupation%20for%20multiple%20geographical%20areas

#### Frameworks

### Navigation

```
Tabs
    │
    ├── Map View (Main Tab)
    │   ├── Filter Controls
    │   └── City Detail View or Company Detail View depending on mode
    │
    └── List View (Second Tab)
        ├── Sorting Controls
        └── City Comparison View
```

### Development Timeline

