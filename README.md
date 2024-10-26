# IEEE39system_Frequency-domain
Data set for network reduction for converter-driven stability analysis MDPI Journal paper

Generic IEEE 39 bus system details are taken, and are modified to fit the in house converter model available. 
Therefore, the frequency and the voltage levels in the system are changed.
These excels are given as an input to the frequency domain tool. Using these topology inputs, the tool
models the network in frequency domain, which are then used for stability analysis and network reduction

Below is a brief description of each excel sheet provided:

#Nodes: Bus Ids and the devices connected to the bus Id. If a component is connected, it is '1' else '0'
Except for generators. If generator is connected, then it has the generator inductance, else '0'

#Branches: From and to bus Ids between which branch elements are connected. A generic line length is considered.
Line Types: 	1 - Lines
				2 - Cables
				3 - Transformers
The line length column incase of a transformer line type is filled with a dummy number.

#Loads: The voltage level of the load, active and reactive power demand at the load are given.

#Transformers: Primary and secondary bus Ids between which the transformers are connected. 
Primary and secondary impedance paameters and primary and secondary voltage levels are provided.

#Stability: The bus Ids which are to be considered as PCC for stability analysis, also where 
the converters are connected. The type of the converter is given here.
Type 1: Grid forming
Type 2: Grid following
If the bus is not considered , then the value is 0, else the converter type.

Same network details are taken also for EMT modelling.