# ✈️ Airline Data Analysis — Tableau Dashboard

An interactive Tableau dashboard analyzing airline ticket pricing, routes, and market share across six major Indian cities. Built to explore how price varies by airline, stops, class, booking window, and source–destination pairs.

![Dashboard Overview](https://github.com/SugamSagar-DS458/Airline-Data-Analysis-Tableau-Dashboard/blob/main/Screenshot%202026-08-20%20133214.png)

---

## 📊 Overview

| Metric | Description |
|---|---|
| **Total Airlines** | 6 carriers tracked (Air India, AirAsia, GO_FIRST, Indigo, SpiceJet, Vistara) |
| **Total Flights** | 1,561 records |
| **Total Cities** | 6 (Bangalore, Chennai, Delhi, Hyderabad, Kolkata, Mumbai) |
| **Avg Ticket Price** | ₹20,890 |
| **Avg Economy Fare** | ₹6,572 |
| **Avg Business Fare** | ₹52,540 |

## 🔍 What the Dashboard Shows

- **KPI Summary Cards** — total airlines, flights, cities, and average fares at a glance
- **Stop Price Analysis** — average fare by number of stops (zero / one / two-or-more), split by class
- **Price vs Days Left** — how ticket price trends as the departure date approaches, by class
- **Avg Fare by Airline** — bar chart comparing average fares across carriers
- **Departure vs Arrival Price** — heatmap-style matrix of price by departure/arrival time-of-day
- **Source → Destination Price** — cross-tab of average fare between every city pair
- **Airline Market Share** — donut/pie chart of flight volume by airline (used as a click-to-filter control)

## 🖱️ Interactivity

- **Class filter** (dropdown, top-right) — filters the whole dashboard by Economy / Business / All
- **Click-to-filter on the Airline Market Share chart** — clicking a slice (e.g. Air India, Vistara) cross-filters every other chart on the dashboard to that airline
- **NEXT navigation button** — moves to the next view/story point in the workbook

## 🗂️ Repository Structure

```
Airline-Data-Analysis-Tableau/
├── README.md                  # You are here
├── tableau/
│   ├── Airline_Data_Analysis.twbx   # (add your packaged workbook here)
│   └── README.md               # Notes on the workbook, sheets, and calc fields
├── data/
│   ├── airline_data.csv        # (add your source dataset here)
│   └── README.md                # Data dictionary / column descriptions
└── docs/
    ├── measures.md             # Calculated fields & measures used
    └── images/                 # Dashboard screenshots for README/docs
```

## 🚀 Getting Started

1. **Clone the repo**
   ```bash
   git clone https://github.com/<your-username>/Airline-Data-Analysis-Tableau.git
   cd Airline-Data-Analysis-Tableau
   ```
2. **Open the workbook**
   - [Tableau Public](https://public.tableau.com/).
   - [Open](https://github.com/SugamSagar-DS458/Airline-Data-Analysis-Tableau-Dashboard/blob/main/Airline_Price_Analysis_Tableau.twbx)
   - 
3. **Data source**
   - The packaged workbook (`.twbx`) already embeds the data extract, so no extra setup is needed.
   - [If you want to rebuild from raw data, point the workbook's data connection to](https://github.com/SugamSagar-DS458/Airline-Data-Analysis-Tableau-Dashboard/blob/main/Airline%20Data.xlsx)

## 🧮 Tech / Tools

- **Tableau Desktop / Public** — dashboard authoring
- **CSV** — underlying flight-price dataset

## 🔗 Live Dashboard

> [My Public Dashboard](https://public.tableau.com/views/Airline_Price_Analysis/Dashboard1?:language=en-GB&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## 📈 Key Insights

- Indigo holds the largest market share (45.1%) by flight volume, followed by GO_FIRST (13.1%) and Air India (14.0%).
- Business class fares average roughly **8x** economy fares (₹52,540 vs ₹6,572).
- Prices generally trend downward the further out a ticket is booked, then spike as the departure date nears.
- Flights with two-or-more stops show the widest fare variance across the dataset.

## 🙌 Acknowledgements

Dashboard designed and built in Tableau as part of a personal data analytics portfolio project.
