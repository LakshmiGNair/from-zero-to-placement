# Topic 1: Voltage, Current, Resistance & Ohm’s Law

---

## 🔋 Voltage (V)
- Voltage is the potential difference between two points.
- It’s what pushes electrons to move.
- Voltage is the reason electrons want to move.
- **No voltage = no push = no flow**

---

## 🔌 Current (I)
- Current is the flow of electrons.
- It’s measured in **amperes (A)**.
- Current is like the number of electrons moving past a point per second.

---

## 🔧 Resistance (R)
- Resistance is what **opposes the flow of current**.
- Measured in **ohms (Ω)**.
- **Copper** → low resistance  
- **Rubber** → high resistance  
- Resistance slows down current.

---

## 📏 Ohm’s Law
V = I × R

Derived formulas:
I = V / R

R = V / I

---

# Topic 2: Power and Energy in Circuits

## 🔌 Power (P)

- Power is the **rate at which energy is used or transferred**.  
- It tells you **how fast work is being done** in a circuit.

### 🔹 Formulas:
- `P = V × I`  
- `P = I² × R`  
- `P = V² / R`

### 🔹 Unit:
- **Watt (W)**
- `1 Watt = 1 Joule per second`

---

## 🔋 Energy (E)

- Energy is the **total amount of work done** or **power used over time**.

### 🔹 Formulas:
- `E = P × t`  
- `E = V × I × t`  
- `E = I² × R × t`  
- `E = (V² / R) × t`

### 🔹 Units:
- **Joule (J)**
- **Watt-hour (Wh)** or **Kilowatt-hour (kWh)**  
  `1 kWh = 1000 Wh`

---

## ⚡ Key Ideas

- **Power** is like the **speed** at which your device uses energy.
- **Energy** is the **total fuel consumed**.

---

## 💡 Example

**For an LED bulb:**  
- Power = `10 W`  
- Time used = `5 hours`  
- Energy used = `10 × 5 = 50 Wh`

---

## 🔥 Power in Resistors

When current flows through a resistor (like a fan or light):

- It **produces heat**
- That **heat is energy** being used

### Formula:
- `P = I² × R`

---

# 📘 Topic 3: Series and Parallel Resistors

---

## 🔌 What is a Resistor?

- A **resistor resists** the flow of current.  
- It's like **putting a speed breaker** in a road.

**Symbol:** `—/\/\/—`  
**Unit:** Ohm (Ω)

---

## 🧵 Series Resistors (Linear Path)

- If you place resistors one after the other, it's called a **series connection**.

R1 ─── R2 ─── R3


### 🔸 Formula:
\[
R_{\text{total}} = R_1 + R_2 + R_3 + \ldots
\]

> The total resistance is just the **sum of all resistors**.

### 🔸 Current:
- **I is the same everywhere** in a series connection.

### 🔸 Voltage:
- **Voltage divides** across resistors based on their values.
- If **one resistor fails**, **all fail** in a series.

---

## 🔀 Parallel Resistors (Branched Path)

- Resistors are connected **side by side**, like lanes on a highway.

 ┌── R1 ──┐
 ├── R2 ──┤
 └── R3 ──┘

### 🔸 Formula:
\[
\frac{1}{R_{\text{total}}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3} + \ldots
\]

For only 2 resistors:
\[
R_{\text{total}} = \frac{R_1 \times R_2}{R_1 + R_2}
\]

### 🔸 Voltage:
- **Voltage is the same** across all branches.

### 🔸 Current:
- **Current splits** across branches.
- **More current flows** where resistance is less.
- If **one resistor fails**, **rest still work**.

---

## 🧪 Practical Examples

### Example 1 — Series:
- R₁ = 10 Ω  
- R₂ = 20 Ω  
\[
R_{\text{total}} = 10 + 20 = \boxed{30\ \Omega}
\]

### Example 2 — Parallel:
- R₁ = 6 Ω  
- R₂ = 3 Ω  
\[
\frac{1}{R_{\text{total}}} = \frac{1}{6} + \frac{1}{3} = \frac{3}{6} \Rightarrow R_{\text{total}} = \boxed{2\ \Omega}
\]

---


