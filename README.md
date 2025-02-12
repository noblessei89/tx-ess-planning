# A Cross-Source Data Repository for Energy Storage Planning
This data repository is thoughtfully designed to enhance accessibility, empowering researchers to conduct more efficient analyses and drive innovation in ESS optimization and grid economics.

## Features
The data repository for Energy Storage planning offers a comprehensive collection of datasets that support in-depth analysis of energy storage opportunities across Texas. The key features include:

![image](https://github.com/user-attachments/assets/e44aa0dd-e37e-4237-9a45-7ebbee6c4d68)

### 1. Locational Marginal Prices (`LMPs`) for ERCOT Nodes
- **Data Coverage**: Historical LMP data for ERCOT nodes, spanning from 2010 to 2022.
- **Resolution**: Prices are available at a 5-minute interval resolution, facilitating granular temporal analysis.
- **Data Structure**: Data is organized by node and year. Each day is represented as a unique column, with 288 rows corresponding to 5-minute intervals over 24 hours.
- **Access**: This dataset democratizes access to long-term ERCOT LMP data, which is otherwise challenging to obtain.

### 2. Estimated Geographic Locations of ERCOT Nodes
- **Mapping**: Geographic data derived from ERCOT's Real-Time Locational Prices map.
- **Visualization**: The provided map and conversion tools enable spatial visualizations, such as comparing LMPs over time.
- **Important**: All geographic information represents only relative positioning on a 600×600 pixel map of Texas for visualization purposes, rather than actual coordinates, and should not be considered accurate. The data were estimated from ERCOT's Real-Time Locational Prices Map, and no details about the actual node locations are available.

### 3. Estimated Locations of Renewable Energy and ESS Sites
- **Coverage**: Includes the estimated geographic locations of solar farms, wind power facilities, and ESS installations across Texas.
- **Support for Spatial Analysis**: The relative coordinates provided for each installation allow for precise spatial analysis and mapping, aiding in identifying synergies in energy generation and storage.
- **Important**: All geographic information represents only relative positioning on a 600×600 pixel map of Texas for visualization purposes, rather than actual coordinates, and should not be considered accurate.

## Navigation
This repository mainly contains three components: source data, released data, and plotting code. We navigate this data repository as follows:

![image](https://github.com/user-attachments/assets/fba7216a-b05f-4a9e-b201-cda018a70cac)

All data sourced from the ERCOT Data Access Portal is archived in the `data_source/` folder. Although ERCOT generates one file every 5 minutes, we have organized these files by year to simplify analysis, consolidating them into a single file per year. Each yearly file is named in the format `lmp_<year>_nodes.csv`.

For filtered data, the `data_release/` folder contains individual files for each node, organized by year. Each file, named `<nodename>_<year>.csv`, provides 5-minute interval LMP values for the respective node.

## Usage
This repository is ideal for:
- **Temporal Analysis**: Examining LMP variability over time across different ERCOT nodes.
- **Spatial Analysis**: Understanding locational price differences and optimizing energy storage deployment.
- **Energy Storage Planning**: Supporting planning for ESS by providing detailed data on prices, locations, and renewable generation facilities.

## Acknowledgments
This repository integrates publicly available data from:
- **ERCOT**: Locational Marginal Price and node data.
- **Energy Information Administration (EIA)**: Locations of renewable energy and ESS installations.

## Support Team
This project is a collaboration of our group members under the supervision of Prof. Le Xie, Gordon McKay Professor of Electrical Engineering at Harvard John A. Paulson School of Engineering and Applied Sciences (SEAS). The support team keeps processing, correcting and updating the data every day. The team will also conduct further research analysis and share the latest progress in this repository.

<img width="532" alt="image" src="https://github.com/user-attachments/assets/4a9b13e1-6d51-4f27-8282-55ea923e7266">

## Contact Us
Please contact us if you need further technical support or search for cooperation. Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Email contact: [Le Xie](mailto:xie@seas.harvard.edu), [Dongjoo Kim](mailto:djkim@tamu.edu), [Subir Majumder](mailto:subir-em@ieee.org)
