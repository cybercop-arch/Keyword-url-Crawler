# 🔍 Keyword URL Crawler

**Keyword URL Crawler** is a two-part Python tool designed to help you **scrape and filter URLs based on a specific keyword** and **validate those URLs** to ensure they are accessible (status code 200). Perfect for web scraping, SEO analysis, or digital research.

---

## 🧠 Features

- ✅ Recursive crawling of any website
- 🔎 Extracts and filters URLs containing a specific keyword
- 🌐 Resolves relative URLs to full URLs
- 🚫 Skips duplicate URLs with visited URL tracking
- ⚙️ Validates URLs to check if they're alive (status 200)
- 📁 Saves working URLs to a text file

---

## 📂 Project Structure

keyword-url-crawler/
│
├── keyword_crawler.py # Crawls and extracts keyword-matching URLs
├── url_validator.py # Validates URLs and saves working ones
├── filtered_urls.txt # Output file for valid URLs
└── README.md # Project documentation

---

## 💡 How It Works

### 1. **Crawl URLs (keyword-based)**  
Use `keyword_crawler.py` to recursively find all `<a>` tag links starting from a base URL. It will print only those URLs that contain the keyword you specify.

### 2. **Validate URLs**  
Use `url_validator.py` to check which of the collected URLs return a status code of 200 (working links). These are saved to `filtered_urls.txt`.

---

## 🚀 Getting Started

### 📋 Requirements

- Python 3.x
- Install dependencies:
  ```bash
  pip install requests beautifulsoup4

## Usage

### ✅ Step 1: Run the Keyword Crawler

 -python keyword_crawler.py

--You will be prompted to enter the base URL and keyword:

-enter a url you would like to scrape: https://example.com
-enter the keyword you want in url: blog

-It will output all URLs containing the keyword blog.

-To save the results to a file:
--python keyword_crawler.py > raw_urls.txt

### 🔎 Step 2: Validate the URLs
-Pass the saved URLs to the validator using:
--cat raw_urls.txt | python url_validator.py
-Valid URLs will be saved to:
--filtered_urls.txt

🧪 Example Workflow
--python keyword_crawler.py > raw_urls.txt
--cat raw_urls.txt | python url_validator.py

📌 Notes
◇ This crawler is not JavaScript-aware. It only extracts static HTML links.

◇ Avoid crawling large or protected websites excessively to prevent being blocked.

◇ For ethical use only: Do not crawl private or rate-limited websites without permission.
---

🔐 Disclaimer
This tool is intended for educational and ethical use only. Ensure you have permission before crawling any external site.

🙋‍♀️ Author
Samiksha
 Cybersecurity & Forensics Student | Developer | Ethical Hacking Enthusiast

🤝 Contributing
Pull requests, ideas, and suggestions are welcome!

---
