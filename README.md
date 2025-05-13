# Digital-electronics_-internship


# Task 1

# What is Digital Electronics?

Digital electronics is a branch of electronics that deals with systems and devices that use digital signals, which are discrete representations of data, 
typically using binary code (0s and 1s).


# Applications of Digital Electronics?

1.Computing

2.Communication

3.Control Systems

4.Home Appliances

5.Medical Devices

6.Automotive

7.Security Systems

8.Industrial automation


# Digital vs Analog signals?

Analog Signals:

Continuous:

They can take on any value within a range, unlike digital signals which are discrete.

Examples:

Sound waves, voltage fluctuations, radio waves, and the hands of a clock. 

High Fidelity:
They can reproduce the original information with high fidelity, but may not be as robust over long distances. 

Digital Signals:

Discrete:

They represent information using a limited set of values, typically binary code (0s and 1s). 
Examples:

Digital clocks, computers, and most modern communication systems. 
Robust to Noise:

Digital signals are more resilient to noise because they can be easily regenerated. 
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

# Logic Levels?

In digital electronics, logic levels refer to the specific voltage ranges used to represent the two binary states: 

0 (low) and 1 (high).

**Common Logic Families and Their Voltage Levels:**

| **Logic Family** |	**Logic Low (0)** |	**Logic High (1)** |
|------------------|--------------------|---------------------|
|TTL (5V) |	0V to 0.8V |	2V to 5V|
|CMOS (5V)|	0V to 1.5V|	3.5V to 5V|
|CMOS (3.3V) |	0V to 1V |	2.3V to 3.3V|

# Number Systems?

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

**1. Decimal → Binary**
Method: Divide the number by 2 repeatedly, write down remainders in reverse.

Example: 13 ÷ 2 = 6 R1 6 ÷ 2 = 3 R0 3 ÷ 2 = 1 R1 1 ÷ 2 = 0 R1 → Binary: 1101

**2. Binary → Decimal**
Method: Multiply each binary digit by 2 raised to its position (from right to left), then sum.

Example: 1101 = 1×2³ + 1×2² + 0×2¹ + 1×2⁰ = 8 + 4 + 0 + 1 = 13

**3. Decimal → Octal**
Method: Divide the decimal by 8 repeatedly, reverse remainders.

Example: 65 ÷ 8 = 8 R1 8 ÷ 8 = 1 R0 1 ÷ 8 = 0 R1 → Octal: 101

**4. Octal → Decimal**
Method: Multiply each octal digit by 8^position and sum.

Example: 101 = 1×8² + 0×8¹ + 1×8⁰ = 64 + 0 + 1 = 65

**5. Decimal → Hexadecimal**
Method: Divide by 16 repeatedly, convert remainders >9 to A–F, reverse.

Example: 254 ÷ 16 = 15 R14 → F and E → Hex: FE

**6. Hexadecimal → Decimal**
Method: Convert each digit to decimal and multiply by 16^position.

Example: FE = F×16¹ + E×16⁰ = 15×16 + 14 = 240 + 14 = 254

**7. Binary → Octal**
Method: Group binary digits in 3s from right, convert each group to decimal.

Example: 110101 = 000 110 101 → 6 5 → Octal: 65

**8. Octal → Binary**
Method: Convert each octal digit to 3-bit binary.

Example: 65 → 6 = 110, 5 = 101 → Binary: 110101

**9. Binary → Hexadecimal**
Method: Group binary digits in 4s from right, convert to hex.

Example: 11111110 = 1111 1110 → F E → Hex: FE

**10. Hexadecimal → Binary**
Method: Convert each hex digit to 4-bit binary.

Example: FE → F = 1111, E = 1110 → Binary: 1111111

**11. Octal → Hexadecimal**
Method: Octal → Binary (3 bits), then Binary → Hex (4 bits).

Example: 65 (Octal) → 110101 (Binary) → 0001 1010 1 = 1A1 (Hex, pad as needed)

**12. Hexadecimal → Octal**
Method: Hex → Binary (4 bits), then Binary → Octal (3 bits).

Example: FE (Hex) → 1111 1110 → Group in 3s: 001 111 111 0 → pad: 000 111 111 010 → 3 7 2 → Octal: 372


# Task 2

# Basic Logic Gates

# AND Gate

An AND gate is a basic digital logic gate that outputs 1 (true) only when all its inputs are 1. Otherwise, it outputs 0 (false).

**Symbol:**

![image](https://github.com/user-attachments/assets/06b17f4e-446d-4716-8b54-1b54191bb661)

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

# OR Gate

An OR gate is a basic digital logic gate that implements logical disjunction. It gives a high (1) output if at least one of its inputs is high. In other words, the output is true when any input is true.

**Symbol**

![image](https://github.com/user-attachments/assets/154e49e1-55b0-44a7-8c85-048318c03223)

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

# NOT Gate

A NOT gate, also known as an inverter, is a basic digital logic gate that outputs the opposite (inverse) of its input. It has only one input and one output.

**Function:**

If the input is 1 (true or HIGH), the output is 0 (false or LOW).

If the input is 0, the output is 1.

**Symbol:**

![image](https://github.com/user-attachments/assets/2645779e-a694-4bf8-95c7-abf3cea3769f)

The NOT gate is usually represented by a triangle pointing to the right with a small circle (called a "bubble") at the output.

**Truth Table:**
|**Input (A)** |	**Output (¬A)**|
|--------------|------------------|
|0	|1|
|1	|0|

This table shows that the NOT gate simply flips the input value.








