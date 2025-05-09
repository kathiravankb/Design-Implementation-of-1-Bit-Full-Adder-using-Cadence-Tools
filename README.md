# Ex No: 05 - DESIGN-IMPLEMENTATION-OF-1-BIT-FULL-ADDER-USING-CADENCE-TOOLS

  
## AIM:

To design and implement a 1-bit full adder circuit using Cadence EDA tools and to understand its behavior in digital arithmetic operations.

## TOOLS REQUIRED: 

•	Personal Computer
•	Cadence Virtuoso Software

S C H E M A T I C S I M U L A T I O N - PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION -Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
•	csh
•	source /cadence/install/cshrc
•	virtuoso
 ###  PROCEDURE FOR SCHEMATIC SIMULATION USING CADENCE :
 
1.	Now two windows must open i) virtuoso/command interpreter window ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window (CIW) for further processing.
i.	Create a New Library
ii.	Create Schematic Cell view.
iii.	Create the Symbol for schematic Cell view.
iv.	Create the test Cell view.
v.	Analog simulation by spectre


i) PROCEDURE FOR CREATING NEW LIBRARY :	

•	File –New – Library
•	Name: Give name for ur library Ex: VLSILAB_EXP_1
•	Enable Attach to an existing technology library, Click OK
•	Attach the library to the technology library gpdk045.Click OK

ii)	CREATE SCHEMATIC CELL VIEW: 

•	Go to 1st window i.e virtuoso (CIW)
•	File-New-Cell view
•	Setup the new file form
	Library: Select the one you created.
	Cell: Give the experiment name Ex: Inverter ViewSchematic
	Type: Schematic press OK
•	Add the required components from the libraries and make the connections.
	Go to instance fixed menu or use shortcut key “I” from keypad to go instances
	Click on browse. This opens the library browser
	Now select the appropriate library for components like 
	Gpdk45 ------------------------nmos1v, pmos1v
	Create Input and Output pins
	Make the connections by using fixed narrow wire key
	Click Check and Save button

![Screenshot 2025-05-08 212048](https://github.com/user-attachments/assets/918875a4-0a39-493f-b9a9-fb9ba9961673)



 
iii)	CREATING THE SYMBOL FOR SCHEMATIC CELL VIEW 

•	In the schematic window, execute 
	Create – Cell view – From Cell view
	The cell view from cell view window appears
	Check Lib Name, Cell Name, From View name must be schematic Press ok
•	Now Symbol generation form appears. Click Ok If No changes required
•	A new window with with default symbol is created.
•	Edit the symbol if you want to give actual symbol shape else continue.
•	Execute Create-Cell view-from cell view
•	Library Name and Cell Name must be same which you have used for schematic. Press OK
•	Check for the position of pin side.Prss OK
•	Edit for the shape by Create-Shape-Choose required options to edit.


![Screenshot 2025-05-08 212113](https://github.com/user-attachments/assets/2308bc52-e8f1-40bf-80d3-f26987246b89)




iv)	CREATING THE NEW TEST CELL VIEW 

•	Go to CIW window, Execute File-New-Cell view
	Setup the new file form
	Library: Select the one you created.
	Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
	View: Schematic
	Type: Schematic press OK
•	Follow the step 3(ii) d to make the required connections


![Screenshot 2025-05-08 212159](https://github.com/user-attachments/assets/aa7e47dc-2e41-4e36-8648-9c5924768055)


 
### ANALOG SIMULATION BY SPECTRE:

•	In test cell view window
•	Launch – ADE L(Analog Design Environment)
	Execute Setup—Simulation/directory/Host A new window opens
	Set the simulation window to spectre and click ok
	Execute Analysis – Choose. A window opens.
	Select the type and set the specifications and press OK
	Execute Output s—to be plotted – Select on Schematic
	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
•	Execute Simulation -- Net list and Run

![Screenshot 2025-05-08 212257](https://github.com/user-attachments/assets/cd4d007e-b295-4d7d-bf30-729cf52978e5)



### FOR TRANSIENT ANALYSIS SETTINGS AND OUTPUT: 
 
![Screenshot 2025-05-08 212325](https://github.com/user-attachments/assets/8c1cf292-a01c-4495-9974-662787cf4197)



 

## RESULTS : 
The design and implementation of the 1-bit full adder using Cadence EDA tools were successfully completed. The simulation results verified the correct operation of the full adder, with accurate sum and carry outputs for all input combinations.
