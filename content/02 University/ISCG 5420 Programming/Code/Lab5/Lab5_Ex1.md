```python
# Building a time calculator
# By: Aidan Murray
# Date: 25/03/24

seconds = int(input("Enter the amount of seconds: "))  
  
seconds = seconds % (24 * 3600)  
hour = seconds // 3600  
seconds = seconds % 3600  
minutes = seconds // 60  
seconds = seconds % 60  
  
print(f"Seconds value in hours {hour}")  
print(f"Seconds value in minutes {minutes}")  
print("------------")  
print(f"Time in preferred format: {hour}:{minutes}:{seconds}")
```
