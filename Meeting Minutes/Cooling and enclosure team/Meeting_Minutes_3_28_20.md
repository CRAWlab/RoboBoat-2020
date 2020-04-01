## Water Cooling System Team Meeting 3/28/20
### Contributions made by: Joseph Stevens, Thomas Poche, Bradley Este
### Topics
***Attributes of System***
1. Steady flow process
	* Steady flow conditions can be closely approximated by pumps.
2. Treat aluminum baseplate as heat sink.
3. Treat the lake as a thermal energy reservoir
	* Can absorb finite amounts of heat without undergoing any change in temperature.
  	Therefore, it can be assumed that new cool water coming into the system would not be affected by old warm water exiting the system even though they are coming from the same body of water.
	* Also, incoming water can be assumed to be approximately 80 degrees
  	Fahrenheit. This was approximated by the reported average salt water temp at Daytona Beach Florida in the following link:
  	<https://www.currentresults.com/Oceans/Temperature/daytona-beach-average-water-temperature.php>
	* The above implies that the incoming water could be expected to remain at a constant temperature of approximately 80 degrees F during the steady flow process.
4. Temperature range of the Jetson = -13 deg F to 176 deg F
5. Temperature range of the Pyboard = find

***Design Ideas***
1. "Pump and Dump" - Pump the water in from the lake. Use the water to cool the system through a heat exchanger attached to the aluminum base plate of the CPUs and dump the water back in to the lake. This method would collect fresh water at approximately 80 deg F while operating as a steady flow process.
	* Inlet and exit hoses should be designed in such a way to reduce drag and it's negative effect on the dynamics of the boat to avoid unexpected complications with the controller.
		* An inlet hose should be placed at about center of mass under the box between the two pontoons.
		* The exit hose should come out of the side of the box and not be submerged under water like the inlet hose but instead be curved down to allow the warm water to exit into the lake.
	* Heat Exchanger Idea #1 - Have a water cooling block attached to the bottom of the base plate
	  consisting of one copper plate that makes direct contact with the aluminum base plate while the
	  other exposed sides are insulated to ensure maximum heat transfer between the base plate and the
	  cooling block.
		* Concerns:
			1. Incomplete coverage of copper plate by the water due to possible cavitation.
			2. Block may need to be custom built to insure proper coverage.
		* Possible solution:
			1. Have the inlet hose coming in from the top of one side of the cooling block and the exit
			   hose on the top of the opposite side. This should insure proper pressure and coverage on
			   the inside of the cooling block.
	* Heat Exchanger Idea #2 - Have an evaporator/radiator on the inside of the box up against the
	  bottom of the aluminum base plate to absorb heat rather than a cooling block. This could
	  eliminate concerns of cavitation.
		* Concerns:
			1. Area of coverage in comparison to previous idea being reduced and therefore reducing the
			    effect of the heat transfer.
			2. Possible increase in cost.
			3. May complicate system.
	* Heat Exchanger Idea #3 - Use copper piping

2. Radiator - have a closed system with a radiator mounted on the outside of the box. Would require a fluid reservoir. The radiator would dissipate heat into the atmosphere while the atmosphere acted as a thermal energy reservoir. There would most likely need to be a fan attached to the radiator to circulate air through the fins while the boat is stopped.

 ***Future Research***
 1. Battery draw from pump and fan
 2. Once a general idea for a system has been decided on, calculations need to be made to support the theory that the system will work.
 	* What type of pump would we need to supply a volume/mass flow rate sufficient enough for cooling
	* What diameter tubing would be needed for proper flow rate
 4. Cost of a radiator and evaporator vs a cooling block.  
