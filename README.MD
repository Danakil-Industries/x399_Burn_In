

This project is about developing a low cost burn-in station for LM399s and ADR1399s in TO-46 packages.


Goals:
	1. Reference-supply rails seperate from, or at least derived from, heater supply rail.
	2. Able to burn-in at least 4 Vrefs simultaneously per unit
	3. All components at least 0603 or larger for ease of assembly
		*Preferrably 0805 or larger
	4. Socketed Vrefs
		*Probably use 2mm 2x2 F headers.
	5. Low cost
		*Possibly have multiple variants, enabling people to not need to spend more on functions they might not want to spend money on
			*Make bare-bones design
	Optional 1 (abandoned): Have a resettable hour meter to keep track of how long the Vrefs have been burning in for
								*Would have increased cost too much. Maybe make as an accessory for the unit?
	Optional 2: Have LEDs for indicating that the heater and +15v rail are alive
	Optional 3: Hot-swapable X399s
					*Alternatively, have a way to safely load a Vref without powering down the whole unit
					*Might end up being too expensive
	Optional 4: LEDs showing if the voltage seen at the X399's Vref+ pin is too high(>≈7.5v), fine(≈7.5v>Vref>≈6.5v), or too low(<≈6.5v)
					*Yes, this range is WAY over the tolerances of the Vrefs. It is meant to indicate if something has gone seriously wrong.
	Optional 5: If Vref+ voltage is too high, shut down the current supply, go into an error state, and light an error LED.
	