# Cryptocurrency Data Fetcher

This Jupyter Notebook retrieves the latest cryptocurrency data from the CoinMarketCap API, processes it, and visualizes trends over time. It fetches real-time information about the top 15 cryptocurrencies by market capitalization.

## Prerequisites

To run this notebook, you'll need to have Python 3.x installed along with the following Python packages:

- `requests`
- `pandas`
- `matplotlib`
- `seaborn`

You can install these dependencies using pip:

```bash
pip install requests pandas matplotlib seaborn

## API Key

To use this notebook, you'll need a CoinMarketCap API key. You can obtain one by signing up at the [CoinMarketCap Developer Portal](https://pro.coinmarketcap.com/). Once you have the API key, replace `'your_api_key_here'` in the notebook with your actual key:

```python
headers = {
  'Accepts': 'application/json',
  'X-CMC_PRO_API_KEY': 'your_api_key_here',
}
```

## Instructions

1. **Clone the Repository:**

   Clone the repository to your local machine using the following command:

   ```bash
   git clone https://github.com/shekharkshitij/Cryptocurrency-Data-Analysis.git
   cd Cryptocurrency-Data-Analysis
   ```

2. **Update API Key:**

   Open the notebook `Automate API Extraction + Appending Data + Extra -- Project.ipynb` and replace the placeholder API key with your actual CoinMarketCap API key as shown above.

3. **Run the Notebook:**

   You can run the notebook by executing:

   ```bash
   jupyter notebook "Automate API Extraction + Appending Data + Extra -- Project.ipynb"
   ```

   Ensure that you are in the directory where the notebook is located.

4. **View the Data:**

   The notebook will retrieve the latest cryptocurrency data and save it in a pandas DataFrame. The data will be normalized and displayed for easy viewing.

   The data can also be saved to a CSV file for future reference. You can modify the CSV file path in the notebook as needed.

5. **Visualize the Data:**

   The notebook includes functionality to visualize data trends over time using Seaborn and Matplotlib.

   It generates a line plot for Bitcoin's price over time and a point plot for percentage changes over different periods.

## Notes

- If you encounter a `KeyError` regarding the `'data'` key, it may be due to exceeding the API rate limit or an issue with your API key.
- Ensure that you adjust the rate limits and API usage according to your subscription plan with CoinMarketCap.

## Troubleshooting

- If you experience data rate issues, try running the following command in your terminal to increase the data rate limit:

  ```bash
  jupyter notebook --NotebookApp.iopub_data_rate_limit=1e10
  ```

- If the data still does not load correctly, verify your API key and check the response from the CoinMarketCap API for error messages.

## Contributing

Feel free to contribute by submitting a pull request or opening an issue.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- This project uses the CoinMarketCap API for data retrieval.
- Visualization is done using Matplotlib and Seaborn.
