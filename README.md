# Digital Electronics Internship

# Task 1

# Table of contents

- [What is Digital Electronics](#what-is-digital-electronics)
- [Applications of Digital Electronics](#applications-of-digital-electronics)
- [Digital vs Analog Signals](#digital-vs-analog-signals)
- [Number Systems](#number-systems)
- [Conversion between Number Systems](#conversion-between-number-systems)
- [Basic Logic Gates](#basic-logic-gates)
 
# What is Digital Electronics

Digital electronics is a branch of electronics that deals with systems and devices that use digital signals, which are discrete representations of data, 
typically using binary code (0s and 1s).


# Applications of Digital Electronics

1.Computing

2.Communication

3.Control Systems

4.Home Appliances

5.Medical Devices

6.Automotive

7.Security Systems

8.Industrial automation


# Digital vs Analog signals

| **Analog** | **Digital** |
|------------|-------------|
|Analog Signals are contionous signals| Digital Signals are not continous ,they are discrete signals|
|We can represent analog signals in the form of sign waves| We can represent digital signals in the form of square waves|
|The values of voltage will be in a continous range| the values of voltage will be discontinous|
|Records the information as it is | Converts the information into binary form|
|Major circuit components: Resistors,Inductors,Capacitors|Major Circuit Components:Diodes,Transistors|
|There are two types of analog circuits-Active circuit and Passive Circuit|There is only one type of digital circuit-Active Circuit|
|Analog Circuits consume more electrical power|Digital circuits consume less electrical power|
|Analog circuits have more noise | Digital circuits have less noise|
|Analog circuits are not so much accurate and precise | Digital circuits are very much accurate and precise|

# Logic Levels

In digital electronics, logic levels refer to the specific voltage ranges used to represent the two binary states: 

0 (low) and 1 (high).

**Common Logic Families and Their Voltage Levels:**

| **Logic Family** |	**Logic Low (0)** |	**Logic High (1)** |
|------------------|--------------------|---------------------|
|TTL (5V) |	0V to 0.8V |	2V to 5V|
|CMOS (5V)|	0V to 1.5V|	3.5V to 5V|
|CMOS (3.3V) |	0V to 1V |	2.3V to 3.3V|

# Number Systems

In digital electronics, number systems are used to represent information. These systems vary in base, with the most common being decimal, binary, octal, and hexadecimal. The base or radix of a number system indicates the total number of unique digits used. For example, a number system that uses digits from 0 to 9 has a base of 10.

Types of Number System

There are four primary types of number systems used in digital electronics:

1.Decimal Number System (Base 10)

2.Binary Number System (Base 2)

3.Octal Number System (Base 8)

4.Hexadecimal Number System (Base 16)

# Binary (Base 2), Decimal (Base 10), Hexadecimal (Base 16).
|**Binary (Base-2)** | **Decimal (Base-10)** | **Hexadecimal (Base-16)** |
|--------------------|-----------------------|---------------------------|
|Digits: 0, 1|Digits: 0 to 9|Digits: 0 to 9, A to F (where A=10, B=11, ..., F=15)|
|Most fundamental system in digital electronics.|Commonly used by humans.|Convenient for representing large binary numbers (4 bits per  digit).|
|Each binary digit (bit) represents an on/off state.|Converted to and from binary for computation.|Common in memory addresses and debugging.|

# Conversion between number systems 

**1. Binary to Decimal Conversion**

To convert a binary number to a decimal number:
Multiply each bit by  $2^n$  where n is the position of the bit (starting from 0 on the right) and then sum all the results.

Binary:   1    0    1    1    0    1

Position: 5    4    3    2    1    0

Value:    1×2⁵ + 0×2⁴ + 1×2³ + 1×2² + 0×2¹ + 1×2⁰

         = 32 + 0 + 8 + 4 + 0 + 1 = 4


**2. Decimal to Binary Conversion**

To convert a decimal number (base-10) to its binary equivalent (base-2), the division-by-2 method. is used

| Step | Division | Quotient | Remainder |
| ---- | -------- | -------- | --------- |
| 1    | 45 ÷ 2   | 22       | 1         |
| 2    | 22 ÷ 2   | 11       | 0         |
| 3    | 11 ÷ 2   | 5        | 1         |
| 4    | 5 ÷ 2    | 2        | 1         |
| 5    | 2 ÷ 2    | 1        | 0         |
| 6    | 1 ÷ 2    | 0        | 1         |

**3. Decimal to Octal Conversion**

Binary to Decimal: Convert the binary number to decimal by multiplying each bit by 2 raised to its position index (starting from 0 on the right) and summing the results.

Decimal to Octal: Divide the decimal number by 8 repeatedly, noting the remainders. The octal number is formed by reading the remainders in reverse order.

Example: Convert (101101)₂ to octal

**Binary to Decimal:**

(101101)₂ = 1×2⁵ + 0×2⁴ + 1×2³ + 1×2² + 0×2¹ + 1×2⁰

= 32 + 0 + 8 + 4 + 0 + 1 = 45

**Decimal to Octal:**

45 ÷ 8 = 5 remainder 5

+1

+1

5 ÷ 8 = 0 remainder 5

Octal: Reading remainders in reverse: 5 5 → (55)₈

**4. Octal to Binary Conversions**

Each octal digit corresponds to exactly 3 binary digits (bits).

Convert 157 (octal) to binary:

1 → 001

5 → 101

7 → 111

So, 157₈ = 001101111₂ 


**5. Binary to Hexadecimal Conversion**

Group binary digits into 4-bit chunks starting from the right, then convert each group to its hexadecimal equivalent.

Convert 10110111 (binary) to hexa

Group into 4-bits: 1011 0111

→ 1011 = B

→ 0111 = 7

So, 10110111₂ = B7₁₆

**6. Hexadecimal to Binary Coversion**

Convert 2F (hex) to binary

- 2 → 0010

- F → 1111

So, 2F₁₆ = 00101111₂

**7. Decimal to Octal Conversion**

Example: Decimal to Octal

125 ÷ 8 = 15, remainder 5 

15 ÷ 8  = 1, remainder 7 

1 ÷ 8   = 0, remainder 1

So, 125₁₀ = 175₈


**8. Octal to Decimal Coversion**

To convert octal to decimal, positional notation is used — each digit is multiplied by 8 raised to the power of its position (from right to left, starting at 0).

Example 1: Convert 175&#8328; to decimal

- 1.8&#178;=6
- 7.8^1=56
- 5.8^0=5

64+56+5=125

So, 
175&#178;=125&#10;

**9.Decimal to Hexadecimal Conversion**

Example:

254 ÷ 16 = 15, remainder 14 → E  

15 ÷ 16  = 0, remainder 15 → F

254₁₀ = FE₁₆

**10. Hexadecimal to Decimal Conversion**

Example: Convert 2F to decimal

- F = 15, in the 16^0 place →15×1=15

- 2 = 2, in the 16^1 place → 2×16=32

Add: 32+15=47

2F₁₆ = 47₁₀

**11. Octal to Heexideacimal Conversion**

Example: Convert 175₈ to hexadecimal

**Octal to Binary**

1 → 001

7 → 111

5 → 101

So, 175₈ = 001 111 101₂ → Combine → 001111101

Pad to make full 4-bit groups: 0001 1111 01 → pad left: 0001 1111 0101

Final binary: 0001 1111 0101

 **Binary to Hexa**

0001 → 1

1111 → F

0101 → 5

So, 175₈ = 1F5₁₆

Method:

Octal → Binary (3 bits), then Binary → Hex (4 bits).

Example: 65 (Octal) → 110101 (Binary) → 0001 1010 1 = 1A1 (Hex, pad as needed)

**12. Hexadecimal to Octal Conversion**

Example: Convert `2F₁₆` to octal

**Hexa to Binary**

* 2 → 0010
* F → 1111

Binary: `0010 1111`

**Binary to Octal**

Group into 3 bits (from right):
`00 101 111` → pad left with zeros → `000 010 111 1`

Better: pad full groups of 3 bits:
`000 010 111 111`

Actually, the binary `00101111` padded to 9 bits is `000 010 111 111`

Groups:

* 000 → 0
* 010 → 2
* 111 → 7
* 111 → 7

Octal: **0277**

---

Answer: 2F_{16} = 277_8



# Task 2

# Basic Logic Gates

# 1.AND Gate

An AND gate is a basic digital logic gate that outputs 1 (true) only when all its inputs are 1. Otherwise, it outputs 0 (false).

Represented as: A AND B = A ⋅ B or A ∧ B

**Truth Table**

|*A*|*B*| *A & B*|
|-----|----|------|
|0|0|0|
|0|1|0|
|1|0|0|
|1|1|1|

**Key Point:**

Output is true (1) only when both inputs are true (1).

**Symbol:**

![image](https://github.com/user-attachments/assets/06b17f4e-446d-4716-8b54-1b54191bb661)

# 2.OR Gate

An OR gate is a basic digital logic gate that implements logical disjunction. It gives a high (1) output if at least one of its inputs is high. In other words, the output is true when any input is true.

**Truth Table:**
|**A**|	**B**|	**Y (A OR B)**|
|-----|-------|---------------|
|0	|0	|0|
|0	|1	|1|
|1	|0	|1|
|1|	1|	1|

**Key Points**:

If both inputs are 0, the output is 0.

If at least one input is 1, the output is 1.

**Symbol**

![image](https://github.com/user-attachments/assets/9a5865c7-a982-4b78-a88f-4b383f66c838)

# 3.NOT Gate

A NOT gate, also known as an inverter, is a basic digital logic gate that outputs the opposite (inverse) of its input. It has only one input and one output.

**Function:**

If the input is 1 (true or HIGH), the output is 0 (false or LOW).

If the input is 0, the output is 1

The NOT gate is usually represented by a triangle pointing to the right with a small circle (called a "bubble") at the output.

**Truth Table:**
|**Input (A)** |	**Output (¬A)**|
|--------------|------------------|
|0	|1|
|1	|0|

This table shows that the NOT gate simply flips the input value.

**Symbol:**

![image](https://github.com/user-attachments/assets/b7ef0b26-2648-4ccd-8ba9-3d6c8bcec104)


# 4.NAND GATE

A NAND gate is a fundamental digital logic gate that outputs false (0) only when all its inputs are true (1); otherwise, it outputs true (1).

Definition:


### Truth Table (2-input NAND gate):

| Input A | Input B | Output (A NAND B) |
| ------- | ------- | ----------------- |
| 0       | 0       | 1                 |
| 0       | 1       | 1                 |
| 1       | 0       | 1                 |
| 1       | 1       | 0                 |


### Symbol:

![image](https://github.com/user-attachments/assets/e778b15d-9fa1-41a3-a75c-50fd50839e8c)


# 5.NOR GATE

* It’s NOT-OR gate — the output is true only when all inputs are false.
* It outputs **1** if all inputs are 0, else outputs 0.

### Truth Table (2-input NOR gate):

| Input A | Input B | Output (A NOR B) |
| ------- | ------- | ---------------- |
| 0       | 0       | 1                |
| 0       | 1       | 0                |
| 1       | 0       | 0                |
| 1       | 1       | 0                |


# Symbol:

![image](https://github.com/user-attachments/assets/3c3e88e0-6c59-4be3-8378-14e478461cdd)


# 6.XOR GATE

* Outputs 1 if the inputs are different.
  
* Outputs 0 if the inputs are the same.

---

### Truth Table (2-input XOR gate):

| Input A | Input B | Output (A XOR B) |
| ------- | ------- | ---------------- |
| 0       | 0       | 0                |
| 0       | 1       | 1                |
| 1       | 0       | 1                |
| 1       | 1       | 0                |


### Symbol: 

![image](https://github.com/user-attachments/assets/8ab12f1d-e963-4a60-9e25-0e380cea3308)


# 7.XNOR GATE

* It outputs 1 if the inputs are the same (both 0 or both 1).
* 
* It outputs 0 if the inputs are different.

---

### Truth Table (2-input XNOR gate):

| Input A | Input B | Output (A XNOR B) |
| ------- | ------- | ----------------- |
| 0       | 0       | 1                 |
| 0       | 1       | 0                 |
| 1       | 0       | 0                 |
| 1       | 1       | 1                 |


### Symbol: 

![image](https://github.com/user-attachments/assets/6c954d16-0ade-459d-b01d-2447943fb80b)

# Integrated Circuits-IC's

**What is an IC**

An IC is a small electronic device made of a semiconductor material, usually silicon, that contains many microscopic components (like transistors, resistors, and capacitors). Found in virtually all electronic equipment (computers, phones, etc.).

Example: A microprocessor is an example of an IC.

**Types of Logic Gates and Their IC's**

| Gate Type | Symbol | Common IC   | No. of Gates in IC | Pin Count | Notes                                                |
| --------- | ------ | ----------- | ------------------ | --------- | ---------------------------------------------------- |
| AND       | ∧      | **7408**    | 4 gates            | 14 pins   | 2 inputs per gate                                    |
| OR        | ∨      | **7432**    | 4 gates            | 14 pins   | 2 inputs per gate                                    |
| NOT       | ¬      | **7404**    | 6 inverters        | 14 pins   | 1 input per gate                                     |
| NAND      | ↑      | **7400**    | 4 gates            | 14 pins   | 2 inputs per gate                                    |
| NOR       | ↓      | **7402**    | 4 gates            | 14 pins   | 2 inputs per gate                                    |
| XOR       | ⊕      | **7486**    | 4 gates            | 14 pins   | 2 inputs per gate                                    |
| XNOR      | ⊙      | **74LS266** | 4 gates            | 14 pins   | 2 inputs per gate (some versions are open-collector) |

**1. 7408 IC - AND GATE**

![image](https://github.com/user-attachments/assets/f43bd36c-0e72-4638-a4dc-43ce3a8ea894)

![image](https://github.com/user-attachments/assets/3f17982b-8f95-456d-be69-e373ef7143e0)

Description: The IC 7408 is a Quad 2-Input AND Gate integrated circuit. It is a digital logic IC that contains four independent AND gates, each with two inputs and one output. This IC is part of the 7400 series of TTL (Transistor-Transistor Logic) chips.

Each AND gate in the IC performs the logical AND operation, which outputs HIGH (1) only when both inputs are HIGH (1). Otherwise, the output remains LOW (0).

| **Pin No.** | **Name** | **Description**                  |
| ----------- | -------- | -------------------------------- |
| 1           | 1A       | Input A of Gate 1                |
| 2           | 1B       | Input B of Gate 1                |
| 3           | 1Y       | Output of Gate 1                 |
| 4           | 2A       | Input A of Gate 2                |
| 5           | 2B       | Input B of Gate 2                |
| 6           | 2Y       | Output of Gate 2                 |
| 7           | GND      | Ground (0V)                      |
| 8           | 3Y       | Output of Gate 3                 |
| 9           | 3B       | Input B of Gate 3                |
| 10          | 3A       | Input A of Gate 3                |
| 11          | 4Y       | Output of Gate 4                 |
| 12          | 4B       | Input B of Gate 4                |
| 13          | 4A       | Input A of Gate 4                |
| 14          | Vcc      | Power Supply (+5V for TTL logic) |

**2. 7432 IC - OR GATE**

![image](https://github.com/user-attachments/assets/78a25972-cd4e-499b-8c67-bfd827dfe799)

![image](https://github.com/user-attachments/assets/825c6ffa-5eed-48d7-be0d-1ec1988cbf93)

Description: The OR gate IC, commonly represented by the 7432 IC in TTL logic families, contains four independent 2-input OR gates.

An OR gate is a basic digital logic gate that outputs HIGH (1) if any one or both of its inputs are HIGH (1). It only outputs LOW (0) when all inputs are LOW (0).

| **Pin Number** | **Pin Name** | **Description**             |
| -------------- | ------------ | --------------------------- |
| 1              | 1A           | Input A of OR Gate 1        |
| 2              | 1B           | Input B of OR Gate 1        |
| 3              | 1Y           | Output of OR Gate 1         |
| 4              | 2A           | Input A of OR Gate 2        |
| 5              | 2B           | Input B of OR Gate 2        |
| 6              | 2Y           | Output of OR Gate 2         |
| 7              | GND          | Ground (0V)                 |
| 8              | 3Y           | Output of OR Gate 3         |
| 9              | 3B           | Input B of OR Gate 3        |
| 10             | 3A           | Input A of OR Gate 3        |
| 11             | 4Y           | Output of OR Gate 4         |
| 12             | 4B           | Input B of OR Gate 4        |
| 13             | 4A           | Input A of OR Gate 4        |
| 14             | Vcc          | Positive power supply (+5V) |

**3. 7404 IC - NOT GATE**

![image](https://github.com/user-attachments/assets/73c9eebf-ff91-4ba9-b58b-90562071988f)

![image](https://github.com/user-attachments/assets/2cd61a62-480c-4b37-8d48-d5eff1f6d01f)

Description: The 7404 IC is a Hex Inverter, meaning it contains 6 independent NOT gates. Each NOT gate takes a single input and outputs the inverted logic level.

If the input is HIGH (1), the output is LOW (0).

If the input is LOW (0), the output is HIGH (1).

This IC is commonly used in digital electronics for signal inversion and logical negation.

| Pin No. | Pin Name | Description          |
| ------- | -------- | -------------------- |
| 1       | 1A       | Input of NOT Gate 1  |
| 2       | 1Y       | Output of NOT Gate 1 |
| 3       | 2A       | Input of NOT Gate 2  |
| 4       | 2Y       | Output of NOT Gate 2 |
| 5       | 3A       | Input of NOT Gate 3  |
| 6       | 3Y       | Output of NOT Gate 3 |
| 7       | GND      | Ground (0V)          |
| 8       | 4Y       | Output of NOT Gate 4 |
| 9       | 4A       | Input of NOT Gate 4  |
| 10      | 5Y       | Output of NOT Gate 5 |
| 11      | 5A       | Input of NOT Gate 5  |
| 12      | 6Y       | Output of NOT Gate 6 |
| 13      | 6A       | Input of NOT Gate 6  |
| 14      | Vcc      | Power supply (+5V)   |

**4. 7400 IC - NAND GATE**

![image](https://github.com/user-attachments/assets/2388c74f-d9b9-490d-88f4-ed105c616fc1)

![image](https://github.com/user-attachments/assets/e87ebbe4-405c-4465-b69c-177ba8b3b81f)

Description: The 7400 IC is a quad 2-input NAND gate integrated circuit. It contains four independent NAND gates, each having two inputs and one output. This IC belongs to the 7400 TTL logic family, widely used in digital electronics.

How the NAND Gate Works:
A NAND gate gives a LOW (0) output only when both inputs are HIGH (1).

In all other cases, the output is HIGH (1).

It’s the inverse of the AND gate.

| Pin No. | Pin Name | Description            |
| ------- | -------- | ---------------------- |
| 1       | 1A       | Input 1 of NAND Gate 1 |
| 2       | 1B       | Input 2 of NAND Gate 1 |
| 3       | 1Y       | Output of NAND Gate 1  |
| 4       | 2A       | Input 1 of NAND Gate 2 |
| 5       | 2B       | Input 2 of NAND Gate 2 |
| 6       | 2Y       | Output of NAND Gate 2  |
| 7       | GND      | Ground (0V)            |
| 8       | 3Y       | Output of NAND Gate 3  |
| 9       | 3A       | Input 1 of NAND Gate 3 |
| 10      | 3B       | Input 2 of NAND Gate 3 |
| 11      | 4Y       | Output of NAND Gate 4  |
| 12      | 4A       | Input 1 of NAND Gate 4 |
| 13      | 4B       | Input 2 of NAND Gate 4 |
| 14      | Vcc      | Power Supply (+5V)     |

**5. 7402 IC - NOR GATE**

![image](https://github.com/user-attachments/assets/0e53d122-f5ef-4fce-b1be-63d55fedf258)

![image](https://github.com/user-attachments/assets/b93d5e54-2d7b-458a-a426-fc9fb29fcc1d)

Description:

The 7402 IC contains four independent 2-input NOR gates.

A NOR gate gives a HIGH output only when both inputs are LOW.

It is the inverse of the OR gate.

| Pin No. | Pin Name | Description           |
| ------- | -------- | --------------------- |
| 1       | 1A       | Input A of NOR Gate 1 |
| 2       | 1B       | Input B of NOR Gate 1 |
| 3       | 1Y       | Output of NOR Gate 1  |
| 4       | 2A       | Input A of NOR Gate 2 |
| 5       | 2B       | Input B of NOR Gate 2 |
| 6       | 2Y       | Output of NOR Gate 2  |
| 7       | GND      | Ground (0V)           |
| 8       | 3Y       | Output of NOR Gate 3  |
| 9       | 3B       | Input B of NOR Gate 3 |
| 10      | 3A       | Input A of NOR        |


**6. 7486 IC - XOR GATE**

![image](https://github.com/user-attachments/assets/3db9e2a7-48e3-438b-b450-28f0b75c016b)

![image](https://github.com/user-attachments/assets/4cea9ef9-3644-44bb-b3d8-ca285ee95779)

Description:

The 7486 IC includes four 2-input XOR (Exclusive OR) gates.

XOR gates output HIGH only when inputs are different.

Useful in arithmetic circuits, parity checkers, and logic comparisons.

| Pin No. | Pin Name | Description           |
| ------- | -------- | --------------------- |
| 1       | 1A       | Input A of XOR Gate 1 |
| 2       | 1B       | Input B of XOR Gate 1 |
| 3       | 1Y       | Output of XOR Gate 1  |
| 4       | 2A       | Input A of XOR Gate 2 |
| 5       | 2B       | Input B of XOR Gate 2 |
| 6       | 2Y       | Output of XOR Gate 2  |
| 7       | GND      | Ground (0V)           |
| 8       | 3Y       | Output of XOR Gate 3  |
| 9       | 3B       | Input B of XOR Gate 3 |
| 10      | 3A       | Input A of XOR Gate 3 |
| 11      | 4Y       | Output of XOR Gate 4  |
| 12      | 4B       | Input B of XOR Gate 4 |
| 13      | 4A       | Input A of XOR Gate 4 |
| 14      | Vcc      | Supply Voltage (+5V)  |


**7. 74LS266 IC - XNOR GATE**

![image](https://github.com/user-attachments/assets/7ee83fbf-3646-4067-9423-f250894cbda7)

![image](https://github.com/user-attachments/assets/a4cf92dc-b8ac-4b40-ab66-73050b1dbb7b)

Description: 

The 74LS266 IC is similar to 7486 but includes open collector outputs.

Open collector allows multiple gate outputs to be connected together (wired-AND logic).

Ideal for bus systems and multi-device communication.

| Pin No. | Pin Name | Description                           |
| ------- | -------- | ------------------------------------- |
| 1       | 1A       | Input A of XOR Gate 1                 |
| 2       | 1B       | Input B of XOR Gate 1                 |
| 3       | 1Y       | Output of XOR Gate 1 (Open Collector) |
| 4       | 2A       | Input A of XOR Gate 2                 |
| 5       | 2B       | Input B of XOR Gate 2                 |
| 6       | 2Y       | Output of XOR Gate 2 (Open Collector) |
| 7       | GND      | Ground (0V)                           |
| 8       | 3Y       | Output of XOR Gate 3 (Open Collector) |
| 9       | 3B       | Input B of XOR Gate 3                 |
| 10      | 3A       | Input A of XOR Gate 3                 |
| 11      | 4Y       | Output of XOR Gate 4 (Open Collector) |
| 12      | 4B       | Input B of XOR Gate 4                 |
| 13      | 4A       | Input A of XOR Gate 4                 |
| 14      | Vcc      | Power Supply (+5V)                    |













