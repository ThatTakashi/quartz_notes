```python
A1 = "Test 1"  
A2 = "Test 2"  
A3 = "Project"  
A4 = "Exam"  
  
W1 = 15  
W2 = 20  
W3 = 25  
W4 = 40  
  
M1 = int(input("Enter your mark for "+A1+": "))  
  
while M1 < 0 or M1 > 15:  
    print("\nEnter a value between 0 and 15")  
    M1 = int(input("Enter your mark for "+A1+": "))  
  
M2 = int(input("Enter your mark for "+A2+": "))  
  
while M2 < 0 or M2 > 20:  
    print("\nEnter a value between 0 and 20")  
    M2 = int(input("Enter your mark for "+A1+": "))  
  
M3 = int(input("Enter your mark for "+A3+": "))  
  
while M3 < 0 or M3 > 25:  
    print("\nEnter a value between 0 and 25")  
    M3 = int(input("Enter your mark for "+A1+": "))  
  
M4 = int(input("Enter your mark for "+A4+": "))  
  
while M4 < 0 or M4 > 40:  
    print("\nEnter a value between 0 and 40")  
    M4 = int(input("Enter your mark for "+A1+": "))  
  
total = M1 + M2 + M3 + M4  
  
print("------------------------------------------")  
print(f"Your total grad this semester is {total}%")
```