# Daikibo Factory Telemetry Analysis

## Project Overview

This project analyzes telemetry data from Daikibo's global manufacturing operations to identify machine reliability issues and optimize factory performance. Using data collected from 4 factories across 3 countries during May 2021, we identified critical failure patterns and provided actionable recommendations.

## Business Objectives

The analysis addresses two key questions:
1. **Which location experienced the most machine breakdowns?**
2. **What specific machines broke most frequently at that location?**

## Factories Analyzed

- **Daikibo Factory Meiyo** - Tokyo, Japan
- **Daikibo Factory Seiko** - Osaka, Japan  
- **Daikibo Berlin** - Berlin, Germany
- **Daikibo Shenzhen** - Shenzhen, China

## Key Findings

### Factory Performance
- Daikibo Shenzhen had ~420 machine breakdowns (highest)
- Daikibo Factory Seiko: ~490 breakdowns
- Daikibo Factory Meiyo: ~105 breakdowns
- Daikibo Berlin: ~10 breakdowns (best performer)

### Machine Analysis
- **LaserCut machines** at Daikibo Shenzhen accounted for ~390 incidents
- This represents **93%** of all failures at the Shenzhen location
- Other machine types showed minimal failures (<2-5 incidents each)

## Project Structure

```
daikibo-telemetry-analysis/
│
├── data/
│   └── telemetry_data.json          # Raw telemetry data from all factories
│
├── analysis/
│   ├── Task_5_Equality_Table.xlsx   # Employee compensation equality analysis
│   └── dashboard.xlsx                # Main analysis dashboard
│
├── reports/
│   └── business_report.md           # Detailed findings and recommendations
│
├── visualizations/
│   ├── factory_performance.png      # Bar chart: Breakdowns by factory
│   └── device_analysis.png          # Bar chart: Breakdowns by device type
│
└── README.md                         # This file
```

##  Technologies Used

- **Microsoft Excel** - Data analysis and visualization
- **JSON** - Raw data format
- **Pivot Tables** - Data aggregation
- **Excel Charts** - Data visualization

## Dashboard Components

### Sheet 1: Factory Analysis
Bar chart showing "Unhealthy" incidents by factory location, clearly identifying Daikibo Shenzhen as the critical outlier.

### Sheet 2: Device Type Analysis  
Bar chart breaking down machine failures by type, highlighting LaserCut as the primary failure point.

##  Key Insights

1. **Concentrated Problem**: 93% of issues at one location stem from a single machine type
2. **Geographic Disparity**: Shenzhen has 42x more problems than Berlin
3. **Actionable**: Focused issue enables targeted intervention
4. **High Impact**: Fixing LaserCut issues could reduce failures by 90%

## Recommendations

### Immediate Actions (Week 1)
- Emergency inspection of Shenzhen LaserCut machines
- Compare maintenance logs between Shenzhen and Berlin
- Interview operators to document failure patterns

### Short-term (1-4 Weeks)
- Implement daily preventive checks
- Deploy Berlin maintenance team to Shenzhen
- Audit environmental controls and parts quality

### Medium-term (1-3 Months)
- Analyze failure patterns (time, shift, operator, material)
- Operator retraining based on Berlin standards
- Consider equipment upgrade if outdated

### Long-term (3-6 Months)
- Implement predictive maintenance using telemetry
- Standardize operations across all locations
- Deploy real-time monitoring dashboard

##  Methodology

1. **Data Collection**: Telemetry data from 36 machines (4 factories × 9 machine types)
2. **Data Processing**: Converted JSON data to structured format
3. **Analysis**: Aggregated breakdowns by factory and machine type
4. **Visualization**: Created comparative charts for executive review
5. **Recommendations**: Developed action plan based on findings

## Data Specifications

- **Time Period**: May 2021 (1 month)
- **Data Frequency**: Every 10 minutes per machine
- **Total Machines**: 36 (9 types × 4 locations)
- **Machine Types**: AirWrench, CNC, Conveyor, Furnace, HeavyDuty, LaserCut, LaserWeld, MetalPress, SpotWeld
- **Expected Messages**: ~155,520 total telemetry messages

## Getting Started

### Prerequisites
- Microsoft Excel 2016 or later
- JSON data file from Daikibo factories

### Installation
1. Clone this repository
   ```bash
   git clone https://github.com/yourusername/daikibo-telemetry-analysis.git
   ```
2. Open `dashboard.xlsx` in Microsoft Excel
3. Review the visualizations in Sheet 1 and Sheet 2

### Data Processing
If you need to process new telemetry data:
1. Place JSON file in the `data/` folder
2. Follow the data processing steps in `analysis/data_processing_guide.md`
3. Update pivot tables and charts accordingly

## Success Metrics

Track these KPIs to measure improvement:
- Monthly breakdown count by factory and machine
- Mean Time Between Failures (MTBF) for LaserCut
- Mean Time To Repair (MTTR)
- Month-over-month percentage improvement
- **Target**: 50% reduction in Shenzhen failures within 3 months

## Future Enhancements

- [ ] Implement automated telemetry processing pipeline
- [ ] Add time-series analysis for failure prediction
- [ ] Create real-time monitoring dashboard
- [ ] Integrate maintenance scheduling system
- [ ] Add cost analysis module
- [ ] Develop machine learning model for predictive maintenance

## Contributing

Contributions are welcome! Please follow these steps:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

##  Additional Analysis

### Task 5: Employee Compensation Equality
This project also includes an analysis of employee compensation equality across factories and job roles:
- **File**: `Task_5_Equality_Table.xlsx`
- **Methodology**: Scores range from -100 to +100 (0 is ideal)
- **Classification**: Fair (±10), Unfair (±11-20), Highly Discriminative (±21+)
- **Results**: 19 Fair, 11 Unfair, 7 Highly Discriminative classifications

## Contact

**Project Lead**: [Your Name]
- Email: your.email@example.com
- LinkedIn: [Your LinkedIn Profile]
- GitHub: [@yourusername](https://github.com/yourusername)

##  License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Daikibo technical team for data collection and unification
- Factory operations teams for their cooperation
- All contributors who helped improve this analysis

## Documentation

For more detailed information, see:
- [Business Report](reports/business_report.md) - Full analysis and recommendations
- [Data Dictionary](docs/data_dictionary.md) - Field definitions and data structure
- [Methodology](docs/methodology.md) - Detailed analysis approach

---

**Last Updated**: December 2025  
**Status**:  Analysis Complete | Recommendations In Progress

---

### Quick Links
- [View Dashboard](analysis/dashboard.xlsx)
- [View Visualizations](visualizations/)
- [Read Full Report](reports/business_report.md)
- [Equality Analysis](analysis/Task_5_Equality_Table.xlsx)
