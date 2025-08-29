# Arithmetic-operation-using-8086
# 8086 Assembly Language Programs for Arithmetic Operations

## AIM

To write and execute Assembly Language Programs to perform arithmetic operations for the 8086 microprocessor.

---

## APPARATUS REQUIRED

* Personal Computer with MASM Software

---

## 1. ADDITION

#### Algorithm

1. Initialize memory location in HL register.
2. Store 1st data.
3. Increment HL to enter 2nd data.
4. Move 2nd number to accumulator.
5. Decrement HL.
6. Add value in memory with accumulator.
7. Store result.
8. Stop.


## FLOW CHART
<img width="707" height="1024" alt="image" src="https://github.com/user-attachments/assets/b5a7062d-e294-47cd-9683-a40de25e82de" />


#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV CL,00H
MOV AX,[SI]
MOV BX,[SI+02H]
ADD AX,BX
JNC L1
INC CL
L1:
MOV [SI+04H],AX
MOV [SI+06H],CL
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|                         |                          |

#### Manual Calculations

![add manual calculation](https://github.com/user-attachments/assets/310f99c0-5960-41a9-83fd-5a23df42d580)


---

## OUTPUT IMAGE FROM MASM SOFTWARE
<img width="732" height="469" alt="Screenshot 2025-08-27 125235" src="https://github.com/user-attachments/assets/bc5f5530-af1e-4b8c-9f39-4b77a7243960" />
<img width="665" height="442" alt="Screenshot 2025-08-27 130853" src="https://github.com/user-attachments/assets/9cb4ed03-1e20-4242-b292-7dd7a6679c6c" />






## 2. SUBTRACTION

#### Algorithm

1. Initialize memory and store 1st data.
2. Increment to get 2nd data.
3. Move 2nd data to accumulator.
4. Subtract memory content.
5. Store result.

## FLOWCHART

<img width="578" height="797" alt="image" src="https://github.com/user-attachments/assets/564c3c7a-33ce-4a1c-8920-beb5c24b9b47" />


#### Program



#### Output Table

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|                         |                          |

#### Manual Calculations

![submanualcalculation](https://github.com/user-attachments/assets/4c73f6a9-3e01-4176-8e9c-1407f976aee9)


---


## OUTPUT SCREEN FROM MASM SOFTWARE

<img width="637" height="430" alt="Screenshot 2025-08-29 103922" src="https://github.com/user-attachments/assets/185b6776-e7ef-4f6e-8dd9-148240e5b1dd" />
<img width="658" height="459" alt="Screenshot 2025-08-29 103307" src="https://github.com/user-attachments/assets/9436c060-0fb0-4cfc-a25d-52ea9bce02b8" />



## 3. MULTIPLICATION

#### Algorithm

1. Initialize memory and store operands.
2. Move operands to registers.
3. Multiply.
4. Store result.

##FLOWCHART

<img width="569" height="906" alt="image" src="https://github.com/user-attachments/assets/88be88ff-2896-4a88-b73d-84ccffd2fcf9" />



#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV DX,0000H
MOV AX,[SI]
MOV BX,[SI+02H]
MUL BX
MOV [SI+04H],AX
MOV [SI+06H],DX
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|                         |                          |

#### Manual Calculations

![multiplicationmanualcalculation](https://github.com/user-attachments/assets/70ddff3b-a312-4bde-8958-08b3fbe5ad8e)


---

## OUTPUT SCREEN FROM MASM SOFTWARE

<img width="627" height="422" alt="Screenshot 2025-08-28 083520" src="https://github.com/user-attachments/assets/4c5f04b6-2286-4428-8eb1-a15bcf4c72a3" />
<img width="622" height="422" alt="Screenshot 2025-08-28 083212" src="https://github.com/user-attachments/assets/498e5260-310f-4063-96c5-61ab34104127" />



## 4. DIVISION

#### Algorithm

1. Load memory location of operands.
2. Perform division.
3. Store result.

   ## FLOWCHART
<img width="1065" height="802" alt="image" src="https://github.com/user-attachments/assets/25b4a483-0d42-494b-8639-1af3ea17191b" />


#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV DX,0000H
MOV AX,[SI]
MOV BX,[SI+02H]
DIV BX
MOV [SI+04H],AX
MOV [SI+06H],DX
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|                         |                          |

#### Manual Calculations

![divisionmanualcalculation](https://github.com/user-attachments/assets/e016a2bf-fd7f-4115-9b71-fdd23ebc3dbe)


---
## OUTPUT FROM MASM SOFTWARE

<img width="637" height="426" alt="Screenshot 2025-08-28 085220" src="https://github.com/user-attachments/assets/44fe55d6-a96e-4d2e-88d5-f942d11d4235" />


<img width="628" height="428" alt="Screenshot 2025-08-28 085052" src="https://github.com/user-attachments/assets/3ed28917-8274-4f6b-b0dc-bed5f779f3ca" />




## RESULT

Thus, the Assembly Language Programs for 8086 to perform arithmetic operations (Addition, Subtraction, Multiplication, and Division) using both direct and indirect methods were successfully written and executed using MASM.
