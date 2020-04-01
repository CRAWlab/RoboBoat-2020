
## Water Cooling System Team Report
### Contributions made by: Joseph Stevens, Thomas Poche, Bradley Este
### Topics
***Attributes of System***
1. Steady flow process
	* Steady flow conditions can be closely approximated by by pumps and fans.
2. Treat aluminum baseplate as heat sink. 
3. Treat the lake or outside air from atmosphere as a thermal energy reservoir
	* Can absorb finite amounts of heat without undergoing any change in temperature.
  	Therefore, it can be assumed that new cool water or air coming into the system would not be affected by old warm water exiting the system even though they are coming from the same body of water.
	* Also, incoming water can be assumed to be approximately 80&deg;F and incoming air approximately 88&deg;F. 
	* The water temperature was approximated by the reported average salt water temp at Daytona Beach Florida in the following link: [Water temp historical average](https://www.currentresults.com/Oceans/Temperature/daytona-beach-average-water-temperature.php)
	 * The air temperature was approximated by reviewing the historical average during June from the 22nd -28th here:[Air temp historical average](https://www.accuweather.com/en/us/daytona-beach/32114/june-weather/328173)
	* The above implies that the incoming water or air could be expected to remain at a constant temperature of approximately 80&deg;F or 88&deg;F, respectively.
4. Temperature range of the Jetson = -13&deg;F to 176&deg;F
5. Temperature range of the Pyboard = need to get exact model to find

***Design Ideas***
1. "Pump and Dump" - Pump the water in from the lake. Use the water to cool the system through a heat exchanger attached to the aluminum base plate of the CPUs and dump the water back in to the lake. This method would collect fresh water at approximately 80 deg F while operating as a steady flow process. 
	* Inlet and exit hoses should be designed in such a way to reduce drag and it's negative effect on the dynamics of the boat to avoid unexpected complications with the controller.
		* An inlet hose should be placed at about center of mass under the box between the two pontoons. 
		* The exit hose should come out of the side of the box and not be submerged under water like the inlet hose but instead be curved down to allow the warm water to exit into the lake.
	* Heat Exchanger Idea #1 - have a water cooling block attached to the bottom of the base plate
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
	* Heat Exchanger Idea #2 - have an evaporator/radiator on the inside of the box up against the
	  bottom of the aluminum base plate to absorb heat rather than a cooling block. This could
	  eliminate concerns of cavitation.
		* Concerns:
			1. Area of coverage in comparison to previous idea being reduced and therefore reducing the
			    effect of the heat transfer.
			2. Possible increase in cost.
			3. May complicate system.
	* Heat Exchanger Idea #3 - use copper piping
	
7. Radiator - have a closed system with a radiator mounted on the outside of the box. Would require a fluid reservoir. The radiator would dissipate heat into the atmosphere while the atmosphere acted as a thermal energy reservoir. There would most likely need to be a fan attached to the radiator to circulate air through the fins when the boat is stopped.

8. Air cooled system
9.  Intake and Exhaust
	* Snorkel air intake with spout and opening pointing downward. 
		* Exhaust and Intake should be symmetrical with respect to each other due to the holonomic capabilities of the boat. This is preferred in order to keep the same functionality when driving in reverse. 
			[Something similar to this, but not exactly](https://www.wish.com/product/598a140c08e12d09fc918b64?hide_login_modal=true&from_ad=goog_shopping&_display_country_code=US&_force_currency_code=USD&pid=googleadwords_int&c=%7BcampaignId%7D&ad_cid=598a140c08e12d09fc918b64&ad_cc=US&ad_curr=USD&ad_price=9.88&campaign_id=7203534630&gclid=Cj0KCQjw1Iv0BRDaARIsAGTWD1un2uznoSLaLp57aooTYjIFVpUlnZ-i83nC90eIvOSy9uJaWBWzo30aAvsEEALw_wcB&share=web)
		* Inlet fan and exhaust fan to create flow of air through system
			[Something like this](https://www.newegg.com/p/1YF-009M-001J3?Description=blower%20fan&cm_re=blower_fan-_-9SIA27CAK71375-_-Product)
			[Or like this](https://www.newegg.com/nonoise-g5015m12d1-6-fans/p/1YF-002N-00090?Item=9SIA6254FA5101&quicklink=true)
			There is another one on McMASTER-CARR but it's relatively expensive. Although, I do plan on using this in the Solidworks assembly of the system. To view this fan click [here.](https://www.mcmaster.com/9602k41)
		* Possible safety system with two closing flaps shuts off all outside environments when IMU board indicates tipping past a certain point.
		* Water resistant membrane that allows air flow
10. Internals
	* Heat sink with fan in middle to pull heat directly from the source. This would transfer heat from the from the aluminum base board to the 4 heat pipes through the coils and be carried out with the flow of air created by the intake and exhaust fans.
		[Heat sink example here](https://www.amazon.com/Noctua-NH-U12S-Premium-Cooler-NF-F12/dp/B00C9EYVGY/ref=sr_1_3?keywords=noctua%20nh-u12s&qid=1585513334&sr=8-3)
		[And here](https://www.coolermaster.com/catalog/coolers/cpu-air-coolers/hyper-212-evo/)

***Conclusions***
1. Decision made to switch focus to an air cooled system first
	 * Design is more simplistic and may be a part of a more complicated design in the future. If it is determined that a more complicated design is needed, then research from an air cooled system be used as well. E.I. may have some type of integration between water and air cooled system. Therefore, this seems the most time efficient route to start with. 
	 * The idea was to start here and if it a greater need is determined after further investigation and calculation to move to a more complicated system.
	 *  Concerns of water system intake pipe and exit pipe creating drag would be avoided if successful.
	 * It also worth mentioning that a typical water pump used in a computer cooling system was found to draw 19 Watts and the fans that we have looked into using would only draw approximately 7.4 W with all three combined. Technical data: [Arctic Fan](https://www.arctic.ac/us_en/p12.html), [Cooler Master Heat Sink Fan](https://www.coolermaster.com/catalog/coolers/cpu-air-coolers/hyper-212-evo/), [Pump](https://www.amazon.com/BXQINLENX-DC12V-Cooling-Exchanger-Cooler/dp/B01H1BE4VQ/ref=sr_1_7?crid=287DINFZONEG9&keywords=water%20cooling%20pump&qid=1585513800&sprefix=water%20cooling%20,aps,194&sr=8-7)
	 
***Future Research***

1. Team is going to begin research in "Heat Transfer 10th Edition" by J.P. Holman on forced air convection cooled systems to start modeling the system and begin some calculations. We believe this is the next step and we have a good decent general mapping of a system to begin investigation.
3. Need to get a copy of 2019 team report for specs
4. Need to get a boat dimensions for proper system design
5. Finish Solidworks model by next report
 6. Once a general idea for a system has been decided on, calculations need to be made to support the theory that the system will work.
 	* What type of pump would we need to supply a volume/mass flow rate sufficient enough for cooling 
	* What diameter tubing would be needed for proper flow rate
 7. Cost of a radiator and evaporator vs a cooling block.  
