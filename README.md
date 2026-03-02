# Food Delivery Analytics

A comprehensive data analysis project exploring food delivery datasets to extract business insights, optimise SQL queries, and visualise patterns across major delivery platforms (Takeaway, Uber Eats, Deliveroo).

This data analytics project focuses on extracting meaningful insights from food delivery databases through SQL operations, geospatial analysis, and data visualisation. The project explores three major delivery platforms to understand restaurant distribution, pricing patterns, ratings, and service coverage across different locations.

## Key Focus Areas
- **SQL Mastery**: Advanced database operations and query optimisation
- **Geospatial Analysis**: Mapping restaurant distribution and delivery coverage
- **Cross-Platform Comparison**: Analysing differences between Uber Eats, Deliveroo, and Takeaway
- **Data Storytelling**: Transforming raw data into business insights through visualisation

## Mission Objectives

Enhance data engineering and analytical skills by working with:

- **SQL Operations**: SELECT, JOIN, GROUP BY, aggregations, and advanced queries
- **Power BI Integration**: Interactive dashboard creation and data visualization
- **Geospatial Data Analysis**: Location-based insights and mapping visualizations
- **Food Delivery Insights**: Extracting patterns from real-world delivery datasets

## Data Sources

### Database Structure
The project works with three SQLite databases containing comprehensive food delivery data:

| Database Platform | Focus Areas | Data Volume |
|------------------|-------------|-------------|
| **Takeaway Database** | Primary analysis focus | Complete dataset |
| **Uber Eats Database** | Optional comparison | Platform-specific data |
| **Deliveroo Database** | Optional comparison | Platform-specific data |

### Key Data Entities
Based on the database schema, the data includes:
- **Restaurants**: Names, locations, ratings, cuisine types
- **Menu Items**: Prices, categories, dietary options (vegetarian, vegan)
- **Orders**: Delivery patterns, fees, service times
- **Geographic Data**: Location coordinates, coverage areas
- **Platform Metrics**: Cross-platform service comparisons

## Technologies & Tools Used

### Core Analysis Tools
| Tool/Technology | Purpose |
|-----------------|---------|
| **SQLite** | Primary database engine for data storage and querying |
| **Python 3.12** | Data analysis, visualisation, and automation |
| **Pandas** | Data manipulation and analysis |
| **SQLAlchemy** | Database connectivity and ORM |
| **Geopandas** | Geographic data analysis and mapping |

### Visualisation & Reporting
| Tool/Technology | Purpose |
|-----------------|---------|
| **Power BI** | Interactive dashboard creation and business intelligence |
| **Matplotlib/Seaborn** | Statistical visualisations and plots |
| **Plotly** | Interactive charts and geospatial visualisations |
| **Jupyter Notebooks** | Interactive data analysis and exploration |

## Core Features & Business Questions Answered
### 1. Price Distribution Analysis
- Price range distribution across all menu items
- Average pricing by category and restaurant type
- Price point analysis for different cuisines

### 2. Geographic Distribution
- Hotspot identification for restaurant concentration
- Location-based service coverage analysis
- Geographic patterns in restaurant density

### 3. Top Sushi Restaurants

### 4. Kapsalon Mapping Analysis

### 5. Price-to-Ratio Optimization
Which restaurants offer the best value for money?

### 6. Delivery Dead Zones
- Where are the areas with minimal restaurant coverage?
- Heat mapping of restaurant density
- Gap analysis in service coverage
- Optimisation opportunities for delivery platforms

### 7. Dietary Options Analysis

### 8. World Hummus Order (WHO)
Top 3 hummus serving restaurants

### 9. Cuisine Specialisation Index
Which restaurants are most specialised in their cuisine type?

### 10. Late-Night Service Analysis
- Which areas offer the best late-night dining options?
- Restaurant hours analysis
- Late-night menu availability
- Delivery time patterns by location and time

## Performance Optimisation
- **SQL Query Optimisation**: Index analysis, query plan optimisation, execution time monitoring
- **Database Schema Improvements**: Normalisation recommendations, indexing strategy
- **Caching Strategies**: Query result caching for frequent analytical operations

## Advanced Insights
- **Cross-Platform Cuisine Comparison**: Analyse average ratings across different platforms
- **High-Density Restaurant Zones**: Identify areas with market saturation opportunities
- **Cuisine Trend Analysis**: Regional culinary preferences and emerging trends

## Project Structure

```
food-delivery-analytics/
├── data/                          # Raw database files
│   ├── takeaway.db
│   ├── uber_eats.db
│   └── deliveroo.db
├── notebooks/                     # Jupyter analysis notebooks
│   ├── 01_data_exploration.ipynb
│   ├── 02_sql_analysis.ipynb
│   ├── 03_geospatial_analysis.ipynb
│   └── 04_visualization.ipynb
├── sql/                           # SQL query scripts
│   ├── core_queries.sql
│   ├── advanced_analysis.sql
│   └── optimization.sql
├── visualization/                 # Charts and maps
│   ├── price_distribution.py
│   ├── geographic_coverage.py
│   └── platform_comparison.py
├── reports/                       # Analysis reports
│   ├── business_insights.pdf
│   └── presentation_slides.pdf
├── requirements.txt               # Python dependencies
└── README.md                      # This file
```

## Configuration & Setup

### Environment Setup
```bash
# Create virtual environment
python -m venv food_delivery_env
source food_delivery_env/bin/activate  # On Windows: food_delivery_env\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Requirements.txt
```txt
pandas>=1.5.0
sqlalchemy>=1.4.0
geopandas>=0.12.0
matplotlib>=3.5.0
seaborn>=0.11.0
plotly>=5.10.0
jupyter>=1.0.0
powerbi-api>=0.6.0
scikit-learn>=1.1.0
```

### Database Connection Configuration
```python
# config.py
DATABASE_PATHS = {
    'takeaway': 'data/takeaway.db',
    'uber_eats': 'data/uber_eats.db', 
    'deliveroo': 'data/deliveroo.db'
}

# SQLAlchemy connection strings
DATABASE_CONNECTIONS = {
    'takeaway': 'sqlite:///data/takeaway.db',
    'uber_eats': 'sqlite:///data/uber_eats.db',
    'deliveroo': 'sqlite:///data/deliveroo.db'
}
```

## Data Quality & Validation

### Data Cleaning Processes
- Missing value handling and imputation
- Duplicate record removal
- Standardisation of categorical variables
- Outlier detection and correction

### Validation Methods
- Cross-platform data consistency checks
- Geographic coordinate validation
- Price range sanity checks
- Rating distribution analysis

## Future Enhancements

### Advanced Analytics Opportunities
- **Machine Learning Integration**: Predictive modeling for demand forecasting
- **Real-time Data Processing**: Live dashboard updates with streaming data
- **Mobile Application**: On-the-go analytics for field teams
- **API Development**: RESTful services for third-party integrations

### Scalability Improvements
- **Database Migration**: PostgreSQL for enterprise-scale operations
- **Cloud Deployment**: Azure/AWS infrastructure for production use
- **Big Data Processing**: Spark for massive dataset handling
- **Containerization**: Docker for consistent deployment environments
