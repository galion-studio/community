# ALD for GAA · working plan

Galion Studio · research plan · 23 September 2026

## Scope

Gate-all-around (GAA) nanosheet transistors need a dielectric that wraps every surface of stacked channels. ALD is the production method that can do that. La2O3 (kappa about 27) and Y2O3 (kappa about 15 to 18) matter first as 1 to 3 angstrom dipole layers on HfO2, and only later as nanolaminate high-k if moisture and silicate growth stay under control. HfO2 remains the reference bulk high-k (kappa about 20 to 25).

## Materials table

| Material | Kappa (approx.) | Role in the stack | Main risk |
| --- | --- | --- | --- |
| HfO2 | 20 to 25 | Reference bulk high-k | Baseline reference, mature |
| La2O3 | about 27 | 1 to 3 angstrom dipole layer on HfO2; later nanolaminate | Hygroscopic, hydroxide in air, low-k silicate on Si |
| Y2O3 | 15 to 18 | 1 to 3 angstrom dipole layer on HfO2; later nanolaminate | Less stable than HfO2 but more stable than La2O3 |
| Al2O3 | cap / barrier | Caps La2O3 to block moisture and silicate growth | Adds EOT if too thick |
| LaAlOx | mixed | Nanolaminate of La2O3 and Al2O3 | Composition control |

Practical stack: Al2O3 / La2O3 / Al2O3, or a LaAlOx nanolaminate. Y2O3 is the more stable of the two rare earths.

## Recipe knobs

- Precursor: La and Y cyclopentadienyl, amidinate, guanidinate.
- Oxidant: water, ozone, or oxygen plasma.
- Temperature: 200 to 300 C.
- Long purges after water.
- Seed layer on released channels.
- Post-deposition anneal inside the foundry thermal budget, often at or below 600 C.
- Target thickness variation under plus or minus 2 percent on 300 mm.

## Lab order

1. Blanket silicon.
2. Dummy high-aspect-ratio wires.
3. Capacitors.
4. Short-loop GAA devices.

## Metrology

- TEM-EELS on the inner sheet.
- XPS.
- C-V.
- Humidity tests on capped versus uncapped films.

## Insertion point

The replacement-gate module after channel release: interfacial layer, ALD high-k with the rare-earth dipole, work-function metal, fill, CMP.

Foundries already run Hf-based GAA (TSMC N2, Intel 18A, Samsung SF2). Rare-earth oxides show up in patents as dipole layers, not as the primary dielectric. Lock dual-source electronic-grade precursor supply before any node commitment.

## Caveat

This plan does not claim that La2O3 or Y2O3 will replace HfO2. The near-term path is a conformal dipole or nanolaminate inside a normal Hf-based replacement-metal-gate stack. Success is wrap-around uniformity, EOT, interface traps, reliability on multi-sheet GAA devices, and a 300 mm recipe with a qualified precursor supply.
