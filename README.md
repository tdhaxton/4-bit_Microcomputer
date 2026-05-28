# 4-bit_Microcomputer
fully-functional 4-register, 4-bit microcomputer in VHDL, implementing a complete hierarchical digital system across eight interdependent components.

This project involved designing the MCA-4 microcomputer, which is a microcomputer with
four, four-bit registers, and is capable of load, addition, shift, move, negate and display
operations. The resulting design performs all operations as instructed. However, the
computer does not wait on a clock pulse to display a register when requested, and the
output switches back to the contents of register zero after a new command is input,
instead of waiting for a clock pulse. This is due to the design for the 4:16 decoder taking an
enable signal that consisted of an AND operation between the first and second input
command bits (7 and 6). Once enabled, the decoder outputs the register called for by the
signal bits (5 and 6), and reverts back to register zero when the enable signal stops.
