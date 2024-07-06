# Options-Gamma-Exposure-Analysis-Tool
This script scrapes options data for a specified stock ticker from the CBOE website, calculates the total Gamma Exposure (GEX) for options expiring on a specified date, and visualizes the GEX by strike price. It also identifies the strike price where the Gamma Exposure crosses zero.

The provided script is a Python program designed to scrape and analyze options data for a given stock ticker from the CBOE (Chicago Board Options Exchange) website. It calculates the total Gamma Exposure (GEX) for options expiring on a specified date and visualizes the GEX by strike price.

# Main functions and their roles:

# run(ticker, expiration_date):
Converts the expiration date to the required format.
Scrapes data for the given ticker and expiration date.
Computes and prints the total GEX.
Computes GEX by strike price and plots it.
Calculates and prints the strike price with zero GEX.

# scrape_data(ticker, expiration_date):
Fetches the options data from the CBOE website for the given ticker.
Fixes the options data and filters it based on the expiration date.

# filter_data_by_expiration(data, expiration_date):
Filters the options data for the specified expiration date.

# fix_option_data(data):
Extracts and fixes various columns (like option type, strike price, and expiration date) from the options data.

# compute_total_gex(spot, data):
Computes the total Gamma Exposure (GEX) for the given options data and prints the total notional GEX.

# calculate_zero_gex_level(data):
Calculates and prints the strike price where the Gamma Exposure (GEX) crosses zero.

# compute_gex_by_strike(spot, data):
Computes and plots the Gamma Exposure (GEX) by strike price using Plotly.

###############################################################################################################################################3

# Options Gamma Exposure Analysis Tool
This project is a Python script that scrapes options data for a given stock ticker from the CBOE (Chicago Board Options Exchange) website, calculates the total Gamma Exposure (GEX) for options expiring on a specified date, and visualizes the GEX by strike price. It also identifies the strike price where the Gamma Exposure crosses zero.

# Features
Scrapes options data from the CBOE website.
Computes total Gamma Exposure (GEX) for a specified expiration date.
Visualizes GEX by strike price.
Identifies the strike price where GEX crosses zero.

# Requirements
Python 3.x
pandas
requests
matplotlib
plotly
