# Currentmirror
### Aim:
Design and Analyze current mirror circuit as load active in amplifier circuit with Av>-10v/v, P<=1mW, Vdd=1.8V.
### Theory:
A **current mirror** is a circuit used to copy  a reference current from one branch to another while maintaining a constant current. It typically consists of two or more transistors, where one sets the reference current, and the others replicate it. Current mirrors are widely used in analog circuits, such as biasing and amplifier stages, to ensure stable and predictable current flow.

###Working Principle:
A current mirror typically consists of two identical transistors (BJTs or MOSFETs).

The first transistor (reference transistor) is biased to set a fixed reference current.

The second transistor (output transistor) copies (mirrors) this current due to identical electrical characteristics.

The mirrored current remains stable even if the supply voltage or load changes.
A **current mirror** is an electrical circuit that copies (or "mirrors") a current from one active device to another while maintaining a constant current. It is widely used in analog circuits, such as biasing transistors and current sources in integrated circuits. Below are its **advantages and disadvantages**:

### **Advantages of Current Mirror:**
1. **Current Stability** – Provides a stable and precise output current that is independent of variations in supply voltage or temperature.
2. **High Output Resistance** – Acts as an ideal current source with a high output impedance, making it useful for biasing transistors.
3. **Low Power Consumption** – Operates efficiently with minimal power loss, particularly in MOSFET implementations.
4. **Circuit Simplicity** – Requires only a few transistors, making it easy to implement in integrated circuits.

### **Disadvantages of Current Mirror:**
1. **Limited Compliance Voltage** – The output current remains constant only within a certain voltage range (compliance range); beyond this, performance degrades.
2. **Limited Frequency Response** – At high frequencies, parasitic capacitances can affect performance.
3. **Voltage Drop Across Transistors** – Requires a minimum voltage drop (V_BE for BJTs or V_GS for MOSFETs), which may affect low-voltage applications.

# Components: 
Mosfet Resistor, voltage supply and connecting wires.

# Procedure:
1.Design the current mirror circuit (using BJTs or MOSFETs).

2.Define component values, supply voltage, and input current.

3.Run DC analysis , AC analysis, and transient analysis.

4.Observe output current stability and voltage compliance range.

# Circuit 1
![Screenshot 2025-03-24 194635](https://github.com/user-attachments/assets/a5134ea7-e6d8-4adc-ab1d-dd2ef6e1c44b)
 #case 1:
 PMOSFET = length is 180nm, width is 10um
NMOSFET = length is 180nm, width is 120.25um
#DC analysis:
![Screenshot 2025-03-24 212129](https://github.com/user-attachments/assets/bc360a68-d5dc-452f-857b-ca9cbac37ddd)
Vout= 1.299v
Vx= 1.178v
Iref = 0.277mA
# Case 2: 500nm
PMOSFET = length is 500nm, width is 10um
NMOSFET = length is 500nm, width is 207.617um
Vout= 1.299v
Vx= 1.178V
Iref = 0.277mA
![Screenshot 2025-03-24 213128](https://github.com/user-attachments/assets/37680f29-95e0-42b2-81e8-5e6ec17ebdf1)
# Case 3: 1umm PMOSFET = length is 1um, width is 10um
NMOSFET = length is 1um, width is 250.5um
Vout= 1.299V
Vx= 1.178V
Iref = 0.277mA
![Screenshot 2025-03-24 213844](https://github.com/user-attachments/assets/ec78c3e3-1304-475c-a8b9-da0853400f69)



