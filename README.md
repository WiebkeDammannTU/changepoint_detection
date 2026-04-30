# 📈 changepoint_detection

R Shiny application – changepoint detection

🔗 https://wiebkedammanntu.github.io/changepoint_detection/

---

## 🧭 Overview

This application enables users to:

- 📤 Upload time series datasets  
- 🔍 Detect changepoints using configurable penalty values  
- 📊 Visualize measurements over time  
- 🧩 Explore segment-wise changes across multiple variables  
- 📄 Export results as an HTML report  
- ⬇️ Download example datasets  

---

## ✨ Features

- 📊 Interactive visualization with faceted plots  
- 🔍 Changepoint detection using the `changepoint` package  
- ⚙️ Adjustable sensitivity via penalty parameter  
- 🧠 Multi-variable support  
- 🔎 Zoom functionality  
- 📄 Report generation (HTML)  
- ⬇️ Example dataset download  

---

## 📥 Input Data Format

The app expects an Excel file (`.xlsx`) with the following columns:

| Column        | Description                                     |
|---------------|-------------------------------------------------|
| `variable`    | Measured variable (e.g. lab endpoint)           |
| `date`        | Date of measurement                            |
| `measurement` | Numeric value                                  |
| `group`       | *(Optional)* grouping variable                 |
