# Behavioral definitions
> Note: This section is incomplete.

Functionally when we use a circuit we don't care how that circuit
is implemented. Nor do we care how it functions. We care how it behaves and what
value it adds to our lives.

So if we care about how a circuit adds value to our lives would it not make
sense to start at a high level of abstraction and just say hey. What do I want
my circuit to be able to do?

Consider an example of a fitness tracker that counts your steps and displays
that on a screen. But does nothing else.

If we break this behavior down into it's components we get a;
- Sensor to detect a step,
- Computation system to interpret sensor output,
- Counter to keep track of steps,
- Display to show us the steps,

TODO: Add a code example here defining custom constraints.