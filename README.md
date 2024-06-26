LAB_EXPERIMENT_6

SCHEMATIC ENTRY AND SIMULATION OF CMOS INVERTER, CMOS NAND and CMOS NOR USING CADENCE TOOL

AIM: To design and simulate the CMOS inverter and observe the DC and transient responses using cadence tool.

APPARATUS REQUIRED:

1.Laptop with MobaXterm
2.Cadence tool PROCEDURE SCHEMATIC ENTRY: Creating a new library:
3.In the library manager, execute File - New library. The new library form appears.
4.In the new library form, type ‘my design lib’ in the name section.
5.In the field of directory section, verify that the path to the library is set to ~/Database / Cadence- analog – lab –bl3 and click ok.
6.In the next ‘technology file for new library form select option attach to an existing tech file and click ok.
7.In the ‘attach design library to technology file’ form, select gpdk045 form the cyclic field and click ok.
8.After creating a new library you can verify it from the library manager.
9.If you right click on the ‘my design lib’ and select properties, you will find that gpdk045 library is attached as techlib to ‘my design lib’.

Creating a schematic cell view:

1.In the CIW or library manager, execute file – new – cell viw.
2.Setup the new file form as follows, Do not edit the library path file and the above might be different from the path shown in your form.
3.Click ok when done the above setting. A black schematic window for the inverter design appears.

Adding components to schematic:

1.In the inverter schematic window, click the instance fixed menu icon to display the add instance form.
2.Click on the browse button. This opens up a library browser from which you can select components and the symbol view.
3.After you complete the add instance form move your cursor to the schematic window and click left to place a component. LIBRARY NAME CELL NAME gpdk045 PMOS gpdk045 NMOS
4.This is a table of components for building the inverter schematic.
5.After entering components, click cancel in the add instance form or press ESC with your cursor in the schematic window.

![image](https://github.com/devasrimathi2004/VLSI-LAB-EXP-6/assets/166363441/0d1f7cc8-a424-4b97-a515-023b32a7cc6d)

Adding pins to schematic:

6.Click the pin fixed menu icon in the schematic window. You can execute create pin or press ‘p’.
7.Add pin form appears. Type the following in the ADD pin form in the next order leaving space between the pin. PIN NAMES DIRECTION Vin,Vdd,Vss Input Vout Output
8.Select cancel and then the schematic window enter window file or press the f bind key. Adding wires to schematic:
9.Click the wire (narrow) icon in the schematic window.
10.In the schematic window click on a pin of one of your components as the first point for your wiring. A diamond shape appears over the starting point of this wire.
11.Follow the prompts at the bottom of design window and click left on the destination point for your wire. A wire is routed between the source and destination points.
12.Complete the wiring as shown in the figure and when done wiring press ECS key in the schematic window to cancel wiring.

Saving the design: Click the check and save icon in the schematic editor window observe CIW output for any errors.

BUILDING THE INVERTER TEST DESIGN: Creating the inverter test cell view:

1.In the CIW or library manager, execute file – new – cell view.
2.Setup the newfile as shown below.
3.Click ok when done. A blank schematic window for the inverter test design appears.
4.Using the components list and properties/ comments in this table build the inverter test schematic. LIBRARY NAME CELL VIEW NAME PROPERTIES/COMMENTS My design lib Inverter Symbol Analog lib Vpulse Voltage1 = 0, Voltage2 = 1.8, delay Time = 0, Rise time=Fall time=1ns Period=20ns Analog lib Vdc, gnd Vdc = 1.8v
5.Add the above components using create – instance or by pressing I.
6.Click the wire (narrow) icon and wire your schematic.
7.Click create wire name or press c to name the i/p (vsin) and output wires as in below schematic.
8.Click on the check and save icon to save the design.

![image](https://github.com/devasrimathi2004/VLSI-LAB-EXP-6/assets/166363441/aa177665-a84b-4225-b929-b7c83fe90ce9)

ANALOG SIMULATION WITH SPECTRA: Starting the simulation environment:

9.In the Inverter-test schematic window execute launch – ADEL. The variable virtuoso analog design environment (ADE) simulation window appears. Choosing a simulator:
10.In the simulation window (ADE) execute setup – simulator / directory / host.
11.In the choosing simulator form, set the simulator field to specra and click ok.
12.In the simulation window (ADE) execute the setup model libraries. To complete, move the cursor and click ok. Choosing Analysis:
13.Click the choose- Analysis icon in the simulation window (ADE).
14.The choosing analysis form appears.
15.To Setup the transient analysis. a. In the analysis section select tron. b. Set the stop time as 100ns c. Click at the moderate or enabled button and the bottom and then click apply.
16.To set for DC analysis a. In the analysis section select DC. b. Turn on save DC operating point. c. Turn on the component parameters. d. Double click the select Vpulse source or Type V0 (capital V zero). e. Select the DC voltage in the select window parameter and click in the form start and stop voltages are 0 to 1.8. f. Select the enable button and click apply and then click ok.

Selecting output for plotting:

1.Execute the o/p’s to be plotted -select on sschematic in the simulation window.
2.Follow the prompt at the bottom. Click on the o/p net vout input vin of the inverter. Press esc with the cursor after selecting.

Running the simulation:

1.Execute the simulation Netlist and run in the simulation window to start the simulation on the icon. This will create the netlist as well as run the simulation.
2.When the simulation finishes the transient and DC plots automatically will be popped up along with netlist.

![image](https://github.com/devasrimathi2004/VLSI-LAB-EXP-6/assets/166363441/bb83d164-f80a-499c-89ba-f08db0697639)

![image](https://github.com/devasrimathi2004/VLSI-LAB-EXP-6/assets/166363441/87cc296e-7929-4ddd-acf6-ec469a761f6a)

CMOS NAND GATE NAND SCHEMATIC

![image](https://github.com/devasrimathi2004/VLSI-LAB-EXP-6/assets/166363441/9e3d8de5-9309-482e-8242-e841c36d3229)

NAND TEST CELL VIEW

![image](https://github.com/devasrimathi2004/VLSI-LAB-EXP-6/assets/166363441/0e328d7d-29f4-4ce7-8212-1639de5a9986)

NAND SIMULATION WITH SPECTRA

![image](https://github.com/devasrimathi2004/VLSI-LAB-EXP-6/assets/166363441/e7f77819-ea1c-4b9c-ab6a-779ae3e215be)

CMOS NOR GATE NOR SCHEMATIC

![image](https://github.com/devasrimathi2004/VLSI-LAB-EXP-6/assets/166363441/547d1a22-19bc-4b4c-9a51-16fb9889c6c4)

NOR TEST CELL VIEW

![image](https://github.com/devasrimathi2004/VLSI-LAB-EXP-6/assets/166363441/4ff81961-76dc-4e7a-b520-2dad4e8d8a78)

NOR SIMULATION WITH SPECTRA

![image](https://github.com/devasrimathi2004/VLSI-LAB-EXP-6/assets/166363441/a22f7d7a-cc6e-482b-84be-e6e7fb7c140b)



