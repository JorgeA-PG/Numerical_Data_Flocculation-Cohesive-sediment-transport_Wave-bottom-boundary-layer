# Data_Flocculation-Cohesive-sediment-transport_Wave-bottom-boundary-layer

<p style="text-align: justify;">
The folder “ModelingFrameworkResults” contains the data and results presented in the scientific paper “A Numerical Modeling Framework for Flocculation and Cohesive Sediment Transport in the Wave Bottom Boundary Layer.” The results are categorized based on the initial profile cases: high constant settling velocity (C1, C2, and C3) and low constant settling velocity (C4, C5, and C6).

<p style="text-align: justify;">
For each case “C”, there is a folder named “InitialProfiles”, which contains 4 input files to run the modeling framework as:

* d_x3.mat 	=	vertical grid points [m]
* dGsed.mat =	wave-period-averaged turbulent shear rate profile [s^{-1}]
* Kt.mat 	  =	turbulent diffusivity [m^{2} s^{-1}]
* Tav_MassC =	wave-period-averaged sediment concentration [kg m^{-3}]

<p style="text-align: justify;">
Additionally, there are three folders corresponding to cases associated with cohesive floc properties (r= [2.5, 5.0, 10.0]). Inside each folder, the number of subfolders varies depending on the iterations required to reach equilibrium. For example, the directory “\Cases_C1_C2_C3\C3\r_10.0\” contains a folder labeled “Iter_4”, indicating that equilibrium was achieved after four iterations. Each iteration folder contains six files, described as follows:

* MassConFlocsEq.mat 	=	concentration profile for each floc size at equilibrium
* Tav_MassC 			    =	sediment concentration [kg m^{-3}] 
* tfloc 				      = 	Printed time array [min]
* wav_d.mat 			    =	weight-averaged floc size [m]
* wav_fdens.mat		    =	weight-averaged floc density [kg m^{-3}]
* wav_ws.mat 			    = 	weight-averaged floc settling velocity [m s^{-1}]
