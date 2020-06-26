Analyze International Debt Statistics
==========================

Project Description
--------------

It's not that we humans only take debts to manage our necessities.
A country may also take debt to manage its economy. For example,
 infrastructure spending is one costly ingredient required for a
 country's citizens to lead comfortable lives. The World Bank is the organization that provides debt to countries.

In this project, you are going to analyze international debt data collected by The World Bank. 
The dataset contains information about the amount of debt (in USD) owed by developing countries
 across several categories. 

	- You are going to find the answers to questions like:
	  * What is the total amount of debt that is owed by the countries listed in the dataset?
	  * Which country owns the maximum amount of debt and what does that amount look like?
	  * What is the average amount of debt owed by countries across different debt indicators?

The data used in this project is provided by The World Bank. 
It contains both national and regional debt statistics for several countries across the globe as recorded from 1970 to 2015.
[Source: DataCamp]


PbSnTe alloys (Pb_1-x Sn_x Te)
==========================

Current status
--------------

- Quantum Espresso PBEsol calculations:
    - Structure has been optimized.
    - Experimental volumen at room temperature has been used.
    - Electronic band structure calculated.
    - Virtual Crystal Approximation (VCA) electronic band structure of 
      Pb0.5Sn0.5Te calculated. 
    - Energy cutoff 90Ry.
    - Spin-orbit coupling included.

Electronic structure results:
--------------

- First, I have calculated the electronic band structures of SnTe and PbTe using their optimized lattice 
constants. Note that, pbesol does not work well for PbTe: bandgap at L underestimated, 
being the fundamental gap indirect (maximum of the valence band located at Sigma).


- Secondly, I have calculated the electronic band structures of SnTe and PbTe using experimental volumen at 
room temperature, along with the Pb0.5Sn0.5Te alloy. This time, PbTe exhibits a direct bandgap
(underestimated), and effective masses do not look right. Just as an exercise to test VCA calculations in Quantum Espresso,
 I have used the experimental volumen for a 50/50 alloy.



- Based on these preliminary results: it is possible to create a VCA pseudopotential in Quantum Espresso. 
We should continue searching for a good description of the electronic band structure of PbTe allowing us
to include spin-orbit (as for SnTe), and then we can use that VCA BS for an electron-phonon calculation
 using EPW code, for instance.

