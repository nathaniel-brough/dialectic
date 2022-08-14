# Generating a netlist
> Note: This description is still a work in progress.

The process for generating a net-list for a design is not dissimilar to the
process of generating the BOM.

We take each constraint in the BOM and match abstract concepts against physical
interfaces. In the previous example of a step counter we had an accelerometer
that interfaced with a microcontroller via SPI. In many cases it's useful to
defer a concrete net-list to the routing stage. Instead of saying that PinA1 is
going to be SPI1-Clock and then routing as is, we can say that the
accelerometer uses one of the SPI interfaces provided by the microcontroller and
allow the routing algorithm to pin-swap to optimize the circuit.

> Note: There is of course a problem with this approach and that is each pin has
> a finite set alternative functions, and even if a micro-controller provides 4
> SPI interfaces it might not be possible to use all of them if other GPIO pins
> are also being used. This seems like a solvable problem, but as it currently
> stands an algorithm to solve this hasn't been developed for dialectic.