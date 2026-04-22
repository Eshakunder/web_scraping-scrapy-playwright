# Playwright-Powered Product Scraper

A s Scrapy spider designed to scrape dynamic, JavaScript-rendered e-commerce sites. 
This project demonstrates how to use **Playwright** integration to wait for specific DOM elements before extracting data.

##  Tools & Technologies
* **Python 3.10+**
* **Scrapy**: The core scraping framework.
* **Scrapy-Playwright**: For headless browser automation and JS rendering.
* **Asyncio**: To handle asynchronous parsing logic.

##  Key Features
* **Dynamic Waiting**: Uses `PageCoroutine` to wait for `div#productListing`, ensuring the page is fully loaded before scraping.
* **Headless Browsing**: Bypasses issues with empty HTML responses from Single Page Applications (SPAs).
* **Asynchronous Processing**: Uses `async def parse` for efficient data handling.

##  Extracted Data
The spider extracts the following fields from the target landing page:
* **Title**: The name/headline of the product.
* **Price**: The cost associated with the item.

