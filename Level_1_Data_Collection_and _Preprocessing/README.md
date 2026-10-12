CBN Exchange Rate Data Collection, Cleaning and Preprocessing

Project Overview

This project was completed as part of the Codveda Technology Data Science Internship — Level 1. It covers two tasks: Data Collection and Web Scraping, and Data Cleaning and Preprocessing.

The project uses historical exchange-rate data from the Central Bank of Nigeria (CBN). The data was collected, cleaned, validated, encoded, and standardized to produce datasets suitable for further analysis and machine learning.

Tasks Completed

Task 1: Data Collection and Web Scraping

The CBN historical exchange-rate data was initially investigated using Python’s requests and BeautifulSoup libraries. However, the webpage response did not expose the required exchange-rate records in the expected structure.

The collection method was therefore adjusted to use the CBN exchange-rate API endpoint, GetAllExchangeRates, which returned the records in JSON format.

The response was inspected, converted into a pandas DataFrame, and exported to CSV.

Original dataset: 62,333 records and 6 columns.

Task 2: Data Cleaning and Preprocessing

The following steps were performed:

* Currency label standardization: Inconsistent currency names and capitalization were standardized.
* Duplicate removal: 37 duplicate observations were removed using currency, date, and exchange-rate values for comparison.
* Anomaly investigation: Suspicious exchange-rate values were investigated using screening rules and comparisons with neighbouring dates. Confirmed isolated anomalies were removed.
* Rate validation: Non-positive rates and records meeting the project’s extreme rate-difference screening rule were checked.
* Rate-order checks: Records where buying, central, and selling rates did not follow the expected order were flagged. Remaining violations were retained because a violation alone does not establish that a record is erroneous.
* Date conversion: The ratedate column was converted to a datetime data type.
* Numerical conversion: Exchange-rate columns were converted to numeric data types.
* One-hot encoding: The categorical currency column was converted into binary currency indicator columns.
* Standardization: The buying, central, and selling rates were standardized using scikit-learn’s StandardScaler.

The original raw dataset was preserved, while the cleaned and preprocessed datasets were saved separately.

Final Results

The cleaned dataset contains 62,250 records and 6 columns.

The preprocessed dataset contains 62,250 records and 20 columns, including the retained ID and date columns, standardized exchange-rate columns, and one-hot-encoded currency columns.

Final validation confirmed that the cleaned dataset had no missing values, exact duplicate records, invalid dates, non-positive exchange rates, or remaining records meeting the defined extreme rate-difference screening rule. Some rate-order violations remained documented rather than being removed automatically.

Project Files

File	Description
CBN_Exchange_Rate_Scraping.ipynb	Notebook containing the collection, cleaning, preprocessing, and validation workflow
cbn_exchange_rates_raw.csv	Original collected data, preserved unchanged
cbn_exchange_rates_cleaned.csv	Cleaned exchange-rate data
cbn_exchange_rates_preprocessed.csv	Encoded and standardized data
README.md	Project overview, methodology, and results

Technologies Used

* Python
* Requests
* BeautifulSoup
* Pandas
* NumPy
* scikit-learn
* Jupyter Notebook
* Visual Studio Code

How to Run the Project

1. Clone or download the repository.
2. Install the required libraries:

pip install pandas numpy requests beautifulsoup4 scikit-learn jupyter

3. Open CBN_Exchange_Rate_Scraping.ipynb in Jupyter Notebook or Visual Studio Code.
4. Run the notebook cells in order.

The notebook collects data through the CBN API. Running the collection cells requires internet access and the API to remain accessible.

Limitations and Notes

* The extreme-value screening rules used in this project are project-specific checks, not official CBN data-validation rules.
* Rate-order violations were retained where the available evidence was insufficient to classify the observations as errors.
* Standardization was performed to demonstrate preprocessing; standardized values are not the original exchange rates.
* The raw CSV was preserved to support traceability and comparison with the cleaned data.

Internship Context

This project demonstrates practical experience in data collection, data quality checks, cleaning, categorical encoding, numerical standardization, and reproducible notebook workflows as part of the Codveda Technology Data Science Internship.