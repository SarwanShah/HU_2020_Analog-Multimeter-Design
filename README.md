# Analog Multimeter Project  

## **📌 Project Overview**  
This project was developed under the **EE-365 Industrial Instrumentation and Measurements** course at **Habib University** during Spring 2020. The objective was to design and build an **analog multimeter** using a **d'Arsonval Galvanometer**, integrating three key measurement modes: **voltmeter**, **ammeter**, and **ohmmeter**. The project explores the challenges of analog instrumentation, including **calibration, component selection, and design integration**.  

**REPORT: https://github.com/SarwanShah/HU_2020_Analog-Multimeter-Design/blob/main/Final_Report.pdf** 

---

## **🛠 Project Features**  
- **Voltmeter:** Measures voltages in the range of **0 to 50V**.
- **Ammeter:** Measures currents in the range of **0 to 100mA**.
- **Ohmmeter:** Measures resistances from **1 to 100Ω**, with provisions for **10% battery variation**.
- **Integrated Design:** Combines all three instruments into one device with selectable modes.
- **Simulation & Hardware Validation:** Includes circuit simulations and hardware implementation using veroboard.

---

## **🏗 Project Implementation**  
### ➤ **Galvanometer Calibration**  
- **Internal Resistance (Rm):** Measured as **218.4Ω**.
- **Full-Scale Deflection Current (IFSD):** Determined to be **4.195mA** through gradual voltage application.

### ➤ **Ammeter Design**  
- **Shunt-Type Design:** Utilizes a parallel shunt resistor to limit the current through the galvanometer.
- **Shunt Resistance (Rsh):** Calculated to be **9.56Ω** with a practical combination of **10Ω || 220Ω**.

### ➤ **Voltmeter Design**  
- **Series-Type Design:** Employs a series resistor to divide the input voltage.
- **Multiplier Resistance (Rse):** Designed at **11.7kΩ**, with a practical combination of **680kΩ || 12kΩ**.

### ➤ **Ohmmeter Design**  
- **Series-Type Design:** Uses a **9V battery**, a fixed resistor for current limiting, and a variable resistor for zero-control.
- **Resistor Network:** Includes **1734Ω**, **192.7Ω**, and **2.2kΩ || 8.2kΩ** resistors to handle various ranges.

---

## **🖥 Simulation Results**  
### ➤ **Ammeter Simulation**  
- Linear relationship observed between input current (0–100mA) and galvanometer deflection current (up to **4.195mA**).

### ➤ **Voltmeter Simulation**  
- Linear increase in galvanometer deflection current as input voltage varies from **0 to 50V**.

### ➤ **Ohmmeter Simulation**  
- Inverse proportional relationship between input resistance (1–100kΩ) and galvanometer deflection current.

---

## **🔧 Hardware Implementation**  
- The circuit was implemented on a **veroboard**, requiring extensive soldering and optimization to minimize interference.
- A **manual jumper setup** was used to switch between modes instead of slide switches, reducing the risk of simultaneous mode activation.
- Additional resistors
