# VHDL Counter Overflow Bug

This repository demonstrates a common bug in VHDL code: counter overflow. The provided `counter.vhdl` file contains a simple counter that increments on each rising clock edge. However, it lacks overflow handling, causing incorrect behavior when the counter reaches its maximum value.

The `counter_fixed.vhdl` file provides a corrected version that addresses the overflow issue.

## Bug Description

The original `counter.vhdl` increments the counter indefinitely. Once it reaches the maximum value ("1111"), it wraps around to "0000", which might not be the intended behavior.  This could lead to unexpected errors in a larger design.