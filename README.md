# KeywordCrawler

A code that would get us all the visited and not visited urls of a particular domain and the keyword we pass will help us in finding correct and related domains which will act as potential targets for us!

**KeywordCrawler** is a lightweight Python-based recursive crawler built for **penetration testers**, **recon enthusiasts**, and **bug bounty hunters**. It crawls web pages from a target URL and collects all URLs that match a specified keyword—ideal for finding endpoints, subpaths, or areas of interest within a scope.
---

## 🚀 Features
- 🔗 Recursively crawls through internal & external links
- 🔍 Filters URLs containing specific keywords (e.g., `admin`, `login`, `api`)
- 🔐 Helps identify juicy endpoints for bug bounty recon
- 🛑 Avoids duplicate visits with URL tracking
- 🧰 Built using `requests` + `BeautifulSoup`

---

## 🎯 Use Cases
- Find hidden or keyword-targeted pages (like `/admin`, `/dev`, `/upload`)
- Build custom recon scripts for domain scope crawling
- Discover hidden areas that may contain security misconfigurations
- Early-stage target mapping for bug bounty & pentesting

---

## 🛠️ Requirements

- Python 3.x  
- `requests`  
- `beautifulsoup4`  

Install with:
```bash
pip install -r requirements.txt
