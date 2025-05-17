#  E-Com Data Finder

**E-Com Data Finder** is a powerful web tool designed to help users extract and filter e-commerce websites by location, industry, technology stack (Shopify), and performance (domain status and load time). It also enables CSV-based filtering and email extraction from websites.

---

##  Features

- **Location-based filtering**: Filter websites by country, state/city, and industry.
- **Performance filters**:
  - Active domain check
  - Page load speed under 5 seconds
- **Technology detection**: Identify Shopify stores.
- **CSV upload support**:
  - Exclude specific websites from search
  - Upload websites to extract emails
- **Email extraction**: Pull emails from fetched domains.
- **Download results** as a CSV.

---

##  Tech Stack

- **Backend**: [FastAPI](https://fastapi.tiangolo.com/)
- **Frontend**: HTML + TailwindCSS (lightweight and responsive)
- **Templating**: Jinja2
- **Web Scraping & Detection**: `SarpAPI` for Website Scraping, `beautifulsoup4` for Email Scraping

---

##  Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/IDKSAM27/INS-CSE-37-11299.git
cd INS-CSE-37-11299
```

##  Getting Started

### 2. Create and Activate a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
---


### 3. Install Requirements

```bash
pip install -r requirements.txt
```
---

### 4. Run the App

```bash
uvicorn main:app --reload
```

### Then open your browser and visit:
http://localhost:8000

---

##  Folder Structure

```graphql
E-Com Data Finder
├── app
│   ├── _pycache_/
│   ├── logic
│   │   ├── _pycache_/
│   │   ├── fetch_emails.py
│   │   ├── fetch_websites.py
│   │   ├── filters.py
│   │   ├── get_websites.py
│   │   └── utils.py
│   ├── static
│   │   └── styles.css
│   └── views
│       ├── static
│       │   └── script.js
│       └── templates
│           ├── fetch_emails.html
│           ├── index.html
│           └── results.html
├── main.py
├── emails.csv
├── readme.md
├── run.py

```