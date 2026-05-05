# COA Lab Experiment

## Design and Implementation of Multiplexers, Priority Encoder, and Boolean Functions using Logisim

---

## Aim

To design, implement, and verify the following combinational circuits using Logisim:

- Multiplexer using smaller MUX units (MUX tree)  
- 8:1 Multiplexer  
- Priority Encoder  
- Boolean functions using Sum of Products (SOP) form  

---

## Software Used

Logisim (NI Circuit Design Suite)

---

## Theory

### Multiplexer (MUX)

A multiplexer is a combinational circuit that selects one input from multiple inputs and forwards it to a single output based on select lines.

For an 8:1 multiplexer:

- Number of inputs = 8  
- Number of select lines = 3  
- Output depends on the binary value of select lines  

---

### MUX Tree (Hierarchical Design)

A larger multiplexer can be constructed using smaller multiplexers. For example, an 8:1 MUX can be implemented using multiple 2:1 MUX units arranged in stages:

- First stage selects between input pairs  
- Intermediate stages combine outputs  
- Final stage produces a single output  

This approach demonstrates modular and scalable circuit design.

---

### Priority Encoder

A priority encoder is a combinational circuit that outputs the binary representation of the highest-priority active input.

- If multiple inputs are active, the input with the highest priority is encoded  
- A valid output signal may be used to indicate the presence of an active input  

---

### Boolean Function using SOP

Boolean functions can be implemented using Sum of Products (SOP) form:

- AND gates generate minterms  
- OR gates combine selected minterms  

Example:

F = Σm(4, 5, 6, 7)

---

## Components Used

- 2:1 Multiplexers  
- 8:1 Multiplexer  
- Priority Encoder module  
- AND gates  
- OR gates  
- Input switches (logic 0 and 1)  
- LEDs (output indicators)  
- Connecting wires  

---

## Circuit Description

### MUX Tree Implementation

Multiple 2:1 multiplexers are connected in a hierarchical structure:

- First level processes input pairs  
- Outputs are fed into higher-level multiplexers  
- Final stage produces a single output  

This configuration behaves as a higher-order multiplexer.

---

### Priority Encoder

- Multiple inputs are connected to the encoder  
- Output lines represent the binary index of the highest-priority active input  
- LEDs indicate the encoded output  

---

### 8:1 Multiplexer

- Eight inputs are connected (logic constants or signals)  
- Three select lines determine which input is passed to the output  
- Output is observed using an LED  

---

### SOP Logic Implementation

- Inputs are applied to AND gates to generate minterms  
- Selected minterms are combined using OR gates  
- Multiple outputs represent different Boolean expressions  

F₁ = Σm(4, 5, 6, 7)  
F₂ = Σm(2, 3, 6, 7)  
F₃ = Σm(1, 3, 5, 7)  

---

## Procedure

- Open Logisim and create a new design file  
- Place the required components from the component library  
- Construct the circuits:  
  - Build the MUX tree using 2:1 multiplexers  
  - Configure the 8:1 multiplexer with appropriate inputs and select lines  
  - Connect the priority encoder with multiple inputs and output indicators  
  - Implement SOP expressions using AND and OR gates  
- Provide input values using switches  
- Run the simulation  
- Observe and verify outputs using LEDs  

---

## Observations

- The multiplexer correctly selects inputs based on select lines  
- The MUX tree behaves as a higher-order multiplexer  
- The priority encoder outputs the correct binary value for the highest-priority active input  
- SOP-based circuits generate correct outputs for given input combinations  

---

## Result

All circuits were successfully designed and simulated in Logisim. The outputs obtained match the expected theoretical results.

---

## Conclusion

The experiment demonstrates:

- Implementation of multiplexers using both direct and hierarchical approaches  
- Working of a priority encoder  
- Realization of Boolean functions using SOP form  
- Practical understanding of combinational circuit design  

---

## Author

Harsh Kumar  
Course: Computer Organization and Architecture Lab