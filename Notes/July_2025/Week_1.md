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
R_total = R_1 + R_2 + R_3 + . . .


> The total resistance is just the **sum of all resistors**.

### 🔸 Current:
- **I is the same everywhere** in a series connection.

### 🔸 Voltage:
- **Voltage divides** across resistors based on their values.
- If **one resistor fails**, **all fail** in a series.

---

## 🔀 Parallel Resistors (Branched Path)

- Resistors are connected **side by side**, like lanes on a highway.


### 🔸 Formula:
General case (for 3 or more resistors):
1 / R_total = 1 / R1 + 1 / R2 + 1 / R3 + ...

For exactly 2 resistors:
R_total = (R1 × R2) / (R1 + R2)


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
 Calculation:
R_total = R1 + R2
         = 10 + 20
         = 30 Ω
### Example 2 - Parallel
- R1 = 6 Ω
- R2 = 3 Ω
 Calculation:
1 / R_total = 1 / R1 + 1 / R2
            = 1/6 + 1/3
            = (1 + 2) / 6
            = 3 / 6

R_total = 6 / 3 = 2 Ω
---
# 📘 Topic 4: Capacitors

## ⚡What is a Capacitor?

A capacitor is a two-terminal electronic component that stores energy in the form of an electric field.

**🪣Think of it like:**  
A water bucket with a rubber sheet in the middle — one side you push electrons (–ve charge), and the other side loses electrons (+ve charge).  
The rubber sheet doesn’t let them meet but stores the tension between them.  
This tension is electrical energy. The more electrons you push, the stronger the electric field.

---

## 🛠️Construction

A basic capacitor is made of:
- Two metal plates (conductors)
- Separated by an insulator (called a dielectric) like air, ceramic, or plastic

> ⚠️ No current flows through the capacitor, but energy is stored between the plates.

---

## 🔄Working

When connected to a voltage source:
- Electrons are pushed onto one plate (–ve side)
- Electrons are pulled from the other plate (+ve side)
- The dielectric prevents direct flow → energy is stored as electric field

Once fully charged, the capacitor:
- Blocks DC current (acts like an open switch)
- Allows AC to pass depending on frequency

---

## 🧮Formulas

- Capacitance: `C = Q / V`  
- Energy Stored: `E = 1/2 * C * V²`  
- Reactance in AC: `Xc = 1 / (2 * π * f * C)`  
  → Higher frequency = Lower reactance

---

## 🧰Real-Life Use Cases

1. **🔋 Power Supply Smoothing** – Stores charge & releases it to keep voltage steady  
2. **⏱️ Timing Circuits (555 Timer)** – Charge/discharge of capacitors controls time intervals  
3. **⚙️ Motor Starters** – Help motors get initial torque by shifting phase in AC  
4. **📱 Touchscreens** – Your finger changes the capacitance of the surface  
5. **📸 Camera Flash** – Stores charge & releases it suddenly for a flash  
6. **📻 Filtering in Radios** – Blocks DC, allows AC  
7. **🚗 Energy Storage (Supercaps)** – Temporarily store energy. Faster than batteries (used in hybrid cars)

---

## ❓Questions

### 1. Does current flow through a capacitor?

During charging/discharging, current flows **into and out** of the terminals, but **not through** the dielectric.
Energy is released into the circuit without acting like a normal conductor.

### 2. Why does a capacitor block DC but allow AC?

DC is constant — once fully charged, it's like a full bucket → flow stops.  
AC keeps changing direction → capacitor keeps charging/discharging → allows current flow, especially at **high frequencies**.

### 3. If frequency increases, what happens?

Using: `Xc = 1 / (2πfC)`  
If `f ↑`, then `Xc ↓` → Easier for AC to pass through the capacitor

### 4. Will a capacitor explode if overcharged?

Yes. Overcharging (esp. electrolytic capacitors) can cause leaking, bursting, or explosion.

**Prevention:**
- Use resistors to control charging current
- Voltage regulators to limit voltage
- Zener diodes or crowbar circuits for protection

### 5. Why use a capacitor in a camera flash?

Batteries are slow (energy over time), but capacitors **instantly** release stored energy — needed for that bright flash in a split second.

---

# 📘 Topic 5: RC Time Constant

## ⏳What is RC Time Constant?

The RC time constant (symbol: `τ`, tau) tells how fast a capacitor charges or discharges in a circuit with a resistor and capacitor.

- `τ = R × C`

> **After 1τ**: Charges to ~63%  
> **After 2τ**: ~86%  
> **After 3τ**: ~95%  
> **After 5τ**: ~99%

So it takes about **5 time constants** to be fully charged.

---

## 🔌 Charging a Capacitor

| Time      | Charge Level |
|-----------|--------------|
| After 1τ  | ~63% charged |
| After 2τ  | ~86% charged |
| After 3τ  | ~95% charged |
| After 5τ  | ~99% charged |

---

## 🔋 Discharging a Capacitor

| Time      | Charge Left |
|-----------|-------------|
| After 1τ  | ~37% remains |
| After 2τ  | ~13% remains |
| After 3τ  | ~5% remains  |
| After 5τ  | ~1% remains  |

---

## 💡 Why Does It Matter?

Because it helps us create timing delays in circuits:

- Blinking LEDs  
- Camera timers  
- Tone generators  
- Sensor sampling delays  
- 555 Timer ICs  

