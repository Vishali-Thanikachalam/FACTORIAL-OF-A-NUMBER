# FACTORIAL-OF-A-NUMBER-USING-8051-KEIL

**AIM:**

To write and execute Assembly language Program to perform factorial of a number using 8051 keil.

**APPARATUS REQUIRED:**

Personal computer with Keil software

**Algorithm**

1. **Start**
2. **Input:** Read the number `n`.
3. **Initialize:**
   * Set `factorial = 1`
   * Set `i = 1`
4. **Loop:** While `i` ≤ `n`
   * Multiply `factorial` by `i`
   * Increment `i` by 1
5. **Output:** Store or print the value of `factorial`.
6. **End**

**FLOW CHART:**

<img width="261" height="308" alt="image" src="https://github.com/user-attachments/assets/bffe89f6-3ba9-4294-b817-8b545f680e66" />

**Program:**

```
ORG 0000H   
MOV A,#04H  
MOV R0,A  
ACALL FACTORIAL  
MOV 40H,A  
SJMP THIN  
FACTORIAL:DEC R0  
CJNE R0,#01H,PRODUCT  
SJMP THICK   
PRODUCT:MOV B,R0  
MUL AB  
ACALL FACTORIAL  
THICK: RET  
THIN:  
END
```

**Output:**  

<img width="500" height="420" alt="image" src="https://github.com/user-attachments/assets/db3c2d31-1a24-49cc-976f-abda28716c33" />


**Manual Calculations:**  

![WhatsApp Image 2025-10-23 at 20 31 50_578c4bbe](https://github.com/user-attachments/assets/da947181-05ca-4bd9-b926-c0510465429a)

**Result:**

Thus the factorial of a number using 8051 keil was calculated and shown the output.
