# Predii_RAG
This repository contains a Jupyter Notebook for processing vehicle recall data. The notebook defines a class-based pipeline to load, clean, and filter tab-separated recall datasets. It is designed for analyzing vehicle recall records and filtering data based on specific manufacturers.

Features

Data Loading: Reads tab-separated data files into a pandas DataFrame.

Data Cleaning: Removes unnecessary columns, renames columns, and consolidates additional fields.

Data Filtering: Filters records for specific manufacturers (e.g., FORD and TOYOTA).

File Structure

preddii.ipynb: Jupyter Notebook containing the implementation and usage example.

FLAT_RCL.txt (not included): Example input dataset for processing.

Prerequisites

Python 3.x

Jupyter Notebook

Required Python Libraries:

pandas

Usage

Clone the Repository:

git clone https://github.com/yourusername/recall-data-processor.git
cd recall-data-processor

Install Dependencies:
Install the required Python libraries:

pip install pandas

Run the Notebook:
Launch Jupyter Notebook and open preddii.ipynb:

jupyter notebook

Prepare the Input File:
Place your tab-separated input file (FLAT_RCL.txt) in the appropriate directory. Update the file path in the notebook accordingly.

Execute the Notebook:
Run all cells in the notebook to:

Load and process the input data.

Display processed data.

Generate filtered datasets for FORD and TOYOTA.

Example

Input Data

The input dataset (FLAT_RCL.txt) should be a tab-separated file with recall information.

Sample Output

The notebook processes the dataset and generates:

A cleaned DataFrame with columns: RECALL_NUMBER, MAKE, MODEL, YEAR, and Extra.

A filtered DataFrame containing only records for FORD and TOYOTA vehicles.

Code Overview

RecallDataProcessor Class

Methods:

load_data: Loads the tab-separated input file into a DataFrame.

clean_data: Cleans and restructures the DataFrame.

get_processed_data: Returns the cleaned DataFrame.

filter_ford_toyota Function

Filters the cleaned DataFrame for records where the MAKE column is either FORD or TOYOTA.
