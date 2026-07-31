# Half Adder using Verilog

## Overview
A Half Adder is a combinational logic circuit that adds two single-bit binary numbers. It produces two outputs:

- Sum (S)
- Carry (C)

## Truth Table

| A | B | Sum | Carry |
|---|---|-----|-------|
| 0 | 0 |  0  |   0   |
| 0 | 1 |  1  |   0   |
| 1 | 0 |  1  |   0   |
| 1 | 1 |  0  |   1   |

## Logic Equations

Sum = A XOR B

Carry = A AND B

## Files

- `half_adder.v` - Verilog implementation
- `half_adder_tb.v` - Testbench
- `simulation_results.png` - Simulation waveform

## Software Used

- ModelSim
- Vivado
- Icarus Verilog
- GTKWave

## How to Simulate

### Using Icarus Verilog

Compile

```bash
iverilog -o halfadder half_adder.v half_adder_tb.v
```

Run

```bash
vvp halfadder
```

Generate waveform

```bash
gtkwave half_adder.vcd
```

## Expected Output

```
A B | Sum Carry
0 0 |  0    0
0 1 |  1    0
1 0 |  1    0
1 1 |  0    1
```

## Author

Your Name