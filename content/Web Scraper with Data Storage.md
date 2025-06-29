---
title: Web Scraper With Data Storage
date: 2025-06-30
author: Your Name
cell_count: 5
score: 5
---

```python
import requests
from bs4 import BeautifulSoup
import sqlite3
```


```python
def scrape_quotes():
    url = "http://quotes.toscrape.com"
    response = requests.get(url)
    soup = BeautifulSoup(response.text, "html.parser")
    quotes = soup.find_all("span", class_="text")
    
    conn = sqlite3.connect("quotes.db")
    c = conn.cursor()
    c.execute("CREATE TABLE IF NOT EXISTS quotes (text TEXT, author TEXT)")
    
    for quote in quotes:
        text = quote.get_text()
        author = quote.find_next("small").get_text()
        c.execute("INSERT INTO quotes VALUES (?, ?)", (text, author))
    
    conn.commit()
    conn.close()
```


```python
scrape_quotes()
```


```python

```


```python

```


---
**Score: 5**