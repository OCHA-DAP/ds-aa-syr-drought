# Syria Drought Analysis (2024/2025 Season)

This repository contains analyses focused on the 2024/2025 drought season in Syria, leveraging various data sources and analytical frameworks to assess agricultural and precipitation trends.

## Components

### Agricultural Stress Index (ASI) Analysis

This section analyzes the evolution and spatial distribution of the Agricultural Stress Index (ASI) across Syrian governorates during the critical 2024/2025 winter cropping season (November 2024 to April 2025).

- **Data Source**: ASI data retrieved via FAO GIEWS using the `cumulus` R package.
- **Key Features**:
  - Filters data by province and dekad to explore trends in crop-growing areas.
  - Calculates empirical return periods for ASI values to assess stress levels.
- **Visualization**:
  - Charts showing ASI trends over the season.
  - Maps highlighting ASI return periods by Syrian governorates.

### Seasonal Precipitation Summary (ERA5 Reanalysis)

This section focuses on precipitation data for the 2024/2025 season, derived from ECMWF's ERA5 Reanalysis product.

- **Data Retrieval**: Historical rainfall data fetched and processed for specific regions.
- **Seasonal Analysis**:
  - Assigning seasonal years to determine temporal trends.
  - Calculating total seasonal rainfall and anomalies.
  - Identifying tercile and quartile rainfall distributions.
- **Return Period Calculation**: Empirical return periods computed to evaluate rainfall deficits.
- **Visualization**:
  - Maps illustrating rainfall return periods and anomalies.
  - Charts tracking seasonal precipitation trends across regions.

## Repository Structure

The repository is organized as follows:

- `book_syr_drought/`: Contains Quarto markdown files and scripts for analysis and visualization.
  - `01_asi.qmd`: ASI analysis scripts.
  - `02_era5.qmd`: ERA5 precipitation analysis scripts.
  - Other supporting files for rendering and publishing outputs.
- `data/`: (Optional) Placeholder for any local datasets used in the analysis.
- `output/`: (Optional) Placeholder for rendered outputs such as maps and charts.

## How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/OCHA-DAP/ds-aa-syr-drought.git
   ```
2. Install required R packages:
   - [cumulus](https://github.com/OCHA-DAP/cumulus)
   - [ggplot2](https://ggplot2.tidyverse.org/)
   - Other dependencies listed in the Quarto scripts.
3. Run the Quarto markdown files (`.qmd`) to generate the analyses and visualizations.

## License

This project is licensed under the [MIT License](LICENSE).

## Contact

For questions or feedback, please contact the repository maintainers or open an issue in this repository.