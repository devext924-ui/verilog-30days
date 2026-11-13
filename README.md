# verilog-30days

30 days of Verilog RTL design and verification, from basic gates to an async FIFO and a UART/APB capstone. Every design comes with a self-checking testbench.

## Tools

- [Icarus Verilog](https://steveicarus.github.io/iverilog/) for simulation
- [GTKWave](https://gtkwave.sourceforge.net) for waveforms
- [Yosys](https://yosyshq.net/yosys/) for synthesis checks

## Repo layout

```
dayNN_topic/
├── rtl/        # synthesizable design files
├── tb/         # testbenches
├── sim/        # waveform screenshots (.png)
└── README.md   # what was built + results
```

## How to run

```bash
cd day01_adders
iverilog -o sim.out rtl/*.v tb/*.v
vvp sim.out
gtkwave dump.vcd
```

## Progress

| Day | Topic | Designs | Status |
|-----|-------|---------|--------|
| 01 | Setup + first modules | Half adder, full adder | ⬜ |
| 02 | Data types, vectors | N-bit ripple-carry adder | ⬜ |
| 03 | Operators, dataflow | 4:1 mux (3 styles), comparator | ⬜ |
| 04 | Behavioural modelling | Decoder, priority encoder, 7-seg | ⬜ |
| 05 | Testbench basics | Self-checking adder TB | ⬜ |
| 06 | Flip-flops | DFF/TFF/JKFF, shift registers | ⬜ |
| 07 | Re-entry revision | Rebuilds from memory | ⬜ |
| 08 | Counters | Up/down, mod-N, ring, Johnson, LFSR | ⬜ |
| 09 | FSMs I | 1011 detector (Moore/Mealy) | ⬜ |
| 10 | FSMs II | Traffic light, vending machine | ⬜ |
| 11 | Hierarchy, generate | Generate adder, 16:1 mux | ⬜ |
| 12 | Checkpoint | 8-bit ALU | ⬜ |
| 13 | Memories | ROM, single/dual-port RAM | ⬜ |
| 14 | Sync FIFO | Parameterised FIFO | ⬜ |
| 15 | Advanced TBs | Scoreboard FIFO TB | ⬜ |
| 16 | Sim semantics | NBA/race experiments | ⬜ |
| 17 | Synthesis | Yosys netlists, latch fix | ⬜ |
| 18 | Signed arithmetic | Signed add/sub, array multiplier | ⬜ |
| 19 | Datapath | CLA, shift-add, Booth multiplier | ⬜ |
| 20 | UART TX | Baud gen + TX | ⬜ |
| 21 | UART RX | RX + loopback | ⬜ |
| 22 | SPI | SPI master (4 modes) | ⬜ |
| 23 | Interview circuits | Clock dividers, edge detect, PWM | ⬜ |
| 24 | CDC | 2-FF, pulse, handshake sync | ⬜ |
| 25 | Async FIFO | Gray-pointer FIFO | ⬜ |
| 26 | Async FIFO verif | Dual-clock scoreboard TB | ⬜ |
| 27 | Timing, pipelining | Pipelined MAC | ⬜ |
| 28–29 | Capstone | APB-mapped UART + FIFO | ⬜ |
| 30 | Final drill | — | ⬜ |

Replace ⬜ with ✅ as each day is done.

## License

[MIT](LICENSE)
