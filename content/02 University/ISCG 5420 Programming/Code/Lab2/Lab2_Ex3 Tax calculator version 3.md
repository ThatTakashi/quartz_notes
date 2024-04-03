```python
print("How much is your salary? (Between 70k and 180k)")  
S = int(input(">>> "))  
  
TR1 = 14000*0.105  
TR2 = (48000-14000)*0.175  
TR3 = (70000-48000)*0.30  
TR4 = (S - 70000)*0.33  
  
tax = TR1 + TR2 + TR3 + TR4  
  
print("total = "+str(tax))  
  
income = S - tax  
  
Message1 = "You pay "+str(tax)+"$ tax."  
  
Message2 = "Your income after tax reduction is " +str(income)+ " $."  
  
print(Message1, "\n", Message2)
```