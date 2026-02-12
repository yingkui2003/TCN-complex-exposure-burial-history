## TCN complex exposure-burial history simulation tool
This tool was developed to simulate the complex exposure burial history based on measured Be and Al concentrations for bedrock/boulder surfaces that experienced the repeated coverages of glaciers or ice sheets. The detailed description of this tool can be found in 
https://www.sciencedirect.com/science/article/abs/pii/S0169555X07004904 or the Geomorphology paper uploaded in this Github page.

This tool was developed by C++. You can download the exe file and run it in Windows by double clicking the downloaded ClimateCurve.exe file. When first runing it, the System may show a warning and just choose run it anyway. The following is the screenshot of the interface of this exe file:

<img width="913" height="588" alt="image" src="https://github.com/user-attachments/assets/6d4fe3ad-5bd4-4693-95d9-97d5713e485d" />

There are two tools under the "ClimateCurve" menu: "Climate Proxy Curve Simulation" and "Climate Proxy Curve Cut Results". The "Climate Proxy Curve Simulation" tool is the major tool for the complex exposure burial history simulation. The following is the interface of this tool:

<img width="511" height="555" alt="image" src="https://github.com/user-attachments/assets/d628c6ba-6183-4595-809c-522857f0fc5c" />
The Input parameters include: 
1) measured Be-10 concentration (atoms/g)
2) Be-10 concentration error (atoms/g)
3) measured Al-26 concentration (atoms/g)
4) Al-26 concentration error (atoms/g)
5) Be-10 production rate at the sample site (atoms/g/yr)
6) Al-26 production rate at the sample site (atoms/g/yr)
7) Rock density (g/cm^3)
8) Free path (attenuation length) (g/cm^2)
9) Potential aerial erosion rate (cm/kyr): this is used to test the maximum allowable erosion rate when ice free
10) Potential Glacial erosion rate (cm/kyr): This is used to test the maximum allowable erosion rate under ice cover
11) Proxy Curve for the simulation (represents the ice cover and free cycles)
12) Output file: to save the simulation results to a txt file that can be used to generate plots and statistics

The simulation results will be showed in the results console box. Note that in this console box only the optimal simulation results are listed. In addtion, additional Monte Carlo simulations are also conducted by changing the Be-10 and Al-26 concentrations with the mearued errors based on normal distrbution. This will provide the potential ranges of exposure and burial durations of the sample site. 

You can click the "Calculation" button to run the simulation, the "Clean" button to clear the results console, the "Save" button to save the console results, and the "Close" button to close the program. By changing the input parameters, you can run multiple simulations for different samples.

This site also includes two climate proxy record (DSDP607.dat and Global_Stack.dat) that can be used for the similation. If you have other climate ptoxy records, you can convert it to the same format to these two files.
The following screenshot shows one example of the simulation:
<img width="506" height="549" alt="image" src="https://github.com/user-attachments/assets/b2f1db78-a239-4dff-bece-73d7e51c840e" />


