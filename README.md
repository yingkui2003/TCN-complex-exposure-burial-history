# TCN complex exposure-burial history simulation tool
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

The second tool is a simple climate proxy curve test result for an exposure age when the sample experienced repreated ice covers. Th interface is below:

<img width="402" height="429" alt="image" src="https://github.com/user-attachments/assets/1438b3b8-0972-4f22-95be-ca1ce1dff6c6" />

The input parameters include: a climate proxy curve (record), an exposure age, and then if run the cut test of the climate curve by the first cut age or a cutoff value. The tool will then determine the total exposure and burial ages based on these parameters. Below is one example:
<img width="408" height="430" alt="image" src="https://github.com/user-attachments/assets/890c802f-868e-4b68-a09e-b16926d6f4b3" />

This exe file also includes some other general cosmogenic nuclide related tools:
<img width="214" height="144" alt="image" src="https://github.com/user-attachments/assets/3f0bd3e8-516a-4d82-93f6-e163bd3b0ac1" />

However, with the continous updates, most of these tools are out dated, except for the thickness correction and shielding factor. In particular, the shielding factor was designed to derive the topographic shielding factor based on a set of measured azimuth and elevation angle pairs, as well as the Dip and strike values. 
<img width="398" height="442" alt="image" src="https://github.com/user-attachments/assets/e334e116-0f2f-48e3-b1fa-168eb414a509" />

The ArcGIS version of the topographic shielding factors can be founded in the Github page https://github.com/yingkui2003/Area-shielding for an area and https://github.com/yingkui2003/topo-shielding for individual samples.

# Cite this work
Li, Y., Fabel, D., Stroeven, A.P., Harbor, J., 2008. Unraveling complex exposure-burial histories of bedrock surfaces under ice sheets by integrating cosmogenic nuclide concentrations with climate proxy records. Geomorphology 99, 139–149. https://doi.org/10.1016/j.geomorph.2007.10.010

# Contact info
Yingkui Li

Department of Geography & Sustainability

University of Tennessee

Knoxville, TN 37996

Email: yli32@utk.edu

Website: https://geography.utk.edu/about-us/faculty/dr-yingkui-li/

Google Scholar: https://scholar.google.com/citations?user=JoNuyCMAAAAJ&hl=en&oi=ao




