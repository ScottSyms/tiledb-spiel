# tiledb-spiel

This project demonstrates how to ingest CSV data into a TileDB sparse array.

## Features

*   **CSV to TileDB:** Ingests data from a CSV file into a TileDB sparse array.
*   **Data Processing:** Processes the data before ingestion, including converting timestamps and handling missing values.
*   **Poetry Support:** Uses Poetry for dependency management.

## Requirements

The dependencies are listed in the `pyproject.toml` file. They include:
*   `tiledb`
*   `pandas`
*   `ipython`
*   `pyarrow`
*   `numpy`
*   `requests`
*   `bs4` (Beautiful Soup)
*   `tiledb-cloud`

## Installation

1.  Clone the repository:
    ```bash
    git clone https://github.com/ScottSyms/tiledb-spiel.git
    cd tiledb-spiel
    ```

2.  Install the dependencies using Poetry:
    ```bash
    pip install poetry
    poetry install
    ```
    Or, install the dependencies using pip:
    ```bash
    pip install tiledb pandas ipython pyarrow numpy requests beautifulsoup4 tiledb-cloud
    ```

## Usage

The main script for ingesting data is `main2.py`.

1.  Make sure you have a `large.csv` file in the root of the project. You can use the `retrievelinks.py` script to download data.
2.  Run the `main2.py` script to create a TileDB sparse array named `sparse` in the root of the project.
    ```bash
    python main2.py
    ```

## Scripts

*   `main.py`: A script for processing a CSV file.
*   `main2.py`: The main script for ingesting CSV data into a TileDB sparse array.
*   `readtest.py`: A script for reading data from the TileDB array.
*   `retrievelinks.py`: A script for downloading data.

## License

This project is licensed under the terms of the LICENSE file.
