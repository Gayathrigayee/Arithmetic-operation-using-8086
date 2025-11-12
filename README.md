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
![WhatsApp Image 2025-11-12 at 22 27 05_d5f0b15f](https://github.com/user-attachments/assets/8cb1a03e-3132-45ca-ab84-eaf17e536af1)
alculation here)

---

## OUTPUT IMAGE FROM MASM SOFTWARE
![WhatsApp Image 2025-11-12 at 22 28 12_93660ddf](https://github.com/user-attachments/assets/5ca1691a-8583-44d0-bb6a-69d166467923)

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
```asm
code segment

C:NUIMALSUB.ASM

assume cs:code,ds:code

org 1000h

mov si, 1200h

mov ax, [si]

mov bx, [si+62h]

mou c1,00h

sub ax, bx jnc 11

inc cl

11:mov[si+04h],ax

mov [si+06h].cl

mov ah, 4ch

int 21h

code ends

end
```
#### Output Table

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|                         |                          |

#### Manual Calculations

(Add your calc![WhatsApp Image 2025-11-12 at 22 27 06_65dcc02c](https://github.com/user-attachments/assets/ce463437-f3ce-4a81-8e0b-e7d7c712bd5c)
ulation here)

---


## OUTPUT SCREEN FROM MASM SOFTWARE
![WhatsApp Image 2025-11-12 at 22 28 11_7dc9153e](https://github.com/user-attachments/assets/e5db3040-32ea-444c-a7c9-5f8e01b2d87e)

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
![WhatsApp Image 2025-11-12 at 22 49 07_ea703293](https://github.com/user-attachments/assets/13f55a6e-2a90-4156-b611-6dd2aa536f71)

## OUTPUT SCREEN FROM MASM SOFTWARE
![WhatsApp Image 2025-11-12 at 22 49 26_8eea7a14](https://github.com/user-attachments/assets/8873aea6-8560-480b-b09c-bba6f12ea7b6)

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

![WhatsApp Image 2025-11-12 at 22 54 03_067bc29a](https://github.com/user-attachments/assets/84be193a-1172-4e3b-b0eb-e23abc4885ba)

---
## OUTPUT FROM MASM SOFTWARE

![WhatsApp Image 2025-11-12 at 22 54 23_07a6f7f6](https://github.com/user-attachments/assets/d679bb06-571e-44ef-8139-5f80483a749b)


## RESULT

Thus, the Assembly Language Programs for 8086 to perform arithmetic operations (Addition, Subtraction, Multiplication, and Division) using both direct and indirect methods were successfully written and executed using MASM.
