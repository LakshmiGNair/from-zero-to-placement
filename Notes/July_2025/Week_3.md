# 🧪 Topic 1 : Practical Simulation of Ohm’s Law using Tinkercad

---

## 🔩 Components Needed
- 🔋 Battery  
- 🔘 Resistor  
- 💡 LED  
- 📟 Multimeter  
- 🧵 Wires  

---

## 🔌 Connections
- Connect **-ve side of battery** to **cathode of LED**.  
- Connect **anode of LED** to **one side of resistor**.  
- Connect **the other side of the resistor** to the **+ve terminal of battery**.

---

## 🔍 To Measure Current
- Break the wire between **+ve terminal of battery** and the **resistor**.  
- Keep the **multimeter in series**.  
- Connect **red terminal** of the multimeter to the **+ve terminal of the battery** and the **black terminal** of the multimeter to the **resistor**.

---

## ⚡ To Measure Voltage
- Keep the **multimeter in parallel** to the resistor.  
- Connect **black terminal** of multimeter to the **-ve side of the resistor**.  
- Connect **red terminal** of multimeter to the **+ve side of the resistor**.  
- Otherwise, we will get **-ve voltage**.

Now measure both and check according to **Ohm’s Law**:  
> **V = I × R**

---

## 🧾 1st Observation
- **R** = 220 Ω  
- **I** = 30.9 mA  
- **V** = 6.79 V  
 - I × R = 6.79
#### So, V = IR

---

## 🧾 2nd Observation
- **R** = 560 Ω  
- **V** = 6.97 V  
- **I** = 12.4 mA  
- I × R = 6.94 V



---

## 📌 Observations
- ➕ As **resistance increases**, **current decreases**.  
- 🔋 **Voltage stays the same** if the battery is constant.  
- 💡 **LED brightness** also varies with current – **dimmer with more resistance**.

---
# 🔋 Topic 2 – Build Voltage Divider in Tinkercad

---

## 🧰 Components Required
- 2️⃣ Resistors  
- 🧱 Breadboard  
- 📟 Multimeter  
- 🔋 Battery  

---

## 🔌 Connections
- Connect **negative terminal** of battery to **ground** (black rail → -ve rail) and **positive terminal** of battery to **positive rail**.
- Connect **one resistor’s end** to the **positive rail** and the **other end** of that resistor to the **2nd resistor**.
- Connect the **other end of the 2nd resistor** to the **negative rail**.

---

## 📏 Measuring Voltage
- Connect the **black terminal** of the multimeter to the **negative rail**.
- Connect the **red terminal** of the multimeter to the **point between the two resistors**.

---

## 📊 Expected Output (For Equal Resistors)
```
Vout = Vin × (R2 / (R1 + R2))


Where:
- **Vin**: Input voltage
- **R1**: Resistor connected to Vin
- **R2**: Resistor connected to Ground
- **Vout**: Output voltage (at the junction of R1 and R2)


Let’s say:

- `Vin = 9V`
- `R1 = 1kΩ`
- `R2 = 1kΩ`

Vout = 9V × (1kΩ / (1kΩ + 1kΩ))
= 9V × (1 / 2)
= 4.5V

```
---

## 📚 Logic

- The goal of the experiment is to **split or divide** an input voltage into a **lower output voltage** using two resistors.
- When two resistors are connected in series, the **total input voltage** is divided between them **proportionally to their resistances**.
- The voltage at the point between the two resistors is given by:
```
Vout = Vin × (R2 / (R1 + R2))
```
---









