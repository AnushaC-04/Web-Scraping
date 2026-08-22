# 🕸️ Web Scraping with Python

A collection of **Web Scraping projects and practice notebooks** built using Python.
This repository covers the fundamentals of extracting data from websites, working with scraped data, saving results into structured formats, and automating browser-based scraping using Selenium.

---

## 📌 Overview

Web scraping is the process of extracting useful information from websites and converting unstructured web content into structured data.

This repository contains hands-on implementations of:

* 🌐 Web page scraping
* 📚 Book data extraction
* 🛒 E-commerce data scraping
* 🤖 Browser automation using Selenium
* 📊 Storing scraped data in Excel files
* 🖼️ Downloading and working with images
* 🧹 Basic data processing using Pandas

---

## 🛠️ Technologies Used

| Technology          | Purpose                                     |
| ------------------- | ------------------------------------------- |
| 🐍 Python           | Core programming language                   |
| 🐼 Pandas           | Data processing and storage                 |
| 🌐 Requests         | Sending HTTP requests                       |
| 🍲 BeautifulSoup    | Parsing HTML content                        |
| 🤖 Selenium         | Browser automation and dynamic web scraping |
| 📊 Excel            | Storing scraped datasets                    |
| 📓 Jupyter Notebook | Development and experimentation             |

---

## 📂 Repository Structure

```text
Web-Scraping/
│
├── images/
│   └── Scraped images and related resources
│
├── books.xlsx
├── books_1000.xlsx
├── Mobiles.xlsx
│
├── book_details.ipynb
├── day1ws.ipynb
├── day2ws.ipynb
├── day3ws.ipynb
├── flipkart_selenium.ipynb
│
├── .gitignore
└── README.md
```

---

## 📚 Projects & Notebooks

### 1. 📖 Book Details Scraping

**Notebook:** `book_details.ipynb`

This notebook focuses on extracting book-related information from a website and converting the scraped information into a structured dataset.

The scraped data can be stored and exported into Excel files for further analysis.

**Output files:**

* `books.xlsx`
* `books_1000.xlsx`

---

### 2. 🕸️ Web Scraping Practice

The following notebooks contain progressive web scraping exercises:

```text
day1ws.ipynb
day2ws.ipynb
day3ws.ipynb
```

These notebooks demonstrate the fundamentals of web scraping, including:

* Sending requests to web pages
* Understanding HTML structure
* Finding required HTML elements
* Extracting text and attributes
* Collecting multiple records
* Converting scraped information into structured data
* Saving extracted data

---

### 3. 🛒 Flipkart Scraping with Selenium

**Notebook:** `flipkart_selenium.ipynb`

This project demonstrates web scraping using **Selenium**, which allows Python to control a web browser.

Selenium is particularly useful when websites rely heavily on JavaScript and dynamically load their content.

The project focuses on extracting product information from an e-commerce website.

**Output:**

```text
Mobiles.xlsx
```

The scraped product information is stored in Excel for further processing and analysis.

---

## 🔄 General Web Scraping Workflow

```text
             Website
                │
                ▼
       Send HTTP Request
                │
                ▼
          Receive HTML
                │
                ▼
        Parse HTML Content
                │
                ▼
       Find Required Elements
                │
                ▼
        Extract Information
                │
                ▼
       Convert to DataFrame
                │
                ▼
          Export to Excel
```

For dynamic websites:

```text
Website
   │
   ▼
Selenium WebDriver
   │
   ▼
Open Browser
   │
   ▼
Load Dynamic Content
   │
   ▼
Locate Web Elements
   │
   ▼
Extract Data
   │
   ▼
Pandas DataFrame
   │
   ▼
Excel / CSV
```

---

## 🧰 Common Libraries

### Requests

Used to send HTTP requests and retrieve webpage content.

```python
import requests

url = "https://example.com"

response = requests.get(url)

print(response.status_code)
print(response.text)
```

### BeautifulSoup

Used to parse HTML and locate required elements.

```python
from bs4 import BeautifulSoup

soup = BeautifulSoup(response.text, "html.parser")

data = soup.find_all("div")
```

### Pandas

Used to organize scraped information into structured datasets.

```python
import pandas as pd

df = pd.DataFrame(data)

df.to_excel("output.xlsx", index=False)
```

### Selenium

Used for browser automation and scraping dynamically generated webpages.

```python
from selenium import webdriver

driver = webdriver.Chrome()

driver.get("https://example.com")
```

---

## 📊 Data Storage

The scraped data in this repository is stored primarily in **Excel format**.

Examples:

```text
books.xlsx
books_1000.xlsx
Mobiles.xlsx
```

This makes the scraped data easy to:

* Inspect
* Clean
* Analyze
* Visualize
* Use in Machine Learning projects

---

## 🎯 Learning Objectives

Through this repository, I practiced:

* Understanding webpage structure
* Inspecting HTML elements
* Extracting information from websites
* Using CSS selectors / HTML tags
* Handling multiple pages
* Collecting structured datasets
* Automating browsers with Selenium
* Saving scraped data into Excel
* Working with Pandas DataFrames
* Understanding the difference between static and dynamic websites

---

## ⚠️ Web Scraping Considerations

When scraping websites, it is important to:

* Respect the website's `robots.txt` and terms of service.
* Avoid sending excessive requests.
* Add appropriate delays when necessary.
* Avoid collecting private or sensitive information.
* Use scraped data responsibly.
* Prefer official APIs when they are available.

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Navigate to the project

```bash
cd Web-Scraping
```

### 3. Install the required libraries

```bash
pip install requests beautifulsoup4 pandas openpyxl selenium jupyter
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open any notebook

For example:

```text
book_details.ipynb
```

or

```text
flipkart_selenium.ipynb
```

Run the cells sequentially.

---

## 📈 Future Improvements

Some possible extensions for this repository:

* [ ] Add more e-commerce scraping projects
* [ ] Scrape multiple pages automatically
* [ ] Add pagination handling
* [ ] Implement error handling
* [ ] Add request delays and retry mechanisms
* [ ] Store data in CSV and JSON formats
* [ ] Connect scraped datasets to Power BI
* [ ] Perform EDA on scraped datasets
* [ ] Build ML projects using scraped data
* [ ] Create automated scraping pipelines

---

## 👩‍💻 Author

**Anusha C**

This repository is part of my journey in learning **Python, Data Analytics, Machine Learning, and Generative AI**, with a focus on building practical projects through hands-on implementation.

---

⭐ If you find this repository useful, consider giving it a star!
