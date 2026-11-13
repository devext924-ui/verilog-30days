# verilog-30days

30 days of Verilog RTL design and verification, from basic gates to an async FIFO and a UART/APB capstone. Every design comes with a self-checking testbench, simulated on [EDA Playground](https://www.edaplayground.com).

## Tools

- [EDA Playground](https://www.edaplayground.com) with Icarus Verilog for simulation
- EPWave (built into EDA Playground) for waveforms
- [Yosys](https://yosyshq.net/yosys/) on EDA Playground for synthesis checks (Day 17 onward)

## Repo layout

```
dayNN_topic/
├── design.sv      # synthesizable RTL (EDA Playground "design" pane)
├── testbench.sv   # self-checking testbench ("testbench" pane)
└── waveform.png   # EPWave screenshot
```

## How to run

Open the day's EDA Playground link in the table below and click **Run**. To run it yourself, paste `design.sv` and `testbench.sv` into a new playground, select **Icarus Verilog**, and tick **Open EPWave after run**.

## Progress

| Day | Topic | Designs | EDA Playground | Status |
|-----|-------|---------|----------------|--------|
| 01 | Setup + first modules | Half adder, full adder | — | ⬜ |
| 02 | Data types, vectors | N-bit ripple-carry adder | — | ⬜ |
| 03 | Operators, dataflow | 4:1 mux (3 styles), comparator | — | ⬜ |
| 04 | Behavioural modelling | Decoder, priority encoder, 7-seg | — | ⬜ |
| 05 | Testbench basics | Self-checking adder TB | — | ⬜ |
| 06 | Flip-flops | DFF/TFF/JKFF, shift registers | — | ⬜ |
| 07 | Re-entry revision | Rebuilds from memory | — | ⬜ |
| 08 | Counters | Up/down, mod-N, ring, Johnson, LFSR | — | ⬜ |
| 09 | FSMs I | 1011 detector (Moore/Mealy) | — | ⬜ |
| 10 | FSMs II | Traffic light, vending machine | — | ⬜ |
| 11 | Hierarchy, generate | Generate adder, 16:1 mux | — | ⬜ |
| 12 | Checkpoint | 8-bit ALU | — | ⬜ |
| 13 | Memories | ROM, single/dual-port RAM | — | ⬜ |
| 14 | Sync FIFO | Parameterised FIFO | — | ⬜ |
| 15 | Advanced TBs | Scoreboard FIFO TB | — | ⬜ |
| 16 | Sim semantics | NBA/race experiments | — | ⬜ |
| 17 | Synthesis | Yosys netlists, latch fix | — | ⬜ |
| 18 | Signed arithmetic | Signed add/sub, array multiplier | — | ⬜ |
| 19 | Datapath | CLA, shift-add, Booth multiplier | — | ⬜ |
| 20 | UART TX | Baud gen + TX | — | ⬜ |
| 21 | UART RX | RX + loopback | — | ⬜ |
| 22 | SPI | SPI master (4 modes) | — | ⬜ |
| 23 | Interview circuits | Clock dividers, edge detect, PWM | — | ⬜ |
| 24 | CDC | 2-FF, pulse, handshake sync | — | ⬜ |
| 25 | Async FIFO | Gray-pointer FIFO | — | ⬜ |
| 26 | Async FIFO verif | Dual-clock scoreboard TB | — | ⬜ |
| 27 | Timing, pipelining | Pipelined MAC | — | ⬜ |
| 28 | Capstone: spec | APB-mapped UART + FIFO blocks | — | ⬜ |
| 29 | Capstone: ship | Integrated system + TB | — | ⬜ |
| 30 | Final drill | Timed rewrites | — | ⬜ |

## License

[MIT](LICENSE)
