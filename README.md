# Digital Electronics Internship

# Table of contents

- [What is Digital Electronics](#what-is-digital-electronics)
- [Applications of Digital Electronics](#applications-of-digital-electronics)
- [Digital vs Analog Signals](#digital-vs-analog-signals)
- [Number Systems](#number-systems)
- [Conversion between Number Systems](#conversion-between-number-systems)
- [Basic Logic Gates](#basic-logic-gates)
- [Implementation of Logic Gates Using Integrated Circuits - IC's](#implementation-of-logic-gates-using-integrated-circuits---ics)
- [IMPLEMENTATION OF HALF ADDER](#implementation-of-half-adder)
- [IMPLEMENTATION OF FULL ADDER](#implementation-of-full-adder)
- [MULTIPLEXERS](#multiplexers)
- [2x1 MULTIPLEXER](#2x1-multiplexer)
- [4x1 MUTIPLEXER](#4x1-mutiplexer)
  
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

| S.No | Conversion Type        | Example Input | Steps / Explanation                                                                                  | Result     |
| ---- | ---------------------- | ------------- | ---------------------------------------------------------------------------------------------------- | ---------- |
| 1    | **Binary to Decimal**      | 101101        | 1×2⁵ + 0×2⁴ + 1×2³ + 1×2² + 0×2¹ + 1×2⁰ = 32 + 0 + 8 + 4 + 0 + 1                                 | 45₁₀       |
| 2    | **Decimal to Binary**      | 45            | Division by 2: Remainders → 1 0 1 1 0 1 (read bottom-up)                                         | 101101₂    |
| 3    | **Decimal to Octal**       | 45            | 45 ÷ 8 = 5 R5 → 5 ÷ 8 = 0 R5 → Octal = Reverse of remainders                                     | 55₈        |
| 4    | **Octal to Binary**        | 157₈          | 1 → 001, 5 → 101, 7 → 111 → Combine: 001101111                                                   | 001101111₂ |
| 5    | **Binary to Hexadecimal**  | 10110111      | Group: 1011 (B), 0111 (7)                                                                        | B7₁₆       |
| 6    | **Hexadecimal to Binary**  | 2F₁₆          | 2 → 0010, F → 1111 → 00101111                                                                    | 00101111₂  |
| 7    | **Decimal to Octal**       | 125           | 125 ÷ 8 = 15 R5 → 15 ÷ 8 = 1 R7 → 1 ÷ 8 = 0 R1 → Reverse remainders                              | 175₈       |
| 8    | **Octal to Decimal**       | 175₈          | 1×8² + 7×8¹ + 5×8⁰ = 64 + 56 + 5                                                                 | 125₁₀      |
| 9    | **Decimal to Hexadecimal** | 254           | 254 ÷ 16 = 15 R14 (E), 15 ÷ 16 = 0 R15 (F) → Reverse remainders                                  | FE₁₆       |
| 10   | **Hexadecimal to Decimal** | 2F₁₆          | 2×16¹ + F(15)×16⁰ = 32 + 15                                                                      | 47₁₀       |
| 11   | **Octal to Hexadecimal**   | 175₈          | Octal → Binary: 001 111 101 = 001111101₂ → Pad: 0001 1111 0101 → 1F5                             | 1F5₁₆      |
| 12   | **Hexadecimal to Octal**   | 2F₁₆          | Hex → Binary: 2 = 0010, F = 1111 → 00101111 → Pad into 3-bit: 000 010 111 111 → Groups = 0 2 7 7 | 277₈       |


# Basic Logic Gates

# 1.AND Gate

An AND gate is a basic digital logic gate that outputs 1 (true) only when all its inputs are 1. Otherwise, it outputs 0 (false).

Represented as: A AND B = A ⋅ B or A ∧ B

**Truth Table**

|**A**|**B**| **A & B**|
|-----|----|------|
|0|0|0|
|0|1|0|
|1|0|0|
|1|1|1|

**Key Point:**

Output is true (1) only when both inputs are true (1).

**Symbol:**

<img src="https://github.com/user-attachments/assets/09cb1e97-f756-4b48-be9f-956216a10c82" width="300" />

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

<img src="https://github.com/user-attachments/assets/ad03011b-8014-42db-aad6-628127139c93" width="300" />

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

<img src="https://github.com/user-attachments/assets/ac6475a2-44b4-4bc6-b1e9-c6bee62f13c4" width="300" />

# 4.NAND GATE

**Definition**

A NAND gate is a fundamental digital logic gate that outputs false (0) only when all its inputs are true (1); otherwise, it outputs true (1).

### Truth Table (2-input NAND gate):

| Input A | Input B | Output (A NAND B) |
| ------- | ------- | ----------------- |
| 0       | 0       | 1                 |
| 0       | 1       | 1                 |
| 1       | 0       | 1                 |
| 1       | 1       | 0                 |


### Symbol:

<img src="https://github.com/user-attachments/assets/43531a7f-350f-4d35-8c37-589b1e89ee99" width="300" />

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

<img src="https://github.com/user-attachments/assets/9805dcb4-97d2-48ba-912e-6cc9f5932daa" width="300" />

# 6.XOR GATE

* Outputs 1 if the inputs are different.
  
* Outputs 0 if the inputs are the same.

### Truth Table (2-input XOR gate):

| Input A | Input B | Output (A XOR B) |
| ------- | ------- | ---------------- |
| 0       | 0       | 0                |
| 0       | 1       | 1                |
| 1       | 0       | 1                |
| 1       | 1       | 0                |


### Symbol: 

<img src="https://github.com/user-attachments/assets/8e657000-92e7-4d27-b17d-69acf030fd99" width="300" />

# 7.XNOR GATE

* It outputs 1 if the inputs are the same (both 0 or both 1).
* It outputs 0 if the inputs are different.

### Truth Table (2-input XNOR gate):

| Input A | Input B | Output (A XNOR B) |
| ------- | ------- | ----------------- |
| 0       | 0       | 1                 |
| 0       | 1       | 0                 |
| 1       | 0       | 0                 |
| 1       | 1       | 1                 |

### Symbol: 

<img src="https://github.com/user-attachments/assets/66024712-e907-4684-8b96-588ce7f86d1b" width="300" />

# Implementation of Logic Gates Using Integrated Circuits - IC's

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

# Applications of Logic Gates

| **Gate** | **IC Number**                           | **Applications**                                                          |
| -------- | --------------------------------------- | ------------------------------------------------------------------------- |
| **AND**  | 7408 (Quad 2-input AND gate)            | **Decision-making** (e.g., **security systems**, **control systems**)     |
|          | 7432 (Quad 2-input OR gate)             | **Multiplexers** (e.g., selecting input based on conditions)              |
| **OR**   | 7432 (Quad 2-input OR gate)             | **Alarm systems** (any condition triggering action)                       |
|          | 7486 (Quad 2-input XOR gate)            | **Control systems** where any input can initiate action                   |
| **NOT**  | 7404 (Hex inverter)                     | **Inversion circuits** (e.g., **complementary systems**, **flip-flops**)  |
| **NAND** | 7400 (Quad 2-input NAND gate)           | **Memory storage** (used in **flip-flops**, **latches**)                  |
|          | 7410 (Triple 3-input NAND gate)         | **Error correction circuits**                                             |
| **NOR**  | 7402 (Quad 2-input NOR gate)            | **Negative logic circuits** (e.g., **reset systems**, **initialization**) |
| **XOR**  | 7486 (Quad 2-input XOR gate)            | **Parity checking** (e.g., **error detection** in data transmission)      |
|          | 7412 (Quad 2-input NAND gate)           | **Digital comparators** (detecting differences between inputs)            |
| **XNOR** | 7485 (Quad 2-input XNOR gate)           | **Equality checkers** (verifying if two inputs match)                     |
|          | 74266 (Quad 2-input Exclusive-NOR gate) | **Parity bit generation** (checking for even parity)                      |

**1. 7408 IC - AND GATE**

<img src="https://github.com/user-attachments/assets/f43bd36c-0e72-4638-a4dc-43ce3a8ea894" width="350" />

![image](https://github.com/user-attachments/assets/10857107-11d2-41a6-80a2-004846ef4059)

<img src="https://github.com/user-attachments/assets/305fc134-0193-4dd4-a5b2-cf767b598a12" width="400" />

**Tinkercad Link**

[AND GATE IC Tinkercad](https://www.tinkercad.com/things/hgTs2riGofA-and-gate-ic-7408)

**Description:** 

An AND gate IC is an integrated circuit that contains multiple AND gates on a single chip. An AND gate is a fundamental digital logic gate that outputs a HIGH signal (1) only when all of its inputs are HIGH. The IC is designed to perform this logical operation electrically.
The internal structure of an AND gate IC is made up of many tiny transistors and other electronic components etched onto a small piece of silicon. These transistors work together to control the flow of electrical signals based on the inputs, producing the correct output according to the AND logic function.

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

<img src="https://github.com/user-attachments/assets/45198fa7-0d6d-474e-8b99-9e085091077d" width="350" />

![image](https://github.com/user-attachments/assets/59c1909c-1fa0-43b4-9f21-da27b86f934a)

<img src="https://github.com/user-attachments/assets/b32beb43-1e13-440a-acae-32aaa0aa924b" width="400" />

**Tinkercad Link**

[OR GATE IC Tinkercad](https://www.tinkercad.com/things/7V7teeZ8tZm-or-gate-ic-7432)

**Description:** 

An OR gate IC is a compact electronic device that contains multiple OR gates integrated onto a single silicon chip. An OR gate is a basic digital logic gate that outputs a HIGH signal (1) if at least one of its inputs is HIGH. The internal circuitry of the OR gate IC is designed to perform this logical operation efficiently using semiconductor components. Inside the IC, millions of tiny transistors and other electronic elements are arranged in such a way that they manipulate electrical signals according to the OR logic. When one or more input signals are at a HIGH voltage level, the transistors inside the IC allow the output to be pulled to a HIGH state. Conversely, if all inputs are LOW, the output remains LOW.

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

<img src="https://github.com/user-attachments/assets/13b52922-b8fc-4163-aa58-001da6ee82e8" width="350" />

![image](https://github.com/user-attachments/assets/a7a4bae7-19e9-4686-971a-5973ef1bc280)

<img src="https://github.com/user-attachments/assets/7e84fd3b-b218-443b-bf43-c94e035c6928" width="400" />

**Tinkercad Link**

[NOT GATE IC Tinkercad](https://www.tinkercad.com/things/aLN9CwaAC5x-not-gate-ic-7404)

**Description:** 

A NOT gate IC, also known as an inverter IC, is an integrated circuit that implements the NOT logic function. The NOT gate takes a single input and produces an output that is the logical complement or inversion of the input signal. In other words, if the input is HIGH (1), the output will be LOW (0), and if the input is LOW (0), the output will be HIGH (1). Inside the IC, this inversion is achieved through a combination of transistors arranged in such a way that the output voltage is opposite to the input voltage. The IC is typically built using semiconductor fabrication technologies such as TTL (Transistor-Transistor Logic) or CMOS (Complementary Metal-Oxide-Semiconductor), which allow the creation of multiple NOT gates on a single silicon chip. For example, the 7404 IC contains six independent NOT gates. 

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

<img src="https://github.com/user-attachments/assets/0c98af27-1036-48c9-b111-bc712ced0b48" width="350" />

![image](https://github.com/user-attachments/assets/fba78895-ca0f-41b9-923f-918ab8d6d245)

<img src="https://github.com/user-attachments/assets/3c647af5-7428-4740-b76c-fff9415152fe" width="400" />

**Tinkercad Link**

[NAND GATE IC Tinkercad](https://www.tinkercad.com/things/je7Ft3yBEBO-nand-gate-ic-7400)

**Description:** 

A NAND gate IC is an integrated circuit that contains several NAND gates, which are fundamental building blocks in digital electronics. A NAND gate produces an output that is LOW only when all its inputs are HIGH; otherwise, its output is HIGH. Essentially, it is the complement of the AND gate. Inside the NAND gate IC, the logic operation is realized using a network of transistors and other semiconductor components fabricated on a tiny silicon chip. These components are arranged so that the electrical signals applied at the inputs control the flow of current through the transistors, determining the output voltage level according to the NAND logic.

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

<img src="https://github.com/user-attachments/assets/6b2eac61-21c1-4f70-b073-137ba249e327" width="350" />

![image](https://github.com/user-attachments/assets/2bf6f9ee-3e20-4dc7-85df-a75dc4760d39)

<img src="https://github.com/user-attachments/assets/93aec80b-0301-4bf0-a44a-9970af68156d" width="400" />

**Tinkercad Link**

[NOR GATE IC Tinkercad](https://www.tinkercad.com/things/3FRNHH2hQEo-nor-gate-ic-7402)

**Description:**

A NOR gate IC is an integrated circuit that contains multiple NOR gates within a single semiconductor chip. A NOR gate is a basic digital logic gate that produces a HIGH output only when all its inputs are LOW. If any of the inputs are HIGH, the output will be LOW. Essentially, the NOR gate combines the functions of an OR gate followed by a NOT gate, meaning it outputs the inverse of the OR operation. Inside the NOR gate IC, tiny electronic components such as transistors are fabricated on a silicon wafer using semiconductor manufacturing processes. These transistors are interconnected in a way that enables them to perform the NOR logic function. When electrical signals representing logical values (HIGH or LOW) are applied to the inputs, the transistors switch states to control the flow of current, thereby determining the output signal.

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

<img src="https://github.com/user-attachments/assets/f0777402-04f9-440b-b2fd-193136e46fd8" width="350" />

![image](https://github.com/user-attachments/assets/d6f3a466-b078-4ba3-86e8-1556eeb4636f)

<img src="https://github.com/user-attachments/assets/4992fbad-d5ea-466d-8b38-83b03535e1c3" width="400" />

**Tinkercad Link**

[XOR GATE IC Tinkercad](https://www.tinkercad.com/things/6naD4VcsiNA-xor-gate-ic-7486)

**Description:**

An XOR (exclusive OR) gate IC is an integrated circuit designed to perform the exclusive OR logical operation on its inputs. The XOR gate outputs a HIGH signal only when an odd number of its inputs are HIGH; for two inputs, this means the output is HIGH if exactly one input is HIGH, and LOW if both inputs are the same (both HIGH or both LOW). Inside the XOR gate IC, tiny semiconductor devices such as transistors are arranged in a specific configuration that allows the chip to perform this function. These transistors control the flow of electric current based on the inputs, ensuring that the output accurately reflects the XOR logic.

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

<img src="https://github.com/user-attachments/assets/765ea0b9-fe12-4327-b131-ec74b6ddf998" width="350" />

![image](https://github.com/user-attachments/assets/b8640aab-c398-46c6-a2de-fc4e169fac6c)

<img src="https://github.com/user-attachments/assets/6f32e846-d99c-436a-b6b4-734d8e8de14f" width="400" />

**Tinkercad Link**

[XNOR GATE IC Tinkercad](https://www.tinkercad.com/things/k2SIEZURJmN-xnor-gate-ic)

**Description:** 

An XNOR gate IC is a type of integrated circuit that contains one or more XNOR (exclusive-NOR) logic gates on a single silicon chip. The XNOR gate is a fundamental digital logic gate that outputs a HIGH signal only when its inputs are equal — either both HIGH or both LOW. In other words, it performs the logical equivalence operation. Inside the XNOR gate IC, the logic function is realized by a network of transistors and other semiconductor components fabricated on a small piece of silicon. These transistors are arranged so that they control the flow of electrical current to produce the correct output depending on the inputs.

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

# IMPLEMENTING AND GATE USING NAND GATE

<img src="https://github.com/user-attachments/assets/8221c86a-edd1-4cc4-bc38-f89cd42c2f18" width="400" />

**Tinkercad Link**

[AND GATE USING NAND GATE Tinkercad](https://www.tinkercad.com/things/kUNVNNtWxwI-and-using-nand-gate)

# IMPLEMENTING OR GATE USING AND GATE

<img src="https://github.com/user-attachments/assets/3a6f18eb-aff8-4273-8729-cbd5a98480fd" width="400"/>

**Tinkercad Link**

[OR GATE USING AND GATE Tinkercad](https://www.tinkercad.com/things/endyNZVZ2Ew-or-using-nand)

# IMPLEMENTING NOT GATE USING NAND GATE

<img src="https://github.com/user-attachments/assets/23993339-7e02-4b53-adde-b7e567db1fb1" width="400"/>

**Tinkercad Link**

[NOT GATE USING NAND GATE Tinkercad](https://www.tinkercad.com/things/6rPcfqVliYz-not-gate-using-nand-gate)

# IMPLEMENTING AND GATE USING NOR GATE

<img src="https://github.com/user-attachments/assets/105b7216-7458-41af-904a-375f3b1024c7" width="400"/>

**Tinkercad Link**

[AND GATE USING NOR GATE Tinkercad](https://www.tinkercad.com/things/2GPXqiYO7ux-and-using-nor-gate)

# IMPLEMENTING OR GATE USING NOR GATE

<img src="https://github.com/user-attachments/assets/e3c69e74-ba24-4e1a-a62b-a18b9fcea033" width="400" />

**Tinkercad Link**

[OR GATE USING NOR GATE Tinkercad](https://www.tinkercad.com/things/4ex3zPNHxup-or-gate-using-nor-gate)

# IMPLEMENTING NOT GATE USING NOR GATE

<img src="https://github.com/user-attachments/assets/c55b53b5-141e-422d-9388-00168cab2d51" width="400" />

**Tinkercad Link**

[NOT GATE USING NOR GATE Tinkercad](https://www.tinkercad.com/things/f87kXOgLGX0-not-gate-using-nor-gate)

# IMPLEMENTATION OF HALF ADDER 

**Block Diagram**

<img src="https://github.com/user-attachments/assets/b3281d2e-194d-45fb-a6ee-758a5357633c" width="500">

<img src="https://github.com/user-attachments/assets/1c308a20-f36d-4127-be96-9b0b008262ab" width="600"/>

**Tinkercad Link**

[Half Adder Tinkercad](https://www.tinkercad.com/things/gebKFc0umAi-half-adder-using-nand-gate)

**Half Adder Using 7400 NAND ICs Connection Table**

| **From Pin**      | **To Pin**            | **Purpose**                         |
| ----------------- | --------------------- | ----------------------------------- |
| DIP Switch 1      | Pin 1 (IC1 - 74HC00)  | Input A to NAND1                    |
| DIP Switch 2      | Pin 2 (IC1)           | Input B to NAND1                    |
| Pin 3 (IC1)       | Pin 4 (IC1)           | Output of NAND1 to input of NAND2   |
| DIP Switch 1      | Pin 5 (IC1)           | A again to NAND2                    |
| Pin 6 (IC1)       | Pin 9 (IC1)           | Output of NAND2 to input of NAND3   |
| DIP Switch 2      | Pin 10 (IC1)          | B again to NAND3                    |
| Pin 8 (IC1)       | Pin 12 (IC1)          | Output of NAND3 to NAND4            |
| Pin 3 (IC1)       | Pin 13 (IC1)          | NAND1 output to NAND4               |
| Pin 11 (IC1)      | LED (Sum Output)      | Output of NAND4 = Final SUM         |
| DIP Switch 3      | Pin 1 (IC2 - 74HC00)  | Carry-in to NAND5                   |
| Pin 11 (IC1)      | Pin 2 (IC2)           | SUM (from NAND4) to NAND5 for Carry |
| Pin 3 (IC2)       | Pin 4 (IC2)           | Output of NAND5 to input of NAND6   |
| DIP Switch 3      | Pin 5 (IC2)           | Cin again to NAND6                  |
| Pin 6 (IC2)       | LED (Carry Output)    | Final Carry Output                  |
| Pin 14 (both ICs) | +5V (Red Power Rail)  | VCC to both NAND ICs                |
| Pin 7 (both ICs)  | GND (Blue Power Rail) | Ground to both NAND ICs             |


**Description**

-Pin 3 provides the Carry output.

-Pin 6 can be used as part of Sum (XOR) if extended with additional NANDs.

**Half Adder Truth Table**

| A | B | SUM (A ⊕ B) | CARRY (A · B) |
| - | - | ----------- | ------------- |
| 0 | 0 | 0           | 0             |
| 0 | 1 | 1           | 0             |
| 1 | 0 | 1           | 0             |
| 1 | 1 | 0           | 1             |

# IMPLEMENTATION OF FULL ADDER

**Block Diagram**

<img src="https://github.com/user-attachments/assets/c953c83c-eda8-47da-93f4-37da31debd65" width="500" />


**Full Adder Using XOR, AND, OR GATES**

<img src="https://github.com/user-attachments/assets/ef2f6063-a8e8-462e-b95a-a65bae5c8e1c" width="600" />

**Full Adder Using NOR GATE**

<img src="https://github.com/user-attachments/assets/809760f8-21ad-4e9a-b373-cdbdae06f6ad" width="600" />

**Tinkercad Link**

[FULL ADDER USING NOR GATE Tinkercad](https://www.tinkercad.com/things/hZOS6CWrOht-full-adder-using-nor-gate)

**Full Adder Using 7402 NOR GATE IC's Connection Table**

| **From Pin**     | **To Pin**           | **Purpose**                                         |
| ---------------- | -------------------- | --------------------------------------------------- |
| DIP Switch 1     | Pin 1 (IC1 - 74HC02) | Input A to NOR gate 1                               |
| DIP Switch 2     | Pin 2 (IC1)          | Input B to NOR gate 1                               |
| Pin 3 (IC1)      | Pin 5 (IC1)          | Output of NOR1 → input of NOR2                      |
| Pin 3 (IC1)      | Pin 10 (IC2)         | Output of NOR1 → input of NOR3                      |
| DIP Switch 1     | Pin 4 (IC1)          | A again to input of NOR2                            |
| Pin 6 (IC1)      | Pin 12 (IC2)         | Output of NOR2 → input of NOR4                      |
| DIP Switch 2     | Pin 9 (IC2)          | B again to input of NOR3                            |
| Pin 8 (IC2)      | Pin 13 (IC2)         | Output of NOR3 → input of NOR4                      |
| Pin 11 (IC2)     | LED (Sum Output)     | Output of NOR4 = Final XOR (SUM)                    |
| DIP Switch 3     | Pin 2 (IC3)          | Carry-in to NOR6 input                              |
| Pin 3 (IC1)      | Pin 1 (IC3)          | Output of NOR1 → input to NOR6 for carry generation |
| Pin 3 (IC3)      | Pin 5 (IC3)          | Output of NOR6 → input of NOR7                      |
| DIP Switch 3     | Pin 4 (IC3)          | Carry-in again → input of NOR7                      |
| Pin 6 (IC3)      | LED (Carry Output)   | Output of NOR7 = Final Carry                        |
| Pin 14 (all ICs) | +5V (Red rail)       | Power supply to all ICs                             |
| Pin 7 (all ICs)  | GND (Blue rail)      | Ground connection to all ICs                        |

**Full Adder Truth Table**

| **A** | **B** | **Cin** | **Sum** | **Carry** |
| :---: | :---: | :-----: | :-----: | :-------: |
|   0   |   0   |    0    |    0    |     0     |
|   0   |   0   |    1    |    1    |     0     |
|   0   |   1   |    0    |    1    |     0     |
|   0   |   1   |    1    |    0    |     1     |
|   1   |   0   |    0    |    1    |     0     |
|   1   |   0   |    1    |    0    |     1     |
|   1   |   1   |    0    |    0    |     1     |
|   1   |   1   |    1    |    1    |     1     |

# MULTIPLEXERS

**What is Multiplexers**

A multiplexer (MUX) is a logic circuit that selects one of several input signals and directs it to a single output. It acts like a digital switch, choosing which input to forward based on a selection input. Multiplexers are commonly used in digital logic circuits to handle multiple data inputs and route them to a single output line. 

**Key Characteristics of a Multiplexer:**

Multiple Inputs: A multiplexer has several input lines, which represent the data signals to be selected. 

Single Output:It has one output line that carries the selected input signal. 

Selection Inputs:Control lines called "select lines" determine which input is routed to the output. 

Data Selector:Multiplexers are also known as "data selectors" because they select which data to send to the output. 

# 2x1 MULTIPLEXER

A 2:1 multiplexer (MUX) is a digital logic device that allows one of two binary inputs to be routed to a single output, depending on the value of a select input. It is an essential building block in digital systems used for data selection and control.The basic principle behind a 2:1 multiplexer is selection. 
The multiplexer examines the value of the select line (S) and chooses between the two inputs:

• If the select line is 0, the output is connected to input I₀

• If the select line is 1, the output is connected to input I₁

• A 2:1 MUX is fundamental for decision-making processes in circuits.

• It is used in ALUs (Arithmetic Logic Units), data buses, and memory selection logic.

• By combining multiple 2:1 multiplexers, larger multiplexers can be constructed (e.g., 4:1, 8:1 MUX).

**Applications:**

•  Register File Access

• Data Bus Control

• Serial Data Transmission

• Interrupt Handling

• Embedded Systems / Microcontrollers

**Block Diagram**

<img src="https://github.com/user-attachments/assets/c18f0a6c-9b4d-41ef-8237-76baae7637e7" width="600">

<img src="https://github.com/user-attachments/assets/2ba58f68-9fa6-44ab-b9d1-0d9380858168" width="600"/>

**Tinkercad Link**

[2x1 Multiplexer Tinkercad](https://www.tinkercad.com/things/0d5xd9rGBOn-2x1-multiplexer)

**2x1 Multiplexer Pin to Pin Connection Table**

| **From Pin**     | **To Pin**           | **Purpose**                             |
| ---------------- | -------------------- | --------------------------------------- |
| DIP Switch 1     | Pin 1 (IC1 - 74HC02) | Input A to NOR gate 1                   |
| DIP Switch 2     | Pin 2 (IC1)          | Input B to NOR gate 1                   |
| Pin 3 (IC1)      | Pin 5 (IC1)          | Output of NOR1 → input of NOR2          |
| Pin 3 (IC1)      | Pin 10 (IC2)         | Output of NOR1 → input of NOR3          |
| DIP Switch 1     | Pin 4 (IC1)          | A again → input of NOR2                 |
| Pin 6 (IC1)      | Pin 12 (IC2)         | Output of NOR2 → input of NOR4          |
| DIP Switch 2     | Pin 9 (IC2)          | B again → input of NOR3                 |
| Pin 8 (IC2)      | Pin 13 (IC2)         | Output of NOR3 → input of NOR4          |
| Pin 11 (IC2)     | LED (Sum Output)     | Output of NOR4 = Final XOR → SUM output |
| DIP Switch 3     | Pin 2 (IC3)          | Carry-in to NOR6 input                  |
| Pin 3 (IC1)      | Pin 1 (IC3)          | Output of NOR1 → input of NOR6          |
| Pin 3 (IC3)      | Pin 5 (IC3)          | Output of NOR6 → input of NOR7          |
| DIP Switch 3     | Pin 4 (IC3)          | Carry-in again → input of NOR7          |
| Pin 6 (IC3)      | LED (Carry Output)   | Output of NOR7 = Final Carry            |
| Pin 14 (all ICs) | +5V (Red rail)       | Power supply to all ICs                 |
| Pin 7 (all ICs)  | GND (Blue rail)      | Ground connection to all ICs            |

**Truth Table**

| **SL (Select Line)** | **IN1** | **IN2** | **OUT** |
| -------------------- | ------- | ------- | ------- |
| 0                    | 0       | 0       | 0       |
| 0                    | 0       | 1       | 0       |
| 0                    | 1       | 0       | 1       |
| 0                    | 1       | 1       | 1       |
| 1                    | 0       | 0       | 0       |
| 1                    | 0       | 1       | 1       |
| 1                    | 1       | 0       | 0       |
| 1                    | 1       | 1       | 1       |

# 4x1 MUTIPLEXER 

A 4×1 multiplexer (also written as 4-to-1 MUX) is a combinational digital circuit that selects one input from four available data inputs and forwards it to a single output line. The selection of which input to send is controlled by two select lines. To perform this selection, the multiplexer uses a combination of basic logic gates such as AND, OR, and NOT gates. Each input line is connected to one AND gate, which is also fed by a specific combination of the select line values. These gates ensure that only the selected input—based on the select line combination—is allowed to reach the output. The outputs of the AND gates are then combined through an OR gate to produce the final output signal.

**Applications:**

- Used in data routing and signal selection.

- Essential in digital communication systems, microprocessors, and memory units.

- Helps in implementing complex logic circuits by using multiplexing instead of many separate logic gates.

**Advantages:**

- Efficient method for signal selection

- Simplifies circuit design

- Reduces the number of logic gates required for complex functions

**Block Diagram**

![WhatsApp Image 2025-05-29 at 12 25 26_e218cea1](https://github.com/user-attachments/assets/5ee3143c-912b-4c55-a927-21e108a1f32d)

<img src="https://github.com/user-attachments/assets/67572133-bde6-43e3-b782-52fd23b79c29" width="600" />

**Tinkercad Link**

[4x1 Multiplexer](https://www.tinkercad.com/things/7Uxe7fvbTzl-4x1-multiplexer-using-7408-7432-7404)

**4x1 Multiplexer Pin to Pin Connection Table**

| From Pin             | To Pin                          | Purpose                                   |
| -------------------- | ------------------------------- | ----------------------------------------- |
| DIP Switch 1         | Pin 1 (IC1 - 74HC08)            | Input A to AND gate 1                     |
| DIP Switch 2         | Pin 2 (IC1 - 74HC08)            | Input B to AND gate 1                     |
| Pin 3 (IC1)          | Pin 5 (IC1)                     | Output of AND1 → input of AND2            |
| DIP Switch 1         | Pin 4 (IC1)                     | A again → input of AND2                   |
| Pin 6 (IC1)          | Pin 2 (IC3 - 74HC32)            | Output of AND2 → input of OR gate         |
| DIP Switch 2         | Pin 9 (IC2 - 74HC08)            | B again → input of AND3                   |
| Pin 3 (IC1)          | Pin 10 (IC2 - 74HC08)           | Output of AND1 → input of AND3            |
| Pin 8 (IC2)          | Pin 1 (IC3 - 74HC32)            | Output of AND3 → input of OR gate         |
| Pin 3 (IC3 - 74HC32) | LED (Sum Output via resistor)   | Output of OR gate = Final SUM output      |
| DIP Switch 3         | Pin 3 (IC4 - 74HC04)            | Carry-in to NOT gate input                |
| Pin 4 (IC4)          | Pin 1 (IC1 - reused)            | Inverted Carry-in → possibly reused logic |
| Pin 3 (IC1)          | Pin 13 (IC3 - 74HC32)           | Output of AND1 → OR for carry             |
| DIP Switch 3         | Pin 12 (IC3)                    | Carry-in again → OR for carry             |
| Pin 11 (IC3)         | LED (Carry Output via resistor) | Output of OR gate = Final Carry output    |
| Pin 14 (All ICs)     | +5V (Red rail)                  | Power supply to all ICs                   |
| Pin 7 (All ICs)      | GND (Blue rail)                 | Ground connection for all ICs             |

**Truth Table**

| S1 | S0 | A | B | C | D | Out |
| -- | -- | - | - | - | - | --- |
| 0  | 0  | 0 | x | x | x | 0   |
| 0  | 0  | 1 | x | x | x | 1   |
| 0  | 1  | x | 0 | x | x | 0   |
| 0  | 1  | x | 1 | x | x | 1   |
| 1  | 0  | x | x | 0 | x | 0   |
| 1  | 0  | x | x | 1 | x | 1   |
| 1  | 1  | x | x | x | 0 | 0   |
| 1  | 1  | x | x | x | 1 | 1   |














