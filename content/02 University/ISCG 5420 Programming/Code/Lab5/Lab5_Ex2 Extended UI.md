```python
# Python web scraper for blog posts  
# By: Takashi  
# Date: 28th March 2024  
  
# Import requests to fetch HTML data from a given website  
import tkinter as tk  
import customtkinter  
import requests  
from bs4 import BeautifulSoup  
import json  
  
click = 0  
  
  
def scrape(url, titleelements, titleclass, dateelements, dateclass, descelements, descclass):  
    click = 1  
    if click != 0:  
        page = requests.get("https://thattakashi.com/blog")  
        file_name = "test.txt"  
  
        data_n = {}  
  
        soup = BeautifulSoup(page.content, "html.parser")  
        results = soup.find(class_="wp-block-query-is-layout-flow")  
  
        job_elements = results.find_all("li", class_="wp-block-post")  
  
        for job_element in job_elements:  
            post = "Post"  
            title_element = job_element.find(titleelements.get(), class_=titleclass.get())  
            date_element = job_element.find(dateelements.get(), class_=dateclass.get())  
            description_element = job_element.find(descelements.get(), class_=descclass.get())  
  
            temp = {}  
            f = "Title"  
            print(title_elements)  
            temp[f] = title_element.text.strip()  
            print(f"Post title: {title_element.text.strip()}")  
            g = "Date Posted"  
            temp[g] = date_element.text.strip()  
            print(f"Date posted: {date_element.text.strip()}")  
            h = "Description"  
            temp[h] = description_element.text.strip()  
            print(f"Post description: {description_element.text.strip()}")  
            print("*------------*")  
            data_n[post] = temp  
  
            file = open(file_name, 'a+')  
            data = data_n  
            json.dump(data, file, indent=4)  
  
  
root = customtkinter.CTk()  
root.title("Web Scraper")  
root.geometry("515x550")  
  
URL = tk.StringVar()  
title_elements = tk.StringVar()  
date_elements = tk.StringVar()  
desc_elements = tk.StringVar()  
  
title_class = tk.StringVar()  
date_class = tk.StringVar()  
desc_class = tk.StringVar()  
  
app_title = customtkinter.CTkLabel(root, text="Python Web Scraper", font=("comfortaa", 25))  
app_title.grid(row=0, column=0, columnspan=3, padx=20, pady=40, sticky="ew")  
  
url_label = customtkinter.CTkLabel(root, text="Website", font=("comfortaa", 15))  
url_label.grid(row=1, column=0, padx=20, pady=20, sticky="w")  
  
label2 = customtkinter.CTkLabel(root, text="Url of website to scrape:")  
label2.grid(row=2, column=0, padx=20, pady=10, sticky="w")  
  
entry = customtkinter.CTkEntry(root, placeholder_text="Enter here", textvariable=URL)  
entry.grid(row=2, column=1, padx=20, pady=10, sticky="w")  
  
element_label = customtkinter.CTkLabel(root, text="Elements", font=("comfortaa", 15))  
element_label.grid(row=3, column=0, padx=20, pady=20, sticky="w")  
  
label3 = customtkinter.CTkLabel(root, text="Title element class and type:")  
label3.grid(row=4, column=0, padx=20, pady=10, sticky="w")  
  
entry2 = customtkinter.CTkEntry(root, placeholder_text="Type", width=60, textvariable=title_elements)  
entry2.grid(row=4, column=2, pady=10, sticky="w")  
  
entry3 = customtkinter.CTkEntry(root, placeholder_text="Class", textvariable=title_class)  
entry3.grid(row=4, column=1, padx=20, pady=10, sticky="w")  
  
label4 = customtkinter.CTkLabel(root, text="Date element class and type:")  
label4.grid(row=5, column=0, padx=20, pady=10, sticky="w")  
  
entry4 = customtkinter.CTkEntry(root, placeholder_text="Type", width=60, textvariable=date_elements)  
entry4.grid(row=5, column=2, pady=10, sticky="w")  
  
entry5 = customtkinter.CTkEntry(root, placeholder_text="Class", textvariable=date_class)  
entry5.grid(row=5, column=1, padx=20, pady=10, sticky="w")  
  
label5 = customtkinter.CTkLabel(root, text="Description element class and type:")  
label5.grid(row=6, column=0, padx=20, pady=10, sticky="w")  
  
entry6 = customtkinter.CTkEntry(root, placeholder_text="Type", width=60, textvariable=desc_elements)  
entry6.grid(row=6, column=2, pady=10, sticky="w")  
  
entry7 = customtkinter.CTkEntry(root, placeholder_text="Class", textvariable=desc_class)  
entry7.grid(row=6, column=1, padx=20, pady=10, sticky="w")  
  
button = customtkinter.CTkButton(root, text="Scrape!", command=lambda:[scrape(URL, title_elements, title_class, date_elements, date_class, desc_elements, desc_class)])  
button.grid(row=7, column=0, columnspan=3, padx=20, pady=20)  
  
root.mainloop()
```
