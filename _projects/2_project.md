---
layout: page
title: Corona App
description: Real-time COVID-19 Tracker App Using Flutter & REST API
img: assets/img/corona_app_banner.png
importance: 2
category: Development Projects
related_publications: false
giscus_comments: true
---

# Corona App – COVID-19 Tracker

**Corona App** is a mobile application built using **Flutter** that provides **real-time COVID-19 statistics** across the globe and per country. It utilizes REST APIs to fetch live data, visualizes it in charts and cards, and offers a user-friendly dashboard.

This project was designed to help users stay informed about the latest developments during the COVID-19 pandemic with accurate and up-to-date data.

---

## 🔍 Features

- 🌐 Global & Country-wise COVID-19 tracking  
- 📊 Real-time statistics (confirmed, active, recovered, deaths)  
- 📈 Pie chart & card-based visualizations  
- 🌙 Dark and Light UI themes  
- 🔁 Pull-to-refresh and API updates  
- 💡 Flutter UI design and responsive layout  

---

## 🧩 Tech Stack

- **Frontend**: Flutter (Dart)  
- **Backend/API**: Public REST COVID-19 APIs (e.g., [https://disease.sh](https://disease.sh))  
- **State Management**: `setState()` (basic), with scope for provider integration  
- **Chart Visualization**: Pie chart using `fl_chart` package  

---

## 📸 Screenshots

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/corona_dashboard.png" title="Main Dashboard" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/corona_countrywise.png" title="Country-Wise Stats" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/corona_piechart.png" title="Data Visualization" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

<div class="caption">
  Dashboard showing global stats, country-specific breakdown, and pie chart data visualization.
</div>

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/mdakilraihaniftee/Corona-App.git
