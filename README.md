# Software Job Market Insights iOS App
## Final Project Proposal
## Penn State CMPSC 475 Applications Programming Fall 2024

### Problem Statement
Software professionals often struggle to make informed decisions about job locations due to the complexity of factors affecting total compensation and quality of life. While raw salary data is available, it's difficult to visualize and compare locations while accounting for factors like cost of living, tax burden, and market demand.

### Solution Overview
The Software Job Market Insights iOS app will provide interactive visualizations in order to help software professionals analyze and compare job markets across the United States. The app will combine geographical data, economic indicators, and market trends to deliver actionable insights for career planning.

### Key Features

#### 1. Interactive Job Market Map
- Interactive US map showing software engineering job concentrations
- Color-coded markers based on selected metrics:
  - Raw salary data
  - Cost of living adjusted salary
  - Tax burden impact
  - Number of available positions
  - Standard of living index
- Filter controls to adjust visualization parameters
- Tap markers to view detailed city statistics

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

#### 2. City Rankings & Comparisons
- Sortable list view of all tracked cities
- Ranking metrics:
  - Total compensation
  - Cost-adjusted compensation
  - Job availability
  - Growth potential
  - Quality of life score
- Side-by-side city comparison tool
- Detailed breakdown of each metric's components
- Export comparison data as PDF

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

#### 3. Market Trends Dashboard
- Historical and projected industry trends
- Key metrics:
  - CS degree graduation rates
  - Industry hiring projections
  - Major employer hiring volumes
  - Inflation impact on compensation
  - Remote work trends
- Interactive charts and graphs
- Quarterly data updates

### Technical Implementation

#### Data Sources
- Company Hiring Data, Locations of Positions, Mean Salaries of Positions
  - https://www.kaggle.com/code/nileshthonte/levels-fyi-salary-dataset-eda-and-modelling/input
- Software Developer Income & Expenses per City
  - https://www.kaggle.com/datasets/thedevastator/u-s-software-developer-salaries/data
- Quantity of Software Developer Jobs by City
  - https://data.bls.gov/oes/#/occGeo/One%20occupation%20for%20multiple%20geographical%20areas

#### Frameworks & Technologies
- MapKit for geographical visualization
- CoreLocation for location services
- Charts framework for trend visualization
- CoreData for local data persistence
- Firebase for authentication and real-time updates
- SwiftUI for modern, responsive UI
- Combine for reactive programming
- Swift Package Manager for dependencies

### User Interface & Navigation

#### Navigation Flow
```
Tabs
    │
    ├── Map View (Main Tab)
    │   ├── Filter Controls
    │   └── City Detail View
    │
    ├── Rankings (Second Tab)
    │   ├── Sorting Controls
    │   └── City Comparison View
    │
    └── Trends (Third Tab)
        ├── Trend Selection
        └── Detailed Analysis View
```

### Development Timeline

#### Beta Version (Week 6)
- Complete map implementation with basic markers
- Initial city ranking list with sorting
- Basic authentication system
- Local data storage implementation
- Preliminary UI for all main screens

#### Final Version (Week 12)
- Enhanced map filters and visualizations
- Complete trends dashboard
- City comparison feature
- Data export functionality
- Polish UI/UX
- Performance optimization

### Weekly Breakdown

#### Weeks 1-2
- Set up project structure
- Implement authentication
- Create basic navigation flow
- Begin MapKit integration

#### Weeks 3-4
- Complete map visualization
- Implement data services
- Build city ranking system
- Begin trends dashboard

#### Weeks 5-6
- Finalize beta version features
- Polish existing functionality
- Prepare for beta review
- Begin user testing

#### Weeks 7-8
- Implement feedback from beta
- Complete comparison features
- Add data export options
- Enhance visualizations

#### Weeks 9-10
- Finalize trends dashboard
- Implement advanced filters
- Add additional data sources
- Performance optimization

#### Weeks 11-12
- Final polish and bug fixes
- Documentation
- App Store preparation
- Final testing

### Success Metrics
- Smooth performance with large datasets
- Intuitive navigation flow
- Accurate data visualization
- Positive user feedback
- Comprehensive market insights

### Future Enhancements
- Machine learning for salary predictions
- International job market comparisons
- Integration with job posting platforms
- Community features and reviews
- Custom alert system for market changes
