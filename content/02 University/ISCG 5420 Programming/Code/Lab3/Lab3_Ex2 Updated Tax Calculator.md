```python
name = input("Whats your name?: ")  
  
print("How much is your salary? (Between 70k and 180k)")  
S = int(input(">>> "))  
  
TR1 = 0  
TR2 = 0  
TR3 = 0  
TR4 = 0  
TR5 = 0  
  
if S <= 14000:  
    TR1 = 14000 * 0.105  
else:  
    if S > 14000 or S <= 48000:  
        TR2 = (48000 - 14000) * 0.175  
    else:  
        if S > 48000 or S <= 70000:  
            TR3 = (70000 - 48000) * 0.30  
        else:  
            if S > 70000 or S <= 180000:  
                TR4 = (S - 70000) * 0.33  
            else:  
                TR5 = (S - 180000) * 0.39  
  
tax = TR1 + TR2 + TR3 + TR4 + TR5  
  
print("total = " + str(tax))  
  
income = S - tax  
  
Message1 = "You pay " + str(tax) + "$ tax."  
  
Message2 = "Your income after tax reduction is " + str(income) + " $."  
  
print(Message1, "\n", Message2)
```