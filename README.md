# 🕸️ Advanced Web Scraper Hub (Scrapy)

A collection of high-performance web spiders built with the **Scrapy** framework in Python. This project demonstrates advanced data extraction techniques from various web structures, including product grids, complex tables, and multi-page pagination.

## 🎯 Project Objectives
The goal of this project is to automate the data collection process from multiple sources and store them in structured formats like **CSV** or **JSON** for further analysis.

## ✨ Key Features
*   **Multi-Spider Architecture:** Dedicated spiders for different web domains (Books, Sports, Geography).
*   **Automated Pagination:** Seamlessly navigates through hundreds of pages using Scrapy's `response.follow`.
*   **Data Cleaning:** Implements `normalize-space()` and `.strip()` to ensure noise-free, production-ready data.
*   **Asynchronous Processing:** Built to handle requests efficiently with high-speed performance.

## 🛠️ Tech Stack
*   **Language:** Python 3.10+
*   **Framework:** Scrapy
*   **Selectors:** XPath (Primary) & CSS Selectors

## 📂 Spiders Overview
1.  **`book_spider`**: Scrapes 1,000+ books from *Books to Scrape*, capturing titles, prices, and stock availability.
2.  **`hocky_spider`**: Extracts historical hockey team data, including win/loss records, goals, and percentages across 24+ pages.
3.  **`scrape_spider`**: Collects geographical data for all countries worldwide, including capitals, populations, and areas.

## 💻 Installation & Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   cd your-repo-name
   ```

2. **Install Scrapy:**
   ```bash
   pip install scrapy
   ```

3. **Run a specific spider:**
   To run the Hockey spider and save data to a CSV file:
   ```bash
   scrapy crawl hocky_spider -O results.csv
   ```

## 📊 Sample Output Fields
The spiders extract the following key data points:
*   **Team/Book Name**
*   **Year/Price**
*   **Wins/Losses/Stock Status**
*   **Win % / Goals For / Goals Against**

---
⭐ **If you find this project helpful, please give it a Star!**
