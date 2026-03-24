# MITECO Hydrological Bulletin Scraper

A Python-based web scraper built with Selenium and Pandas to automate the extraction of daily hydrological data from the Spanish Ministry for the Ecological Transition and the Demographic Challenge (MITECO).

The script navigates the [Hydrological Bulletin Portal (BoleHWeb)](https://www.miteco.gob.es/es/agua/temas/evaluacion-de-los-recursos-hidricos/boletin-hidrologico.html), iterates through the calendar, extracts summary tables, and compiles the data into a clean, structured CSV file.

## Features

* **Automated Navigation:** Handles cookie banners and pop-up windows automatically.
* **Historical Data Extraction:** Iterates through months and years (from 2023 to the current year) to collect daily reports.
* **Smart CSV Saving:** Appends new data to an existing CSV file (`historic_boletin_miteco.csv`) and automatically drops duplicated entries based on the date.
* **Error Handling:** Built-in mechanisms to retry and recover if the portal's session expires or a page fails to load.

## Prerequisites

Before running the script, ensure you have the following installed:

* [Python 3.7+](https://www.python.org/downloads/)
* Google Chrome Browser

## Installation

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
   cd YOUR_REPO_NAME
