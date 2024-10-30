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
- Save favorite locations for quick comparison

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
- Salary Data: Levels.fyi API and Bureau of Labor Statistics
- Cost of Living: Numbeo API
- Tax Information: TaxJar API
- Job Market Data: LinkedIn and Indeed APIs
- Educational Statistics: National Center for Education Statistics
- Company Hiring Data: SEC filings and company reports

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
Login/Registration
    │
    ├── Map View (Main Tab)
    │   ├── Filter Controls
    │   └── City Detail View
    │
    ├── Rankings (Second Tab)
    │   ├── Sorting Controls
    │   ├── City Comparison View
    │   └── Export Options
    │
    ├── Trends (Third Tab)
    │   ├── Trend Selection
    │   └── Detailed Analysis View
    │
    └── Settings (Fourth Tab)
        ├── Profile Management
        ├── Preferences
        └── Data Update Controls
```

#### Mock Screens

[Note: In an actual proposal, insert mockup screenshots here using design tools like Figma]

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
