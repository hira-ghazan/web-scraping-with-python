# web-scraping-with-python# Web Scraping & AI Data Extraction
This repository contains Python-based projects focused on automated data collection, HTML parsing, and structured data preparation using industry-standard libraries.

---

## Project 1: Tutorial Freak - Manual Web Scraping
This project serves as a foundational tutorial for navigating and extracting content from [Tutorial Freak](https://www.tutorialfreak.com/). It focuses on understanding the underlying HTML structure and retrieving data manually.

### Core Implementation:
*   **Request Management:** Used the `requests` library to fetch raw HTML content, ensuring proper user-agent headers to mimic browser behavior.
*   **DOM Parsing:** Employed `BeautifulSoup` to navigate the nested tags of the website.
*   **Targeted Scraping:**
    *   Extracted tutorial titles and descriptions.
    *   Collected internal links to map out site navigation.
    *   Identified specific `div` classes and `id` attributes to isolate high-value content.

### Tools Used:
*   **Python Libraries:** `requests`, `BeautifulSoup4`
*   **Key Techniques:** HTML Tag traversal, CSS Class selection, and Prettify for code inspection.


## Project 2: Books to Scrape - AI & Automation
A more advanced implementation targeting [Books to Scrape](https://books.toscrape.com/), designed to handle pagination and prepare a large dataset for AI-driven analysis.

### Workflow & Data Pipeline:
*   **Automated Navigation:** Implemented a pagination script that automatically crawls through all 50 pages of the catalog without manual intervention.
*   **Data Extraction & Cleaning:** 
    *   **Titles & Prices:** Captured book titles and prices, using Python to strip currency symbols and convert values to `float`.
    *   **Availability:** Scraped stock status and converted it into a boolean format.
    *   **Rating Conversion:** Built a dictionary mapping to convert text-based ratings (e.g., "Four") into numerical integers (4) for statistical use.
*   **AI Readiness:** The resulting CSV file is structured specifically for training recommendation engines or performing sentiment analysis on book categories.

### Technical Achievements:
*   **Data Integrity:** Validated 1,000+ entries to ensure no missing values during the scraping process.
*   **Efficient Storage:** Exported the final cleaned dataset into a `.csv` file using `pandas` for immediate use in machine learning models.

---

## Technical Stack
*   **Languages:** Python 3.x
*   **Parsing:** BeautifulSoup4, lxml
*   **Networking:** Requests
*   **Data Processing:** Pandas, NumPy
*   **Environment:** Jupyter Notebook / VS Code
