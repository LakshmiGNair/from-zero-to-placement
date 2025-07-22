# Topic 1: Inductors

## 📘 **What is an Inductor?**

An **inductor** is a passive electronic component that **stores energy in a magnetic field** when electric current flows through it.

* It’s usually a **coil of wire** (copper), often wound around a core (air or magnetic material).
* **Symbol:** `L` (measured in **Henrys (H)**)

---

## ⚡️ **Basic Principle**

> **When current through an inductor changes, it resists the change by inducing a voltage (EMF) in the opposite direction.**

This is called **self-inductance**, and it's governed by **Lenz’s Law** and **Faraday’s Law**.

---

## **Lenz's Law** 🔁


> *The direction of the induced current is such that it opposes the change in magnetic flux that produced it.*

---

### 🧠 **What It Means:**

* If a magnetic field **increases**, the induced current will produce a field **opposing that increase**.  
* If the magnetic field **decreases**, the induced current will try to **maintain it** by producing a field in the same direction.

---
## **Faraday's Law of Electromagnetic Induction** ⚡

> *Whenever there is a change in magnetic flux linked with a circuit, an electromotive force (EMF) is induced. The magnitude of this EMF is directly proportional to the rate of change of the magnetic flux.*

---

## 🔧 **Inductor Formula**

The voltage across an inductor:

$$
V_L = L \frac{dI}{dt}
$$

* $V_L$: Induced voltage  
* $L$: Inductance (in Henry)  
* $\frac{dI}{dt}$: Rate of change of current

---

## 🧠 **Key Concepts to Remember**

| Concept            | Description                                 |
| ------------------ | ------------------------------------------- |
| **Inductance (L)** | Ability to oppose change in current         |
| **Energy Stored**  | $E = \frac{1}{2}LI^2$                       |
| **Ideal Inductor** | Has no resistance or capacitance            |
| **Real Inductor**  | Has some resistance (modeled as RL circuit) |

---

## 🔁 **Inductor Behavior in Circuits**

| Condition           | Inductor Behavior                                        |
| ------------------- | -------------------------------------------------------- |
| **DC steady state** | Acts like a **short circuit** (0V drop)                  |
| **AC or switching** | Opposes changes → **acts like a resistor + phase shift** |
| **Switching ON**    | Resists sudden current → builds gradually                |
| **Switching OFF**   | Can cause **voltage spike** (flyback)                    |

---

---

## 🔄 **RL Circuit Basics – What is Happening Here?**

## 📈 CHARGING Equation:

When you suddenly apply voltage (step input):

$$
I(t) = I_{\text{max}} \left(1 - e^{-t/\tau}\right)
$$

Where:

* $I(t)$ = current at time $t$  
* $I_{\text{max}} = \frac{V}{R}$ (Ohm's law final value)  
* $\tau = \frac{L}{R}$ (called the **time constant**)  
* $e$ is Euler's number ≈ 2.718  

---

### 🧠 **What This Really Means**

Let’s break this down like a story:

1. At $t = 0$:

   $$
   I(0) = I_{\text{max}}(1 - e^0) = I_{\text{max}}(1 - 1) = 0
   $$

   ➤ **No current flows instantly** (inductor blocks it at first).

2. As time increases:  
   The exponential term $e^{-t/\tau}$ becomes smaller and smaller:

   * At $t = \tau$: $I \approx 63\%$ of max value  
   * At $t = 5\tau$: $I \approx 99.3\%$ → **almost full current**

3. After a long time:

   $$
   e^{-t/\tau} \rightarrow 0 \quad \Rightarrow \quad I(t) \rightarrow I_{\text{max}}
   $$

   ➤ Now the inductor behaves like a **wire**, and full current flows.

---

### 🧠 MEMORY TRICK:

* **"1 - e⁻ᵗ/τ" = Slowly rising curve**  
* It starts at 0 and rises like a water tank filling up.

---

##  💨 DISCHARGING Equation:

Now suppose you disconnect the battery and just leave the inductor + resistor.

$$
I(t) = I_{\text{max}} \cdot e^{-t/\tau}
$$

This time:

* Inductor tries to **keep current flowing** (like a spinning fan after turning off power)  
* But the resistor **dissipates energy** and current **falls gradually**

---

### 🧠 FEEL THIS HAPPENING:

1. At $t = 0$:  
   Current is at its **maximum** (just before disconnecting)

2. As time goes on:

   * At $t = \tau$: current is **37%**  
   * At $t = 5\tau$: current is **almost zero**

---

---

### 🔂 What is This “𝜏 = L / R” Time Constant?

It's like a **"speed controller"** for how fast the current builds or drops.

* **Higher L = more delay** (inductor is more stubborn)  
* **Higher R = faster process** (resistor pulls current down quicker)

You can remember:

> 🔁 Time Constant = L/R  
> → Larger L = lazy current  
> → Larger R = quick decay

---

### 🧠 One-Line Summary to Burn in Brain:

> ✅ **Charging**: $I(t) = I_{\text{max}}(1 - e^{-t/\tau})$ → slowly rises  
> ✅ **Discharging**: $I(t) = I_{\text{max}} e^{-t/\tau}$ → slowly falls  
> ✅ $\tau = \frac{L}{R}$ = how fast things happen

---


## 📊 **Frequency Response (AC)**

* Inductive Reactance:

$$
X_L = 2\pi f L
$$

Where:

* $X_L$: Inductive reactance  
* $f$: Frequency of the signal

As **frequency increases**, **inductive reactance increases** — so inductors **block high-frequency signals** and **allow low-frequency** (opposite of capacitors).

---

## ⚙️ **Applications of Inductors**

| Application                  | Role                               |
| ---------------------------- | ---------------------------------- |
| **Filters**                  | Remove AC from DC or vice versa    |
| **Transformers**             | Magnetic coupling between coils    |
| **Switching Power Supplies** | Energy storage and transfer        |
| **RF Circuits**              | Frequency tuning (with capacitors) |
| **Motors & Relays**          | Magnetic field generation          |

---

# Topic 2: DIODES

---

## 🔹 1. What is a Diode?

A **diode** is a two-terminal **semiconductor device** that allows **current to flow in only one direction**.

* **Terminals**:
  * **Anode (A)** – Positive side
  * **Cathode (K)** – Negative side

---

## 🔹 2. How a Diode Works (Basic Principle)

A **PN junction** forms the core of a diode:

* **P-type material** has **holes (positive charge carriers)**
* **N-type material** has **electrons (negative charge carriers)**

### 🔄 Biasing Conditions

| Bias Type        | Connection         | Result                 |
| ---------------- | ------------------ | ---------------------- |
| **Forward Bias** | Anode +, Cathode - | Diode conducts current |
| **Reverse Bias** | Anode -, Cathode + | Diode blocks current   |

When forward-biased and voltage exceeds the **threshold (≈0.7V for silicon)**, it conducts.

---

## 🔹 3. V-I Characteristics of a Diode

| Region           | Description                                         |
| ---------------- | --------------------------------------------------- |
| Forward region   | Current rises exponentially after threshold voltage |
| Reverse region   | Very little leakage current flows                   |
| Breakdown region | In Zener diodes, reverse voltage causes conduction  |

---

## 🔹 4. Types of Diodes & Their Uses

| Type                           | Description                                     | Applications                   |
| ------------------------------ | ----------------------------------------------- | ------------------------------ |
| **PN Junction Diode**          | Basic diode for rectification                   | AC to DC converters            |
| **Zener Diode**                | Allows reverse current after breakdown voltage  | Voltage regulation             |
| **Schottky Diode**             | Low forward voltage drop, fast switching        | High-speed circuits, SMPS      |
| **Light Emitting Diode (LED)** | Emits light when forward biased                 | Indicators, displays           |
| **Photodiode**                 | Generates current when exposed to light         | Light sensors, solar cells     |
| **Tunnel Diode**               | Exhibits negative resistance region             | Microwave oscillators          |
| **Varactor Diode**             | Acts as a variable capacitor under reverse bias | Frequency tuning in radios     |
| **Laser Diode**                | Emits coherent light (laser)                    | CD/DVD players, fiber optics   |
| **PIN Diode**                  | Used for RF switching, high frequency circuits  | RF attenuators, photodetectors |

---

## 🔹 5. Diode Circuits and Applications

### 📦 5.1. Rectifiers (AC to DC Conversion)

* **Half-Wave Rectifier** – Uses 1 diode, passes half AC cycle.
* **Full-Wave Rectifier** – Uses 2 or 4 diodes (bridge), passes both halves.
* **Bridge Rectifier** – 4 diodes arranged in a bridge, full-wave output.

### 💡 5.2. Clipping Circuits

* Diodes limit the voltage to a desired level.
* Used for signal protection and shaping.

### 📉 5.3. Clamping Circuits

* Shift the voltage level of a signal.
* Used in oscilloscopes and waveform processing.

### 🔁 5.4. Voltage Regulation

* **Zener diodes** maintain a constant voltage across a load.
* Used in power supplies.

### 📡 5.5. Switching and Logic Gates

* Diodes used in **digital logic gates** (AND, OR).
* Fast diodes (like Schottky) used in **high-speed switching**.

---





