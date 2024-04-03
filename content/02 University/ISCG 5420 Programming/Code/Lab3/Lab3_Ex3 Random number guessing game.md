```python
# Python random number guessing game  
# By Aidan Murray  
# 11/03/2024  
# Ver 1.0  
  
# Import the random library  
import random  
  
# Generate a random number between 1 and 6 and store it in the variable "a"  
a = random.randint(1, 6)  
  
# Ask the user for their guess  
answer = int(input("Enter your guess between 1 and 6: "))  
  
# Check the users answer against the generated random number  
if answer == a:  
    # If the user guessed correctly, they win  
    print(f"Your answer was {answer}. You guessed correctly! The number was {a}")  
else:  
    # If the user does not guess correctly, they loose  
    print(f"Your answer of {answer} was wrong. The correct answer was {a}")
```
