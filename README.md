# Currentmirror
### Aim:
Design and Analyze current mirror circuit as load active in amplifier circuit with Av>-10v/v, P<=1mW, Vdd=1.8V.
### Theory:
A **current mirror** is a circuit used to copy  a reference current from one branch to another while maintaining a constant current. It typically consists of two or more transistors, where one sets the reference current, and the others replicate it. Current mirrors are widely used in analog circuits, such as biasing and amplifier stages, to ensure stable and predictable current flow.
![Screenshot 2025-03-24 201447](https://github.com/user-attachments/assets/f8149444-e3f1-4a96-b72e-52ffd916376f)


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
![Screenshot 2025-03-25 130504](https://github.com/user-attachments/assets/64f4b10a-84cd-410a-bc95-f81170750b52)

 #case 1:
 PMOSFET = length is 180nm, width is 100m
NMOSFET = length is 180nm, width is 28.2um
#DC analysis:
![Screenshot 2025-03-25 141540](https://github.com/user-attachments/assets/cacdc4c3-acbc-4681-a800-123a76cd9f01)

Vout= 1.202v
Vx= 1.206v
Iref = 0.277mA
# TRANSIENT ANALYSIS
![Screenshot 2025-03-25 141617](https://github.com/user-attachments/assets/d455f4f8-4696-47f2-a402-89b966a70e45)


# AC ANALYSIS:
![Screenshot 2025-03-25 141644](https://github.com/user-attachments/assets/0bdc3491-0465-4353-bad9-05ccdb821121)


# Case 2: 500nm

PMOSFET = length is 500nm, width is 100u
NMOSFET = length is 500nm, width is 35.5
Vout= 1.71936v
Vx= 1.15586v
Iref = 0.277mA
![Screenshot 2025-03-25 131615](https://github.com/user-attachments/assets/358ff88d-39ad-4b22-8a18-146eb90545ea)

# TRANSIENT ANALYSIS:
![Screenshot 2025-03-25 132201](https://github.com/user-attachments/assets/df3b6bc9-ce42-4847-b633-200abcb5c7ef)

#  AC ANALYSIS:
![Screenshot 2025-03-25 132320](https://github.com/user-attachments/assets/d8b30127-6357-42b6-a884-3d6cd6370ad7)


# Case 3: 1umm PMOSFET = length is 1um, width is 100u
NMOSFET = length is 1um, width is 40um
Vout= 1.72293
Vx= 1.07207
Iref = 0.277mA
![Screenshot 2025-03-25 132910](https://github.com/user-attachments/assets/a5a7cb55-9554-48bc-b2a1-e025d3ee41f9)

# TRANSIENT ANALYSIS:
![Screenshot 2025-03-25 133045](https://github.com/user-attachments/assets/4d2537a2-d4cc-4e20-a6fc-e322a6b373b2)

#  AC ANALYSIS:
![Screenshot 2025-03-25 133127](https://github.com/user-attachments/assets/9c024b7d-8405-49e1-92d8-bf825de69161)

# Circuit 2:
# Aim : Design the diffrential amplifier having VDD=2V, P<=1mW, Vicm =1V as per the 3rd experiment and perform DC, Transient , AC analysis
![Screenshot 2025-03-25 134911](https://github.com/user-attachments/assets/38dd2abb-c4ce-4d4b-b4fe-24f15834421e)


# TRANSIENT ANALYSIS:
![Screenshot 2025-03-25 135041](https://github.com/user-attachments/assets/8bfd593c-811a-4972-a471-78130fe0f767)

#  AC ANALYSIS:
![Screenshot 2025-03-25 125826](https://github.com/user-attachments/assets/06da16e9-e2bd-49fb-ba65-b5661351e680)

The GAIN from the LTSpice simulation of this circuit is 12db

# INFERENCE:

1.The current mirror circuit effectively replicates a reference current with high accuracy, ensuring stable operation despite supply or load variations.

2.The DC analysis confirms proper biasing and current mirroring.

3.AC analysis demonstrates improved gain and output resistance due to the active load configuration. 

4.The designed differential amplifier with a current mirror successfully enhances performance by improving bias stability and increasing gain.

5.DC analysis confirms proper transistor biasing, AC analysis shows improved gain and bandwidth, and transient analysis verifies stable differential signal amplification.




