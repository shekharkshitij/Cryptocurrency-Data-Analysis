```markdown
# Cryptocurrency Data Fetcher

This script retrieves the latest cryptocurrency data from the CoinMarketCap API, processes the data, and visualizes trends over time. It uses the CoinMarketCap API to get real-time information about the top 15 cryptocurrencies by market capitalization.

## Prerequisites

To run this script, you'll need to have Python 3.x installed along with the following Python packages:

- `requests`
- `pandas`
- `matplotlib`
- `seaborn`

You can install these dependencies using pip:

```bash
pip install requests pandas matplotlib seaborn
```

## API Key

To use this script, you'll need a CoinMarketCap API key. You can obtain one by signing up at [CoinMarketCap Developer Portal](https://pro.coinmarketcap.com/). Once you have the API key, replace `'your_api_key_here'` in the script with your actual key.

## Instructions

1. **Clone the Repository:**

   Clone the repository to your local machine using the following command:

   ```bash
   git clone https://github.com/shekharkshitij/Cryptocurrency-Data-Analysis.git
   cd cryptocurrency-data-fetcher
   ```

2. **Update API Key:**

   Open the script `/Automate API Extraction + Appending Data + Extra -- Project.ipynb` and replace the placeholder API key with your actual CoinMarketCap API key:

   ```python
   headers = {
     'Accepts': 'application/json',
     'X-CMC_PRO_API_KEY': 'your_api_key_here',
   }
   ```

3. **Run the Script:**

   You can run the script by executing:

   ```bash
   jupyter notebook "Automate API Extraction + Appending Data + Extra -- Project.ipynb"
   ```

   Make sure you are in the directory where the script is located.

4. **View the Data:**

   The script will retrieve the latest cryptocurrency data and save it in a pandas DataFrame. The data will be normalized and displayed for easy viewing. 

   It will also save the data to a CSV file for future reference. The CSV file path can be modified in the script as needed.

5. **Visualize the Data:**

   The script includes functionality to visualize the data trends over time using Seaborn and Matplotlib. 

   It generates a line plot for Bitcoin's price over time and a point plot for percentage changes over different periods.

## Notes

- If you encounter a `KeyError` regarding the `'data'` key, it may be due to exceeding the API rate limit or a problem with your API key.
- Make sure to adjust the rate limits and API usage as per your subscription plan with CoinMarketCap.

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

```
