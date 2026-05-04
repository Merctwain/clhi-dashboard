# Community Loss and Hope Index Dashboard

A data visualization dashboard mapping community grief and loss indicators across Philadelphia ZIP codes.

**Developed by the [Wealth + Work Futures Lab](https://wealthworkfutures.org) at Drexel University's Lindy Institute for Urban Innovation**

## Overview

The Community Loss and Hope Index (CLHI) Dashboard provides researchers, policymakers, and community stakeholders with tools to explore the geographic distribution of loss indicators across Philadelphia. The dashboard demonstrates that loss isn't random—it's place-based and persistent.

## Dashboard Views

### 1. Interactive Map (`explore.html`)
- Bubble map visualization of ZIP codes sized by population and colored by indicator
- Year slider with animation (2015-2023)
- Multiple indicators: Community Loss Index, Early Death, Overdose, Homicide, Shootings, Hospitalization, Foster Care, School Closures
- Geographic mini-map navigation
- Detailed ZIP code statistics panel

### 2. Data Story (`narrative.html`)
- Guided narrative presentation of key findings
- Section-by-section breakdown of loss patterns
- Bereavement gap visualization (42 years of data)
- Compounding effects analysis
- At-a-glance statistics

## Key Findings

- **40%** of all shootings concentrated in just 5 ZIP codes (19134, 19140, 19132, 19124, 19143)
- **81% spike** in homicides during COVID (257 in 2019 to 465 in 2021)
- **1.5-2x higher** bereavement rate for Black children—persistent for 42 consecutive years
- The same neighborhoods appear at the top of every loss indicator

## Data Sources

- PA Vital Registration
- Philadelphia Department of Human Services (DHS)
- Philadelphia Police Department
- Pennsylvania Health Care Cost Containment Council (PHC4)
- Prison Policy Initiative
- Judi's House CBEM

## Deployment

This dashboard is designed for GitHub Pages deployment:

1. Push this repository to GitHub
2. Go to repository Settings > Pages
3. Select "Deploy from a branch" and choose `main` branch
4. The site will be available at `https://[username].github.io/clhi-dashboard/`

## File Structure

```
clhi-dashboard/
├── index.html                              # Landing page
├── explore.html                            # Interactive map view
├── narrative.html                          # Data story view
├── data.json                               # All dashboard data (editable)
├── CLHI Data Documentation & Methodology.pdf   # Methodology documentation
└── README.md                               # This file
```

## Updating the Data

All dashboard data is stored in `data.json`. To update the data:

1. Open `data.json` in any text editor
2. Edit the relevant sections:
   - `fullData` - ZIP code data by year (2015-2023)
   - `cityTrends` - City-wide annual statistics
   - `summaryStats` - At-a-glance statistics
   - `rankings` - Top 5 highest loss ZIP codes
   - `thenVsNow` - Overdose comparison data
   - `narrativeBarChart` - Bar chart data by indicator
   - `bereavementGap` - Historical bereavement data
3. Save the file and refresh the dashboard

No HTML code changes are needed to update the data.

## License

This project is developed for research and public benefit by the Wealth + Work Futures Lab at Drexel University.

## Contact

Wealth + Work Futures Lab
Lindy Institute for Urban Innovation
Drexel University
[wealthworkfutures.org](https://wealthworkfutures.org)
