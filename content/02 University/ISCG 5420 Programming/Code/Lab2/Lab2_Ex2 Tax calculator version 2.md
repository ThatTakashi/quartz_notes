```python
print("How much is your salary? (Between 48k and 70k)")  
S = int(input(">>> "))  
  
tax = (14000 * 10.5 / 100) + (34000 * 17.5 / 100) + ((S - 48000) * 30 / 100)  
  
print("total = "+str(tax))  
  
income = S - tax  
  
Message1 = "You pay "+str(tax)+"$ tax."  
  
Message2 = "Your income after tax reduction is " +str(income)+ " $."  
  
print(Message1, "\n", Message2)
```