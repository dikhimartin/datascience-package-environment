# Data Science Package Environment

## Description

This repository provides the necessary configuration and environment for **Data Science** projects using **Conda** to manage packages and dependencies. The environment includes libraries for data analysis, visualization, and machine learning. Users can download and set up this environment using the `environment.yml` file for a consistent and reproducible project setup.

## Features

- **Jupyter Lab** for interactive data exploration
- **Pandas**, **NumPy**, **Matplotlib** for data analysis and visualization
- **Scikit-learn** for basic machine learning models
- **DuckDB** for SQL-based data analysis
- **PyGWalker** for interactive data visualization

## Prerequisites

Ensure that **Miniconda** or **Anaconda** is installed on your system.

## Installation

1. **Clone this repository:**

   ```bash
   git clone https://github.com/username/datascience-package-environment.git
   cd datascience-package-environment
   ```

2. **Create the Conda environment from the `environment.yml` file:**

   ```bash
   conda env create -f environment.yml
   ```

3. **Activate the Conda environment:**

   ```bash
   conda activate datascience_package
   ```

4. **Install Jupyter Lab if it's not already installed:**

   ```bash
   conda install -c conda-forge jupyterlab
   ```

5. **Run Jupyter Lab:**

   ```bash
   jupyter lab
   ```

   If you're using Visual Studio Code, make sure the Python and Jupyter extensions are installed, then select the `datascience_package` kernel to run the notebook.

## Running the Project

Once the environment is activated, you can open the `main.ipynb` file to perform data analysis and verify that all libraries are working correctly. This notebook includes examples using the main libraries, including data visualization and simple machine learning model creation.

## Troubleshooting

If you encounter issues while running the environment or Jupyter Lab, try the following steps:

- **Make sure the correct kernel is selected in Jupyter Lab or VSCode** (kernel `datascience_package`).

- Jupyter Lab not starting?

   Try reinstalling it with:

  ```bash
  conda install -c conda-forge jupyterlab
  ```

- Error activating environment:

   If you get an error like 

  ```
  CondaError: Run 'conda init' before 'conda activate'
  ```

  , run:

  ```bash
  conda init
  ```

## Repository Structure

```
datascience-package-environment/
├── environment.yml         # Conda environment configuration
├── main.ipynb              # Main notebook for data analysis
└── README.md               # Project documentation
```

## License

This project is licensed under the [MIT License](https://chatgpt.com/c/LICENSE).