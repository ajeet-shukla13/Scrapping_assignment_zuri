# Web Scraping Assignment – Myntra & NykaaFashion

Submitted by: Ajeet Kumar Shukla  
Role: App Developer  
Company: Zuri  
Assignment Goal: Extract structured fashion product data from Myntra and Nykaa Fashion using Python and Selenium.

---

## Overview

This project scrapes structured product details from two e-commerce websites:

- [Myntra](https://www.myntra.com)
- [Nykaa Fashion](https://www.nykaafashion.com)

The scraper targets 10 popular fashion-related search keywords and retrieves the top 10 product results per keyword.

---

## Tech Stack

- Python 3.x
- Selenium WebDriver
- ChromeDriver Manager
- JSON for output format

---

## Function Details

### `def scrape_myntra(KEYWORDS, browser)`
- Navigates to Myntra homepage
- Searches each keyword
- Extracts top 10 product links
- For each product, scrapes:
  - Brand  
  - Product Name  
  - Original Price  
  - Discounted Price  
  - Product Image URL  
  - Ratings  
  - Reviews  
  - Available Sizes (with stock status)  

### `def scrape_nykaa(KEYWORDS, browser)`
- Handles "No Thanks" popup
- Searches each keyword
- Extracts top 10 product links
- For each product, scrapes:
  - Brand  
  - Product Name  
  - Original Price  
  - Discounted Price  
  - Product Image URL  
  - Rating  
  - Reviews  
  - Available Sizes (with stock status)

---
```python
## Keywords Used
KEYWORDS = ["white shirt", "black dress", "denim jeans", "summer kurti", "co-ord set", "oversized t-shirt", "sneakers", "blue linen pants", "pink blazer for women", "yellow maxi dress"]
