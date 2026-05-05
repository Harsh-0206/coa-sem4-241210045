# COA Lab Experiment

## Design and Implementation of 4-bit Ripple Carry Adder using Logisim

---

## Aim

To design, implement, and verify a **4-bit Ripple Carry Adder** using basic logic gates in Logisim.

---

## Software Used

Logisim (NI Circuit Design Suite)

---

## Theory

### Full Adder

A full adder is a combinational circuit that performs the addition of three binary inputs:

- Two significant bits (A and B)  
- One carry input (Cin)  

It produces:

- Sum (S)  
- Carry output (Cout)  

#### Equations:

Sum:
S = A ⊕ B ⊕ Cin  

Carry:
Cout = (A · B) + (Cin · (A ⊕ B))  

---

### Ripple Carry Adder

A Ripple Carry Adder is formed by cascading multiple full adders.

- Each full adder adds one bit  
- Carry output of one stage becomes carry input of next stage  
- Carry propagates (ripples) from LSB to MSB  

For a 4-bit adder:

- Inputs: A₃ A₂ A₁ A₀ and B₃ B₂ B₁ B₀  
- Outputs: S₃ S₂ S₁ S₀ and final carry Cout  

---

## Components Used

- XOR gates  
- AND gates  
- OR gates  
- Input switches  
- LEDs (output indicators)  
- Connecting wires  

---

## Circuit Description

- The circuit consists of **four full adders connected in series**
- Each full adder is implemented using:
  - XOR gates for sum calculation  
  - AND and OR gates for carry generation  
- The carry output of each stage is connected to the next stage
- The first stage takes initial carry input (Cin = 0)

---

## Working

1. The least significant bits (A₀, B₀) are added first  
2. Carry generated is passed to the next stage  
3. This process continues through all four stages  
4. Final output consists of:
   - 4-bit sum  
   - 1-bit carry output  

---

## Truth Table (Full Adder)

| A | B | Cin | Sum | Cout |
|---|---|-----|-----|------|
| 0 | 0 |  0  |  0  |  0   |
| 0 | 0 |  1  |  1  |  0   |
| 0 | 1 |  0  |  1  |  0   |
| 0 | 1 |  1  |  0  |  1   |
| 1 | 0 |  0  |  1  |  0   |
| 1 | 0 |  1  |  0  |  1   |
| 1 | 1 |  0  |  0  |  1   |
| 1 | 1 |  1  |  1  |  1   |

---

## Procedure

- Open Logisim and create a new circuit  
- Place XOR, AND, and OR gates  
- Construct a full adder  
- Replicate the full adder four times  
- Connect carry output of each stage to next stage  
- Provide inputs using switches  
- Observe outputs using LEDs  

---

## Observations

- Each stage correctly computes sum and carry  
- Carry propagates sequentially from LSB to MSB  
- Final output matches binary addition  

---

## Result

The 4-bit Ripple Carry Adder was successfully designed and simulated. The outputs obtained are correct as per theoretical calculations.

---

## Conclusion

- Ripple Carry Adder is simple and easy to design  
- It demonstrates carry propagation between stages  
- However, delay increases due to ripple effect  

---

## Author

Harsh Kumar  
Course: Computer Organization and Architecture Lab