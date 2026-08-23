# Kosovo Climate Change and Environmental Exposure

Geospatial analysis of heat, urbanization, vegetation change, air pollution, and population exposure across Kosovo.

## Overview

This repository supports a reproducible research project examining how environmental and climate-related conditions vary across Kosovo. The project brings together satellite observations, air-quality data, population estimates, and administrative boundaries to identify spatial patterns, changes over time, and communities facing overlapping environmental pressures.

The repository is under active development. Data sources, study periods, indicators, and analytical choices will be documented as the research design is finalized.

## Research themes

- **Heat:** Map land-surface temperature and identify persistent or intensifying hot spots.
- **Urbanization:** Measure changes in built-up land and their relationship to local environmental conditions.
- **Vegetation:** Track vegetation cover and greenness using satellite-derived indicators such as NDVI.
- **Air pollution:** Examine the spatial and temporal distribution of pollutants where suitable observations are available.
- **Population exposure:** Estimate how many people—and which places—are exposed to heat, pollution, vegetation loss, or multiple hazards.

## Guiding questions

1. How have heat, vegetation, and built-up land changed across Kosovo?
2. Where are environmental pressures concentrated?
3. How do patterns differ among municipalities and urban and rural areas?
4. Which populated areas experience multiple, overlapping exposures?
5. How sensitive are the results to the selected datasets, time periods, and spatial resolutions?

## Planned workflow

1. Define the study area, time period, indicators, and spatial units.
2. Acquire and document authoritative geospatial and demographic datasets.
3. Harmonize coordinate systems, resolution, temporal coverage, and geographic boundaries.
4. Calculate indicators for heat, urbanization, vegetation, air pollution, and population exposure.
5. Analyze trends, spatial disparities, and overlapping exposures.
6. Validate results and conduct sensitivity and uncertainty checks.
7. Produce reproducible maps, tables, figures, and summary outputs.

## Repository structure

```text
enri-kosovo-climate-change/
├── data/
│   ├── raw/          # Original data; generally not committed
│   ├── interim/      # Intermediate processing outputs
│   └── processed/    # Analysis-ready datasets
├── notebooks/        # Exploratory and documented analyses
├── src/              # Reusable processing and analysis code
├── outputs/
│   ├── figures/
│   ├── maps/
│   └── tables/
├── docs/             # Methods, data dictionary, and supporting notes
├── requirements.txt  # Python dependencies
└── README.md
```

Folders will be added as the project develops. Large, restricted, or externally licensed datasets should not be committed to the repository.

## Data sources

A complete data inventory will be added before analysis. Each source should be recorded with:

- provider and dataset title;
- version and access date;
- temporal and spatial coverage;
- spatial resolution and coordinate reference system;
- license and redistribution conditions;
- preprocessing steps and known limitations.

Potential source categories include Earth-observation imagery, atmospheric composition products, land-cover or built-up-area products, gridded population estimates, and official administrative boundaries. Inclusion here does not imply that a particular dataset has already been selected or validated.

## Reproducibility

The analysis is intended to be reproducible from documented source data. Scripts should use relative paths and preserve raw inputs unchanged. Derived outputs should record the software environment, parameters, processing date, and source-data versions used to create them.

Once dependencies are defined, the expected setup will be:

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
```

## Responsible interpretation

Satellite and modeled products are estimates, not direct measurements of individual exposure or health effects. Results may be affected by cloud cover, retrieval uncertainty, spatial resolution, missing observations, boundary definitions, and differences among data products. Population-exposure estimates should therefore be reported with appropriate caveats and, where possible, sensitivity analysis.

## Status

Project setup and research design are in progress. Results have not yet been finalized.

## License

Code in this repository is available under the [MIT License](LICENSE). Individual datasets remain subject to the licenses and terms of their original providers.

