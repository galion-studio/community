# The layer that wraps everything

Galion Studio · research plan · 23 September 2026

Gate-all-around nanosheet transistors are the current frontier of logic. The channel is no longer one flat slab of silicon with a gate laid on top. It is a stack of thin sheets, and the gate must wrap every sheet on all sides. That geometry restores the channel control the gate had been losing as transistors shrank.

A gate that wraps everything needs a dielectric that wraps everything. The insulating layer between the metal gate and the silicon has to coat the top, the bottom, and both sides of each stacked sheet, at a few nanometres of thickness, without pinholes and without variation. Line-of-sight deposition cannot do that inside a released stack. Atomic layer deposition can. ALD grows the film one self-limiting step at a time from gas-phase chemistry, so it reaches surfaces a shadowed process misses and it stops when the surface is saturated. For gate-all-around, ALD is not one option among several. It is the production method.

The open question is what to deposit. Hafnium oxide has carried the high-k role for a decade, and it remains the reference bulk dielectric: kappa around 20 to 25, mature chemistry, and already qualified on 300 mm lines. Rare-earth oxides occupy a different seat. Lanthanum oxide has a higher kappa, near 27. Yttrium oxide sits lower, roughly 15 to 18. The first useful job for either is not as a bulk replacement. It is as a dipole: one to three angstroms of rare earth at the interface, which shifts the effective work function so the gate stack can reach its threshold-voltage target without thickening the interfacial layer.

That is the near-term insertion. A dipole of La2O3 or Y2O3, a few atomic layers thick and deposited by ALD, inside an otherwise ordinary Hf-based replacement-metal-gate flow. Later, if the chemistry holds, either oxide could serve as a nanolaminate high-k in its own right.

Control is the entire difficulty. Lanthanum oxide is hygroscopic. It draws moisture from air, forms a hydroxide, and reacts with silicon to grow a low-k silicate at the interface. That reaction is the failure mode, and the answer is a cap: Al2O3 above the La2O3, so the stack reads Al2O3 / La2O3 / Al2O3. Yttrium oxide is the more stable of the two and tolerates the flow with less protection. A LaAlOx nanolaminate is the other practical form, mixing the two oxides in repeated thin cycles.

The recipe has knobs. The metal precursor is a lanthanum or yttrium cyclopentadienyl, amidinate, or guanidinate. The oxidant is water, ozone, or an oxygen plasma. The window is 200 to 300 degrees Celsius. Water demands long purges, because residual vapour drives the hydroxide reaction. Released channels get a seed layer first, so the film nucleates evenly instead of clumping. A post-deposition anneal finishes the film, and it has to fit inside the foundry thermal budget, which in practice means at or below 600 Celsius. Thickness variation is the number to hold: better than plus or minus 2 percent across a 300 mm wafer.

The work order runs from simple to hard. Blanket silicon first. Dummy high-aspect-ratio wires second, to prove that the film reaches the buried surfaces. Capacitors third, for the electrical data. Short-loop gate-all-around devices last. Metrology follows the same logic: TEM-EELS on the inner sheet, to see the film on the surface no one can reach from outside; XPS for chemistry; capacitance-voltage for the electrical thickness and the trap density; and humidity tests comparing capped films against uncapped ones.

The insertion point is the replacement-gate module, after channel release. The sequence is interfacial layer, ALD high-k carrying the rare-earth dipole, work-function metal, fill, then CMP. Foundries already run Hf-based gate-all-around flows at the leading nodes, and the rare-earth oxides appear in their patent record as dipole layers rather than as the primary dielectric.

One item comes before any node commitment: electronic-grade precursor supply from two qualified sources, locked and qualified in advance. A recipe that depends on a single supplier is not a recipe a foundry can adopt.

This plan does not claim that La2O3 or Y2O3 will replace HfO2. The near-term path is a conformal dipole or nanolaminate inside a normal Hf-based replacement-metal-gate stack. Success is wrap-around uniformity, EOT, interface traps, reliability on multi-sheet GAA devices, and a 300 mm recipe with a qualified precursor supply.
