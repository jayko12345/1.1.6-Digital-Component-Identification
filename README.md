# 1.1.6 Digital Component Identification

## Overview

In this activity, you will investigate combinational and sequential logic devices using Circuit Design Software (CDS).

You will build and simulate circuits using fundamental logic gates, generate truth tables from observed outputs, and identify the behavior of each gate. You will also investigate a D flip-flop and use a 555 timer circuit to create a repeating clock signal.

## Learning Objectives

By the end of this activity, you should be able to:

- Investigate combinational and sequential logic gates.
- Simulate simple circuits using basic logic gates.
- Generate truth tables from simulated circuit outputs.
- Analyze truth tables to determine logic-gate functions.
- Describe the basic operation of a D flip-flop.
- Explain how a 555 timer can be used to generate a clock signal.

## Materials

- Computer with Circuit Design Software (CDS)
- Component Identification: Digital presentation
- Activity 1.1.6 Digital Component Identification resource

## Vocabulary

| Term | Description |
|---|---|
| Combinational logic | Logic in which the output depends only on the present inputs |
| Sequential logic | Logic in which the output depends on present inputs and previous circuit states |
| Logic gate | An electronic device that performs a Boolean operation on one or more inputs |
| Truth table | A table showing the output for every possible input combination |
| Toggle | To change a switch from one state to another |
| Flip-flop | A sequential logic device that stores one bit of information |
| Clock signal | A repeating signal used to control the timing of sequential circuits |
| Active low | An input that is activated when its logic level is `0` or LOW |

## Logic-Level Conventions

Use the following conventions throughout this activity:

| Circuit State | Logic Value |
|---|---:|
| Switch connected to GND | `0` |
| Switch connected to +5 V | `1` |
| Output probe off | `0` |
| Output probe on | `1` |

For a truth table with \(N\) inputs, there are \(2^N\) possible input combinations.

For example, a circuit with two inputs has:

$$
2^2 = 4
$$

possible input combinations.

---

# Part A: Combinational Logic

Combinational logic circuits produce an output based only on the current input values. When an input changes, the output changes immediately according to the Boolean function of the logic gate.

Before beginning, review the **Component Identification: Digital Worksheet** presentation.

## 1. Inverter Gate

Create the circuit shown in the figure using:

- A switch to provide input `X`
- A probe to indicate output `Z`

<img width="531" height="168" alt="chrome_KPBysZJ36i" src="https://github.com/user-attachments/assets/08fd4fb8-1e81-4011-bdb9-d989a343080f" />

<!-- IMAGE: Figure 1 — Inverter gate circuit with input X, output Z, switch, and probe -->

Toggle the input switch and observe output `Z`.

### Truth Table: Inverter

| X | Z |
|---:|---:|
| 0 | 0
| 1 | 0 |

### Reflection

**From your truth table, why do you think this gate is called an inverter?**

because it switches on and off

---

## 2. AND Gate

Create the circuit shown in the figure using:

- A switch to provide input `X`
- A switch to provide input `Y`
- A probe to indicate output `Z`

<img width="541" height="259" alt="chrome_QDsHxNeTIs" src="https://github.com/user-attachments/assets/53486f6c-1302-4079-88f0-220c5fc67f4f" />


<!-- IMAGE: Figure 2 — AND gate circuit with inputs X and Y and output Z -->

Toggle the input switches and observe output `Z` for every input combination.

### Truth Table: AND

| X | Y | Z |
|---:|---:|---:|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

### Reflection

**From your truth table, why do you think this gate is called an AND gate?**

because if x AND y are 1 that means it'll be 1 aka on

---

## 3. NAND Gate

Create the circuit shown in the figure using:

- A switch to provide input `X`
- A switch to provide input `Y`
- A probe to indicate output `Z`

<img width="663" height="301" alt="chrome_QRcWRb1675" src="https://github.com/user-attachments/assets/a6390999-3a1e-441b-9320-97532076178b" />


<!-- IMAGE: Figure 3 — NAND gate circuit with inputs X and Y and output Z -->

Toggle the input switches and observe output `Z` for every input combination.

### Truth Table: NAND

| X | Y | Z |
|---:|---:|---:|
| 0 | 0 | 1 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

### Reflection

**From your truth table, why do you think this gate is called a NAND gate?**



---

# Part B: Additional Combinational Logic

## 4. OR Gate

Create the circuit shown in the figure using:

- A switch to provide input `X`
- A switch to provide input `Y`
- A probe to indicate output `Z`

<img width="636" height="299" alt="chrome_ySZphETZZp" src="https://github.com/user-attachments/assets/8904c480-ca64-4ed5-b410-3acaa3bbe05f" />


<!-- IMAGE: Figure 4 — OR gate circuit with inputs X and Y and output Z -->

Toggle the input switches and observe output `Z` for every input combination.

### Truth Table: OR

| X | Y | Z |
|---:|---:|---:|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1  |
| 1 | 1 | 1  |

### Reflection

**From your truth table, why do you think this gate is called an OR gate?**



---

## 5. NOR Gate

Create the circuit shown in the figure using:

- A switch to provide input `X`
- A switch to provide input `Y`
- A probe to indicate output `Z`

<img width="650" height="303" alt="chrome_Lk9KiQmtHB" src="https://github.com/user-attachments/assets/a8fa7fbb-872b-4392-b9e7-acd4a5f9c251" />


<!-- IMAGE: Figure 5 — NOR gate circuit with inputs X and Y and output Z -->

Toggle the input switches and observe output `Z` for every input combination.

### Truth Table: NOR

| X | Y | Z |
|---:|---:|---:|
| 0 | 0 | 1 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 0 |

### Reflection

**From your truth table, why do you think this gate is called a NOR gate?**



---

## 6. XOR Gate

Create the circuit shown in the figure using:

- A switch to provide input `X`
- A switch to provide input `Y`
- A probe to indicate output `Z`

<img width="651" height="303" alt="chrome_8PDSqdhUqc" src="https://github.com/user-attachments/assets/533d77d4-3113-4b27-833f-b63d93981d8a" />


<!-- IMAGE: Figure 6 — XOR gate circuit with inputs X and Y and output Z -->

Toggle the input switches and observe output `Z` for every input combination.

### Truth Table: XOR

| X | Y | Z |
|---:|---:|---:|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

### Reflection

**From your truth table, why do you think this gate is called an XOR gate, or exclusive OR gate?**

because it only works when it's either 1 and 0 or 0 and 1 

## Truth-Table Pattern

Truth-table inputs are conventionally listed in ascending binary-count order.

For two inputs, `X` and `Y`, list the input values as follows:

| Decimal Value | Binary Value | X | Y |
|---:|---:|---:|---:|
| 0 | `00` | 0 | 0 |
| 1 | `01` | 0 | 1 |
| 2 | `10` | 1 | 0 |
| 3 | `11` | 1 | 1 |

Most work in this course will use two-input gates. Gates with more than two inputs are also available.

---

# Part C: Flip-Flops

A combinational logic circuit immediately produces an output whenever an input changes. The new output replaces the old output.

A sequential logic circuit can remember a previous output state. Its output depends on both the current inputs and the sequence of previous inputs. This ability to retain a state makes sequential logic useful for memory and timing applications.

## D Flip-Flop Basics

A D flip-flop has:

- A data input, `D`
- A clock input, `CLK`
- An output, `Q`
- A complementary output, `NOT_Q` or `\overline{Q}`

The clock signal repeatedly changes between LOW (`0`) and HIGH (`1`). A clock transition tells the flip-flop when to process the data input.

The outputs `Q` and `NOT_Q` are complements of one another:

$$
NOT\_Q = \overline{Q}
$$

When `Q` is `1`, `NOT_Q` is `0`. When `Q` is `0`, `NOT_Q` is `1`.

<img width="349" height="360" alt="chrome_8Xo2sQ2pon" src="https://github.com/user-attachments/assets/88a5362e-2e39-4b90-8837-4fa93aa01b55" />


<!-- IMAGE: Figure 7 — D flip-flop symbol and equivalent NAND-gate representation -->

The simplified flip-flop symbol hides additional inputs:

- `PR` or preset
- `CLR` or clear

These inputs are not synchronized to the clock signal. They can force the flip-flop into a preset state or a cleared state.

---

# Part D: Sequential Logic Investigation

## 7. Investigate the 74LS74N Flip-Flop

Using Circuit Design Software, construct the `74LS74N` test circuit shown in the figure.

Use:

- A switch for input `T`
- A probe for input `CLK`
- A probe for input `D`
- A probe for output `Q`
- A probe for output `NOT_Q`

<img width="637" height="391" alt="chrome_nQE2kWcIN8" src="https://github.com/user-attachments/assets/f3e6a5ff-6339-4c8f-a22b-0c4c0ac34b08" />


### Circuit Notes

The `74LS74N` includes:

- A data input (`D`)
- A clock input (`CLK`)
- A preset input (`PR`)
- A clear input (`CLR`)
- An output (`Q`)
- A complementary output (`NOT_Q`)

In this test circuit:

- The switch `T` provides the clock input.
- The data input is connected to `NOT_Q`.
- `PR` and `CLR` are connected to +5 V.
- `PR` and `CLR` are active-low inputs, so they are inactive when connected to +5 V.

## Procedure

1. Toggle switch `T` several times until `T` is LOW and `NOT_Q` is LOW.
2. Start with the switch connected to GND.
3. Move the switch from GND to VCC (+5 V).
4. Observe and record the output at `Q`.
5. Move the switch from VCC (+5 V) back to GND.
6. Observe and record the output at `Q`.
7. Toggle the switch one additional time.
8. Observe and record the output at `Q`.

### Observations

| Switch Action | T State | Q Output | NOT_Q Output | Observation |
|---|---:|---:|---:|---|
| Starting condition | 0 | ___ | 0 | ___ |
| Move switch from GND to VCC | 1 | ___ | ___ | ___ |
| Move switch from VCC to GND | 0 | ___ | ___ | ___ |
| Toggle switch one more time | ___ | ___ | ___ | ___ |

### Analysis Questions

**What happens to output `Q` when switch `T` moves from GND to VCC?**

> _Write your answer here._

**What happens to output `Q` when switch `T` moves from VCC to GND?**

> _Write your answer here._

**What does your observation tell you about when `Q` changes relative to changes at the `CLK` input?**

> _Write your answer here._

**What is the relationship between `Q` and `NOT_Q`?**

> _Write your answer here._

**What is the relationship between data input `D` and output `Q`?**

> _Write your answer here._

**Based on your observations, explain the relationship among `D`, `Q`, `NOT_Q`, and `CLK`. What does a flip-flop do?**

> _Write your answer here._

### Reflection

**In this investigation, you changed the flip-flop state by manually toggling a switch. How could a flip-flop change states without direct human input?**

> _Write your answer here._

---

# Part E: Clock Signals and the 555 Timer

A clock signal can automate changes in a sequential circuit. In this section, you will investigate the LM555CN timer configured as an oscillator.

The 555 timer oscillator is a common introductory electronics circuit. Later, you will use this type of circuit to generate a clock signal for a random number generator.

## 8. Build 555 Timer Test Circuits

Using Circuit Design Software, create the three LM555CN test circuits shown in the figures on the same simulation sheet.

The only component value that changes among the three circuits is capacitor `C2`.

<img width="275" height="360" alt="555A" src="https://github.com/user-attachments/assets/431a5dab-df30-405b-8d31-a884a2cf0193" />

<!-- IMAGE: Figure 9 — LM555CN Circuit A -->

<img width="275" height="360" alt="555B" src="https://github.com/user-attachments/assets/ffe64220-cf6f-4387-ae17-9eca9983b3e1" />

<!-- IMAGE: Figure 10 — LM555CN Circuit B -->

<img width="275" height="360" alt="555C" src="https://github.com/user-attachments/assets/793057d8-2b11-4dc9-be5d-a67b372b0cdf" />

<!-- IMAGE: Figure 11 — LM555CN Circuit C -->

Observe the output behavior of each circuit.

### Observations

| Circuit | Relative C2 Value | Output Behavior | Estimated Frequency or Period |
|---|---|---|---|
| Circuit A | Original value | ___ | ___ |
| Circuit B | C2 halved | ___ | ___ |
| Circuit C | C2 doubled | ___ | ___ |

### Analysis Questions

**What happens to the clock signal when capacitor `C2` is halved?**

> _Write your answer here._

**What happens to the clock signal when capacitor `C2` is doubled?**

> _Write your answer here._

**Based on your observations, how does capacitor value affect the timing of a 555 timer oscillator?**

> _Write your answer here._

---

# Conclusion

## 9. Combine the 555 Timer and Flip-Flop

Create or modify a simulation that connects the 555 timer clock signal to the flip-flop clock input.

Your goal is to make the flip-flop change state automatically at a rate you select.

### Design Challenge

**Can you combine the 555 timer circuit with the flip-flop circuit so that the flip-flop changes state automatically at a rate you choose?**

- Build the combined simulation.
- Adjust the timer circuit to change the flip-flop’s switching rate.
- Verify that the flip-flop changes state automatically.
- Share your completed simulation with your instructor.

> **Image Placeholder:** Insert a screenshot of your completed 555-timer-and-flip-flop simulation.

<!-- IMAGE: Completed 555 timer connected to flip-flop clock input -->

## Final Reflection

**How do combinational logic, sequential logic, flip-flops, and clock signals work together in a digital system?**

> _Write your answer here._

---

# Sources

- Original activity resource: *Activity 1.1.6 Digital Component Identification*
- Third-party historical highlight image source:
  - Square Reader and iPhone 3G, Chris Harrison, Wikimedia Commons, CC BY 2.0
