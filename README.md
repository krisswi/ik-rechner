# Short-Circuit Current Calculator (Ik Tool)

This web-based tool calculates the short-circuit current (Ik) at the end of a cable based on a known short-circuit current at the supply point.

The application is intended for professional use in **Switzerland** and follows the relevant Swiss installation practice (NIN).

## Purpose

The tool allows quick verification whether the calculated short-circuit current at the end of a conductor is sufficient for the selected protective device to trip within the required disconnection time.

## Inputs

- Voltage (U0) – default 230 V (editable)
- Short-circuit current at origin (Ik start)
- Cable length
- Copper conductor cross-section
- Conductor configuration:
  - 1-pole (factor 2 × L)
  - 3-pole (factor √3 × L)
- Protective device type:
  - DIAZED
  - DIN gG/gL
  - MCB B / C / D
- Rated current (In)
- Disconnection time (0.4 s / 5 s)
- NIN correction factor (1.00 / 0.66)

## Calculation

The tool calculates:

- Loop resistance of the cable (Copper, ρ = 0.0178 Ω·mm²/m)
- Total impedance at the cable end
- Short-circuit current at the cable end
- Minimum required short-circuit current according to the stored Swiss reference table

The calculated value is automatically compared with the required minimum value and displayed as:

- **OK**
- **NOT OK**

## Disclaimer

This tool is intended as a calculation aid only.  
It does not replace a compliant loop impedance measurement at the installation site.  
Results depend entirely on the accuracy of the input values.
