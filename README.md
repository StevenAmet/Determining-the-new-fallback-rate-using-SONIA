# Determining the New Fallback Rate Using SONIA

## Project Summary

This project demonstrates the process of calculating and analyzing a new financial “fallback rate” based on SONIA (Sterling Overnight Index Average). Using Python and Jupyter Notebook, the analysis explores how to work with historical SONIA data, visualize rate changes, and estimate substitute rates in the context of risk-free reference rates in financial contracts.

## Features / Usage

- Download and process SONIA and other rate data using Python
- Visualize interest rate movements with clear plots
- Calculate statistics and compare fallback rates versus previous benchmarks
- Provide example methodologies for fallback rate determination
- All core logic and analysis implemented in a clear, step-by-step Jupyter Notebook

## How to Install / Run the Code

1. **Clone the repository:**
    ```bash
    git clone https://github.com/StevenAmet/Determining-the-new-fallback-rate-using-SONIA.git
    cd Determining-the-new-fallback-rate-using-SONIA
    ```

2. **(Optional) Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    # On Windows:
    venv\Scripts\activate
    # On macOS/Linux:
    source venv/bin/activate
    ```

3. **Install dependencies:**
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```

4. **Run the notebook:**
    ```bash
    jupyter notebook
    ```
    Then open `Determining the new 'fallback rate' using SONIA.ipynb`.

## Example Usage

```python
import pandas as pd
import matplotlib.pyplot as plt

# Load SONIA historical data
sonia_data = pd.read_csv("sonia-historical.csv", parse_dates=['Date'])
plt.figure(figsize=(10,5))
plt.plot(sonia_data['Date'], sonia_data['SONIA'])
plt.title("SONIA Daily Rate Over Time")
plt.xlabel("Date")
plt.ylabel("SONIA Rate (%)")
plt.grid()
plt.show()
```

## Dependencies

- pandas
- numpy
- matplotlib
- seaborn


