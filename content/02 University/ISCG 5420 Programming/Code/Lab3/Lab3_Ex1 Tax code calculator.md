```python
# New Zealand Tax Code Calculater  
# By Aidan Murray  
# 11/03/2024  
# Ver 0.1  
  
# Ask for the users name  
name = input("Please enter your name: ")  
  
# Tell the user the expected input  
print("Please answer the following questions with 'yes' or 'no'")  
  
# Define questions for Other Tax Codes  
print("Do you fall into any of the following categories? ")  
OTQ1 = "Casual agricultural worker, shearer or shedhand"  
OTQ2 = "Election day worker"  
OTQ3 = "Recognised seasonal worker"  
OTQ4 = "Special tax code"  
  
# Define questions for Tax Codes  
Q1 = "Q1: DO you receive an income tested benefit? "  
Q2 = "Q2: Is this tax code for the income tested benefit? "  
Q3 = "Q3: Is this tax code for your main or highest source of income? "  
Q4 = "Q4: Is your annual income from all sources likely to be $14000 or less? "  
Q5 = "Q5: Is your annual income from all sources likely to be between 14001 and 48000? "  
Q6 = "Q6: Is your annual income from all sources likely to be between 48001 and 70000? "  
Q7 = "Q7: Are you a NZ tax resident? "  
Q8 = "Q8: Is your annual income between $24K and $48K? "  
Q9 = "Q9: Are you or your partner entitled to Working for Families Tax Credits? "  
Q10 = "Q10: Do you have a NZ student loan? "  
  
# Define common program messages  
M1 = "This program cannot determine your tax code. Please use the program for secondary income "  
M2 = "Do you have a student lone? "  
  
# Define TaxCode variable  
TaxCode = ""  
  
# Test all questions against the users input to each  
OTA1 = input(OTQ1)  
if OTA1 == "yes":  
    TaxCode = "CAE"  
    quit()  
else:  
    TaxCode = ""  
  
OTA2 = input(OTQ2)  
if OTA2 == "yes":  
    TaxCode = "EDW"  
    quit()  
else:  
    TaxCode = ""  
  
OTA3 = input(OTQ3)  
if OTA3 == "yes":  
    TaxCode = "NSW"  
    quit()  
else:  
    TaxCode = ""  
  
OTA4 = input(OTQ4)  
if OTA4 == "yes":  
    TaxCode = "STC"  
    quit()  
else:  
    TaxCode = ""  
  
A1 = input(Q1)  
if A1 == "yes":  
    A2 = input(Q2)  
    if A2 == "yes":  
        TaxCode = "M"  
    else:  
        A4 = input(Q4)  
        if A4 == "yes":  
            SL = input(M2)  
            if SL == "yes":  
                TaxCode = "SB SL"  
            else:  
                TaxCode = "SB"  
        else:  
            A5 = input(Q5)  
            if A5 == "yes":  
                SL = input(M2)  
                if SL == "yes":  
                    TaxCode = "S SL"  
                else:  
                    TaxCode = "S"  
            else:  
                A6 = input(Q6)  
                if A6 == "yes":  
                    SL = input(M2)  
                    if SL == "yes":  
                        TaxCode = "SH SL"  
                    else:  
                        TaxCode = "SH"  
                else:  
                    SL = input(M2)  
                    if SL == "yes":  
                        TaxCode = "ST SL"  
                    else:  
                        TaxCode = "ST"  
else:  
    A3 = input(Q3)  
    if A3 == "no":  
        A4 = input(Q4)  
        if A4 == "yes":  
            SL = input(M2)  
            if SL == "yes":  
                TaxCode = "SB SL"  
            else:  
                TaxCode = "SB"  
        else:  
            A5 = input(Q5)  
            if A5 == "yes":  
                SL = input(M2)  
                if SL == "yes":  
                    TaxCode = "S SL"  
                else:  
                    TaxCode = "S"  
            else:  
                A6 = input(Q6)  
                if A6 == "yes":  
                    SL = input(M2)  
                    if SL == "yes":  
                        TaxCode = "SH SL"  
                    else:  
                        TaxCode = "SH"  
                else:  
                    SL = input(M2)  
                    if SL == "yes":  
                        TaxCode = "ST SL"  
                    else:  
                        TaxCode = "ST"  
  
    else:  
        A7 = input(Q7)  
        if A7 == "yes":  
            A8 = input(Q8)  
            if A8 == "yes":  
                A9 = input(Q9)  
                if A9 == "no":  
                    A10 = input(Q10)  
                    if A10 == "yes":  
                        TaxCode = "ME SL"  
                    else:  
                        TaxCode = "ME"  
                else:  
                    A10 = input(Q10)  
                    if A10 == "yes":  
                        TaxCode = "M SL"  
                    else:  
                        TaxCode = "M"  
            else:  
                A10 = input(Q10)  
                if A10 == "yes":  
                    TaxCode = "M SL"  
                else:  
                    TaxCode = "M"  
        else:  
            A10 = input(Q10)  
            if A10 == "yes":  
                TaxCode = "M SL"  
            else:  
                TaxCode = "M"  
print(f"Thanks for answering the questions, {name}. Your tax code is {TaxCode}")
```