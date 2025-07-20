# Topic 1: Inductors

### 📘 **What is an Inductor?**

An **inductor** is a passive electronic component that **stores energy in a magnetic field** when electric current flows through it.

* It’s usually a **coil of wire** (copper), often wound around a core (air or magnetic material).
* **Symbol:** `L` (measured in **Henrys (H)**)

---

### ⚡️ **Basic Principle**

> **When current through an inductor changes, it resists the change by inducing a voltage (EMF) in the opposite direction.**

This is called **self-inductance**, and it's governed by **Lenz’s Law** and **Faraday’s Law**.

---

### **Lenz's Law** 🔁


> *The direction of the induced current is such that it opposes the change in magnetic flux that produced it.*

---

### 🧠 **What It Means:**

* If a magnetic field **increases**, the induced current will produce a field **opposing that increase**.  
* If the magnetic field **decreases**, the induced current will try to **maintain it** by producing a field in the same direction.

---
### **Faraday's Law of Electromagnetic Induction** ⚡

> *Whenever there is a change in magnetic flux linked with a circuit, an electromotive force (EMF) is induced. The magnitude of this EMF is directly proportional to the rate of change of the magnetic flux.*

---

### 🔧 **Inductor Formula**

The voltage across an inductor:

$$
V_L = L \frac{dI}{dt}
$$

* $V_L$: Induced voltage  
* $L$: Inductance (in Henry)  
* $\frac{dI}{dt}$: Rate of change of current

---

### 🧠 **Key Concepts to Remember**

| Concept            | Description                                 |
| ------------------ | ------------------------------------------- |
| **Inductance (L)** | Ability to oppose change in current         |
| **Energy Stored**  | $E = \frac{1}{2}LI^2$                       |
| **Ideal Inductor** | Has no resistance or capacitance            |
| **Real Inductor**  | Has some resistance (modeled as RL circuit) |

---

### 🔁 **Inductor Behavior in Circuits**

| Condition           | Inductor Behavior                                        |
| ------------------- | -------------------------------------------------------- |
| **DC steady state** | Acts like a **short circuit** (0V drop)                  |
| **AC or switching** | Opposes changes → **acts like a resistor + phase shift** |
| **Switching ON**    | Resists sudden current → builds gradually                |
| **Switching OFF**   | Can cause **voltage spike** (flyback)                    |

---

---

### 🔄 **RL Circuit Basics – What is Happening Here?**

#### 📈 CHARGING Equation:

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

#### 🧠 **What This Really Means**

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

#### 🧠 MEMORY TRICK:

* **"1 - e⁻ᵗ/τ" = Slowly rising curve**  
* It starts at 0 and rises like a water tank filling up.

---

####  💨 DISCHARGING Equation:

Now suppose you disconnect the battery and just leave the inductor + resistor.

$$
I(t) = I_{\text{max}} \cdot e^{-t/\tau}
$$

This time:

* Inductor tries to **keep current flowing** (like a spinning fan after turning off power)  
* But the resistor **dissipates energy** and current **falls gradually**

---

#### 🧠 FEEL THIS HAPPENING:

1. At $t = 0$:  
   Current is at its **maximum** (just before disconnecting)

2. As time goes on:

   * At $t = \tau$: current is **37%**  
   * At $t = 5\tau$: current is **almost zero**

---

---

#### 🔂 What is This “𝜏 = L / R” Time Constant?

It's like a **"speed controller"** for how fast the current builds or drops.

* **Higher L = more delay** (inductor is more stubborn)  
* **Higher R = faster process** (resistor pulls current down quicker)

You can remember:

> 🔁 Time Constant = L/R  
> → Larger L = lazy current  
> → Larger R = quick decay

---

## 🧠 One-Line Summary to Burn in Brain:

> ✅ **Charging**: $I(t) = I_{\text{max}}(1 - e^{-t/\tau})$ → slowly rises  
> ✅ **Discharging**: $I(t) = I_{\text{max}} e^{-t/\tau}$ → slowly falls  
> ✅ $\tau = \frac{L}{R}$ = how fast things happen

---


### 📊 **Frequency Response (AC)**

* Inductive Reactance:

$$
X_L = 2\pi f L
$$

Where:

* $X_L$: Inductive reactance  
* $f$: Frequency of the signal

As **frequency increases**, **inductive reactance increases** — so inductors **block high-frequency signals** and **allow low-frequency** (opposite of capacitors).

---

### ⚙️ **Applications of Inductors**

| Application                  | Role                               |
| ---------------------------- | ---------------------------------- |
| **Filters**                  | Remove AC from DC or vice versa    |
| **Transformers**             | Magnetic coupling between coils    |
| **Switching Power Supplies** | Energy storage and transfer        |
| **RF Circuits**              | Frequency tuning (with capacitors) |
| **Motors & Relays**          | Magnetic field generation          |

---


