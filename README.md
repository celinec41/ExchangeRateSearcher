# ExchangeRateSearcher

This script fetches **USD/CNY**, **EUR/CNY**, **JPY/CNY**, and **Shanghai Gold AU99.99** prices from **WindPy** and plots them using **Matplotlib**.

---
## Features

* Get data directly from Wind Financial Terminal
* Dual-axis plot: FX (left) and Gold (right)
* Saves chart as a PNG file
* Supports Chinese fonts for labels

---

## Requirements

* Python 3.9+
* Logged in to **Wind Terminal**
* Libraries:

  ```bash
  pip install pandas matplotlib
  ```

  *(WindPy is installed with the Wind Terminal)*

---

## How to Run

1. Make sure Wind is open and logged in.
2. Run the script:

   ```bash
   python fx_gold_plot.py
   ```
3. Enter the start and end month (format: `YYYY-MM`).
4. The program will show a chart and save it as a PNG.

---

## Notes

* If WindPy is not connected → log in to the Wind Terminal first.
* If data is empty → your account may not have access to some symbols.
* To change fonts:

  ```python
  plt.rcParams['font.family'] = 'SimHei'  # for Windows
  ```

---

## Output Example

* **Left axis:** Exchange rates (USD, EUR, JPY → CNY)
* **Right axis:** Gold price (AU99.99)
* **File saved:** `2025-11-08_23-15-12.png`

