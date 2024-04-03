```python
print("How much is your salary?")  
S = int(input(">>> "))  
  
print("What is your tax rate in %?")  
TR = int(input(">>> "))  
  
tax = S * TR / 100  
  
income = S - tax  
  
Message1 = "You pay "+str(tax)+"$ tax."  
  
Message2 = "Your income after tax reduction is " +str(income)+ " $."  
  
print(Message1, "\n", Message2)
```