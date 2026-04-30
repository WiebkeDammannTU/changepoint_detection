# Changepoint Detection (R Shiny App)

An interactive **R Shiny application** for detecting and visualizing changepoints in time series data.

🔗 https://wiebkedammanntu.github.io/changepoint_detection/

---

## 🧭 Overview

This application enables users to:

- 📤 Upload time series datasets *(or use a built-in example dataset)*  
- 📊 Visualize measurements over time  
- 🔍 **Detect changepoints** using the R package `changepoint`  
  (DOI: 10.32614/CRAN.package.changepoint)  
- ⚙️ Adjust detection sensitivity via a penalty parameter  
- 🧩 Explore changepoints across multiple variables  
- 📋 View detected changepoints and corresponding **segment means** in a table  
- 📄 Export results as an **HTML report**  

---

## 📥 Input Data Format

The app expects an Excel file (`.xlsx`) with the following columns:

| Column        | Description                                                  |
|---------------|--------------------------------------------------------------|
| `variable`    | Measured variable (e.g. laboratory endpoint)                |
| `date`        | Date of the measurement                                      |
| `measurement` | Numeric measurement value                                    |
| `group`       | *(Optional)* grouping variable used for coloring (e.g. company) |

➡️ An example dataset is included in the app and can also be downloaded.

---

## 📊 Changepoint Detection

Changepoints are estimated using the R package `changepoint`.  
It implements a likelihood-based method for detecting changes in the mean, assuming a constant mean within segments.

A key component of the approach is the penalty term, which controls the sensitivity of the detection and can be adjusted manually.

The **penalty value** controls detection sensitivity:

- 🔽 Low values → more changepoints *(higher sensitivity)*  
- 🔼 High values → fewer changepoints *(lower sensitivity)*  
- ⚖️ Default: `25` *(balanced choice)*  

---

## 🔎 Visualization Features

- **Zoom functionality:** Select a region along the x-axis to zoom in.  
  Use the reset button (right side of the plot) to return to the full view.  
- **Variable ordering in the plot:**
  - Alphabetical order  
  - By most recent changepoint (variables with later changepoints appear at the top)  

---

## 🧪 Example Dataset

The example dataset is provided for demonstration purposes.

It contains data from five laboratory endpoints derived from control animals in the VICT3R database (https://www.vict3r.eu/). The dataset has the following characteristics:

- Origin: multiple pharmaceutical companies ("groups", labeled A–J)  
- Study type: 28-day toxicity studies  
- Species: male Sprague-Dawley rats  

The dataset can be downloaded directly within the app.

---

## 👩‍💻 Author

Developed by  
**Wiebke Dammann**, **Kai Kammers**, **Jörg Rahnenführer**

---

## 📬 Feedback & Questions

If you have any questions, suggestions, or feedback, please send an email:

📧 dammann@statistik.tu-dortmund.de

We appreciate your feedback!
