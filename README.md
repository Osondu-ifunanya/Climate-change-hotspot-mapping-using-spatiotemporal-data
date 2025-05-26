# Climate Change Hotspot Mapping 

This project simulates climate change hotspot mapping using synthetic spatiotemporal temperature anomaly data. It demonstrates how temperature trends over time can be analyzed to identify regions experiencing statistically significant warming — referred to as *hotspots*.

---

## 📊 Project Description

- A synthetic 50x50 spatial grid is generated, representing hypothetical locations.
- Each grid cell has yearly temperature anomaly data from **2000 to 2020**.
- A linear regression is applied to each pixel to estimate the warming trend over time.
- Hotspots are identified as cells with:
  - A statistically significant **positive slope** in the regression (p < 0.05)
  - A slope greater than a defined threshold (**0.02°C/year**)

---

## 🛠️ Technologies Used

- Python 3
- NumPy
- SciPy
- Pandas
- Matplotlib
- Seaborn

---

## 📁 Files

- `climate_hotspots_synthetic.xlsx`: Contains all simulated temperature anomaly data, slope values, p-values, and hotspot flags for each grid cell.
- `hotspot_mapping.py` *(optional)*: Python script to generate the data and visualizations.
- `README.md`: This file.

---

## 📤 Output Columns in Excel

| Column        | Description                                      |
|---------------|--------------------------------------------------|
| `Row`, `Col`  | Spatial grid indices                             |
| `Slope`       | Linear regression slope of temperature anomaly   |
| `P_value`     | P-value for the regression trend significance    |
| `Hotspot`     | 1 = Hotspot (significant warming), 0 = not       |
| `Temp_YYYY`   | Temperature anomaly for each year 2000–2020      |

---

## ✍️ Author

Ifunanya  Osonduifunaya77@gmail.com

---

## 📘 License

This project is open for educational and non-commercial use. Feel free to modify and expand it.

