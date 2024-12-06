# Hydrograph-Versus-Seatek-Sensors-Project

[![GitHub issues](https://img.shields.io/github/issues/abhimehro/Hydrograph-Versus-Seatek-Sensors-Project)](https://github.com/abhimehro/Hydrograph-Versus-Seatek-Sensors-Project/issues)

# Hydrograph-Seatek-Data-Visualizer

This repository contains a Python script that visualizes hydrograph and Seatek sensor data from Excel files. The script dynamically handles data for different river miles and sensors, providing a flexible solution for data visualization.

## Project Overview

The project consists of one main element:

1. **Visualizer**: Creates visualizations to compare sensor data with hydrograph measurements.
   The project processes data for multiple river miles, each with a varying number of sensors,
   and generates charts comparing sensor data with hydrograph measurements over a 20-year period.

## Project Structure

Hydrograph-Versus-Seatek-Sensors-Project/

├── data/
│   ├── Data_Summary.xlsx
│   ├── RM_13.1.xlsx
│   ├── RM_15.0.xlsx
│   └── ... (other RM files)
├── scripts/
│   └── updated_visualizer.py
output/
RM_54.0/
RM_54.0_Year_1_Sensor 1.png
RM_54.0_Year_1_Sensor 2.png
RM_54.0_Year_2_Sensor 1.png
...
RM_53.0/
...
└── ... (other directories)
├── docs/ │
├── README.md

## Data File Format

The primary data source for this project is an Excel file named `Data_Summary.xlsx`. This file contains a sheet named 'Data_Summary' that provides an overview of the available data, including river miles, the number of sensors at each river mile, and the corresponding years of data.

# Data Structure

The data files contain the following columns:

*   **River Mile:** The river mile where the data was collected.
*   **Num Sensors:** The number of Seatek sensors deployed at that river mile.
*   **Start Year:** The starting year of the data collection period.
*   **End Year:** The ending year of the data collection period.
*   **Notes:** Any additional notes or comments about the data.

## Script Description

The `updated_visualizer.py` script reads data from the `Data_Summary.xlsx` file and generates visualizations of the hydrograph and Seatek sensor readings. The script dynamically adapts to different river miles and sensors, providing a versatile tool for data analysis.

## Output

The generated charts are saved in the `output` folder.

## Dynamic Data Handling

The script leverages the `Data_Summary.xlsx` file to dynamically handle data for different river miles and sensors. It reads the relevant data for each river mile and sensor combination, ensuring that the visualizations are tailored to the specific data being analyzed.

## Illustrative Examples

Here are a few examples of the charts generated by the script:

![Chart for River Mile 54.0, Sensor 1, Year 1](https://raw.githubusercontent.com/abhimehro/Hydrograph-Versus-Seatek-Sensors-Project/main/output/RM_54.0/RM_54.0_Year_1_Sensor%201.png)

![Chart for River Mile 54.0, Sensor 2, Year 1](https://raw.githubusercontent.com/abhimehro/Hydrograph-Versus-Seatek-Sensors-Project/main/output/RM_54.0/RM_54.0_Year_1_Sensor%202.png)

## Additional Considerations

*   **Data Validation:** The script includes data validation checks to ensure the integrity of the input data.
*   **Error Handling:** Robust error handling is implemented to provide informative messages to the user in case of issues.
*   **Code Comments:** The code is well-commented to improve readability and maintainability.
*   **Unit Tests:** Comprehensive unit tests are included to cover various scenarios and edge cases.
  
## Setup

1. Clone the repository:
    ```bash
    git clone https://github.com/abhimehro/Hydrograph-Versus-Seatek-Sensors-Project.git
    cd Hydrograph-Versus-Seatek-Sensors-Project
    ```

2. Create and activate a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate # On Windows use venv\Scripts\activate.bat
    ```

3. Install required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Place Excel files in the `data` directory.
2. Run the visualizer script:
    ```bash
    python scripts/updated_visualizer.py
    ```
3. View generated charts in `output`.

## Running Tests

To run the unit tests:
```bash
pytest
```

Edit the `config.yaml` file to adjust settings such as data directory paths, river miles, sensor configurations, and
chart parameters.

## Contributing

 ```markdown
 Please read `CONTRIBUTING.md` for details on our code of conduct and the process for submitting pull requests.
 ```

## Roadmap

See the open issues for a list of proposed features (and known issues).

## Authors

- Abhi Mehrotra - [abhimehro](https://github.com/abhimehro)

## Acknowledgments

We welcome contributions to the Hydrograph-Versus-Seatek-Sensors-Project! Please follow these guidelines to help us
review and accept your changes.

## How to Contribute

1. Fork the repository: Click the "Fork" button at the top right of this repository and clone your fork locally.
2. Create a branch: Create a new branch for your changes:
    ```bash
    git checkout -b my-feature-branch
    ```

## License

This project is licensed under the MIT License—see the `LICENSE.md` file for details.

## Contact

Abhi Mehrotra - <abhimhrtr@pm.com>

## Project Link

[Hydrograph-Versus-Seatek-Sensors-Project](https://github.com/abhimehro/Hydrograph-Versus-Seatek-Sensors-Project)
