# SafeCREW-T4.1-NOM-anthropogenic-impact

## Overview

This repository contains the analyses performed for the paper *Adapting to Climate Change: Evaluating the role of human activities on the quality of source waters for drinking water production*, part of the [EU-funded SafeCREW project](https://safecrew.org).

## 🗂️ Project Structure

- **`safecrew_t4/`**: Contains the core modules and scripts for data processing and analysis.
    - **`tarragona/`**: Contains scripts tailored for the Tarragona case study. This includes:
        - `1-preprocessing.ipynb`: Data preprocessing steps including formatting, filtering, and merging for Tarragona datasets.
        - `2-trend-analysis.ipynb`: Trend estimation and evaluation for each environmental variable.
    - **`berlin/`**: Contains scripts tailored for the Berlin case study. This includes:
        - `1-preprocessing.ipynb`: Data preprocessing steps including formatting, filtering, and merging for Berlin datasets.
        - `2-trend-analysis.ipynb`: Trend estimation and evaluation for each environmental variable.
        - `3-segmented-reg-analysis-305.ipynb`: Applies piecewise (segmented) regression to explore potential breakpoints in every environmental variable in the Upper Havel station (305).
        - `4-segmented-reg-analysis-325.ipynb`: Same as above but for the Lower Havel station (325).
- **`.vscode/`**: Configuration files for Visual Studio Code.
- **`pyproject.toml` & `poetry.lock`**: Define the project's dependencies and environment settings using Poetry.
- **`README.md`**: This documentation file.
- **`LICENSE`**: The project's MIT license.

## Getting Started

### Prerequisites

- [Python 3.11](https://www.python.org/downloads/release/python-3110/) or higher;
- [Poetry](https://python-poetry.org/) for dependency management.

### Installation

Clone the repository and install the environment with Poetry:

```bash
git clone https://github.com/MassimilianoArca/SafeCREW-T4.1-NOM-anthropogenic-impact.git
cd SafeCREW-T4.1-NOM-anthropogenic-impact
poetry install
poetry shell
```

## 📊 Usage

For a complete pipeline, follow the numerical order of the notebooks within each site folder.

Before running any notebook, you need to create a **`data/`** directory inside **`safecrew_t4/`**, structured as follows:
- **`data/`**
    - **`tarragona/`**
    - **`berlin/`**

Each subfolder must contain the relevant datasets for the corresponding case study. The required data can be downloaded from [Zenodo](somelink). Make sure the files are placed in the correct subdirectories before execution.