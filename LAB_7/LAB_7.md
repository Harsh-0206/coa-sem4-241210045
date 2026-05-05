# COA Lab Experiment

## Design and Implementation of Logical and Arithmetic Shift Operations using 8-bit Shift Register

---

## Aim

To design and implement the following operations using an 8-bit shift register in Logisim:

- Logical Shift Left (LL)
- Logical Shift Right (LR)
- Arithmetic Shift Left (AL)
- Arithmetic Shift Right (AR)
- Rotate Left (RL)
- Rotate Right (RR)
- Rotate Left with Carry (RLC)
- Rotate Right with Carry (RRC)

---

## Software Used

Logisim (NI Circuit Design Suite)

---

## Theory

### Shift Registers

A shift register is a sequential circuit used to store and shift binary data. It consists of a series of flip-flops connected in such a way that data can be shifted left or right on each clock pulse.

An 8-bit shift register stores 8 bits of data and allows shifting operations to be performed.

---

### Logical Shift Operations

#### Logical Shift Left (LL)
- All bits are shifted to the left
- LSB is filled with 0
- MSB is discarded

#### Logical Shift Right (LR)
- All bits are shifted to the right
- MSB is filled with 0
- LSB is discarded

---

### Arithmetic Shift Operations

#### Arithmetic Shift Left (AL)
- Same as logical left shift
- Used in signed multiplication (may cause overflow)

#### Arithmetic Shift Right (AR)
- Preserves the sign bit (MSB)
- MSB is replicated during shift
- Used in signed division

---

### Rotate Operations

#### Rotate Left (RL)
- MSB is moved to LSB position
- No data loss

#### Rotate Right (RR)
- LSB is moved to MSB position
- No data loss

---

### Rotate with Carry Operations

#### Rotate Left with Carry (RLC)
- MSB is moved to Carry flag
- Previous Carry is inserted into LSB

#### Rotate Right with Carry (RRC)
- LSB is moved to Carry flag
- Previous Carry is inserted into MSB

---

## Components Used

- 8-bit Shift Register  
- Flip-flops (if built manually)  
- Multiplexers (for control logic)  
- Clock signal  
- Input switches  
- LEDs (output indicators)  
- Connecting wires  

---

## Circuit Description

- An 8-bit shift register is used to store data  
- Control signals determine the operation (shift/rotate)  
- Multiplexers are used to select input source for shifting  
- Carry bit is used in rotate-with-carry operations  
- Clock pulse triggers the shifting action  

---

## Working

- Input data is loaded into the register  
- Based on control signals, the desired operation is selected  
- On each clock pulse:
  - Bits shift left or right
  - Rotate operations wrap bits around
  - Carry-based operations use an external carry bit  
- Output is displayed using LEDs  

---

## Procedure

- Open Logisim and create a new circuit  
- Place an 8-bit shift register  
- Add multiplexers for selecting operations  
- Provide control inputs for operation selection  
- Connect clock signal  
- Input binary data using switches  
- Run simulation and observe outputs  

---

## Observations

- Logical shifts correctly insert 0s  
- Arithmetic right shift preserves sign bit  
- Rotate operations circulate bits without loss  
- Carry-based rotations correctly use carry input/output  

---

## Result

All shift and rotate operations were successfully implemented using an 8-bit shift register. The outputs obtained match the expected behavior.

---

## Conclusion

- Shift registers are essential for data manipulation  
- Different shift operations serve different purposes  
- Rotate and carry operations are useful in processors  
- The experiment provides practical understanding of bit-level operations  

---

## Author

Harsh Kumar
Course: Computer Organization and Architecture Lab