```python
# Python blog post web scraper for my website
# By: Aidan Murray
# Date: 25/03/24

import requests  
from bs4 import BeautifulSoup  
  
URL = "https://thattakashi.com/blog/"  
page = requests.get(URL)
  
soup = BeautifulSoup(page.content, "html.parser")  
results = soup.find(class_="wp-block-query-is-layout-flow")  
  
job_elements = results.find_all("li", class_="wp-block-post")  
  
print(f"Blog Posts from {URL}")  
print("------------")  
  
for job_element in job_elements:  
    title_element = job_element.find("h3", class_="wp-block-post-title")  
    date_element = job_element.find("div", class_="wp-block-post-date")  
    description_element = job_element.find("p", class_="wp-block-post-excerpt__excerpt")  
  
    print(f"Post title: {title_element.text.strip()}")  
    print(f"Date posted: {date_element.text.strip()}")  
    print(f"Post description: {description_element.text.strip()}")  
    print("*------------*")  
```
