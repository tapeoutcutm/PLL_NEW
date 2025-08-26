⚙️ How it works
This project implements a Phase-Locked Loop (PLL) designed to lock the phase of an output signal to a reference input. The core architecture includes:

Phase Detector: Compares the input and feedback signals to generate a phase error.

Loop Filter: Smooths the error signal to control the voltage-controlled oscillator (VCO).

VCO: Generates a frequency-adjustable output based on the filtered control voltage.

Feedback Divider: Scales the output frequency for comparison with the reference.

The PLL stabilizes the output frequency and phase, making it suitable for clock generation, frequency synthesis, and jitter reduction in digital systems.

🧪 How to test
To validate the PLL functionality:

Simulation:

Run behavioral simulations using your testbench to verify lock time, jitter, and frequency stability.

Check waveform outputs for phase alignment between reference and output signals.

Hardware Testing:

Deploy the design on an FPGA or ASIC test platform.

Use a signal generator to provide the reference clock.

Monitor the output using an oscilloscope or logic analyzer to confirm phase lock and frequency accuracy.

Lock Detection:

Include a lock signal output in your design to indicate when the PLL has stabilized.

🔌 External hardware
This PLL project may interface with the following external components:

Reference Clock Source: Typically a crystal oscillator or external clock generator.

Test Equipment: Oscilloscope, signal generator, and logic analyzer for validation.

Optional PMOD Interface: For modular integration with FPGA boards.

Power Supply: Stable voltage source for analog blocks (if implemented in mixed-signal flows).
