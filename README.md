# IPL Bar Chart Race 🏏📊

An animated bar chart race visualizing **cumulative IPL team wins over seasons**, built using **Python, Pandas, and Matplotlib**.  
This project showcases data processing, time-series analysis, and animated data storytelling.

---

## 📌 Project Overview

The Indian Premier League (IPL) has evolved significantly over the years, with teams rising and falling in dominance.  
This project transforms historical IPL match data into a **dynamic bar chart race**, allowing viewers to visually track how teams accumulate wins season by season.

---

## 📂 Data Source

- **Cricsheet (IPL match data)**  
- Format: Raw JSON files (one file per match)

The project involves:
- Parsing raw JSON data  
- Converting it into structured CSV format  
- Cleaning team name inconsistencies  
- Computing cumulative wins over time  

---

## 🛠️ Tech Stack

- **Python**
- **Pandas** – data manipulation & aggregation  
- **NumPy** – numerical operations  
- **Matplotlib** – animation & visualization  
- **FFmpeg / Pillow** – saving animations  

---

## 📁 Project Structure

ipl-bar-chart-race/
│
├── data/
│ ├── raw/
│ │ └── ipl_json/ # Raw Cricsheet IPL JSON files
│ └── processed/
│ ├── ipl_matches_raw.csv
│ ├── ipl_matches_clean.csv
│ └── ipl_cumulative_wins.csv
│
├── notebooks/
│ ├── 01_json_to_csv.ipynb
│ ├── 02_data_cleaning.ipynb
│ ├── 03_prepare_animation.ipynb
│ └── 04_bar_chart_race.ipynb
│
├── outputs/
│ ├── ipl_bar_chart_race.gif
│ └── ipl_bar_chart_race.mp4
│
├── README.md
└── requirements.txt

## ⚙️ How It Works

1. **JSON → CSV Conversion**  
   Extracts season and match winner from raw Cricsheet JSON files.

2. **Data Cleaning**  
   Handles team name changes (e.g., Delhi Daredevils → Delhi Capitals).

3. **Feature Engineering**  
   Calculates season-wise and cumulative team wins.

4. **Visualization**  
   Generates a smooth animated bar chart race with:
   - Team colors  
   - Rank labels  
   - Value annotations  
   - Smooth transitions  

---

## ▶️ How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/<your-username>/ipl-bar-chart-race.git
   cd ipl-bar-chart-race

Install dependencies:

pip install -r requirements.txt


Open Jupyter Notebook:

jupyter notebook

Run notebooks in order from the notebooks/ folder:

01_json_to_csv.ipynb

02_data_cleaning.ipynb

03_prepare_animation.ipynb

04_bar_chart_race.ipynb