# Analysis preconditions
> Note: This section is incomplete.

This stage in the pipeline is used to constrain your design e.g.
- The operating temperature, pressure, humidity ranges.
- The PCB manufacturing process.
- The PCB assembly process.

This stage isn't intended to do anything particularly fancy. Instead it is just
a means of collecting data to constrain the design at later stages in the
pipeline.

## Operating environment
The following set of constraints are proposed to optionally constrain the design of your device;
- Temperature range.
- Pressure range.
- Vibration.
- Humidity.
- Heat dissipation.

## PCB Manufacturing
The following set of constraints are proposed to optionally constrain the design of your device;

### Vias
- Minimum width annular ring.
- Drill sizes (list)
- Microvias
- Blind vias
- Buried vias
- Plug hole diameter

### Clearance
- Minimum trace width
- Hole to hole clearance

### Stackup
- List of material variants
  - Fiberglass (FR4)
  - Copper
  - Prepreg
  - Solder-mask
  - etc.