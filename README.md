# VLSI-LAB-EXP-6
**SCHEMATIC ENTRY AND SIMULATION OF CMOS INVERTER, CMOS NAND and CMOS NOR USING CADENCE TOOL**

**AIM:**

To design and simulate the CMOS inverter and observe the DC and transient responses using cadence tool.

**APPARATUS REQUIRED:**
 
1.	Laptop with MobaXterm
2.	Cadence tool
	
**PROCEDURE**

**Creating a new library:**
1.	In the library manager, execute File - New library. The new library form appears.
2.	In the new library form, type ‘my design lib’ in the name section.
3.	In the field of directory section, verify that the path to the library is set to ~/Database / Cadence- analog – lab –bl3 and click ok.
4.	In the next ‘technology file for new library form select option attach to an existing tech file and click ok.
5.	In the ‘attach design library to technology file’ form, select gpdk045 form the cyclic field and click ok.
6.	After creating a new library you can verify it from the library manager.
7.	If you right click on the ‘my design lib’ and select properties, you will find that gpdk045 library is attached as techlib to ‘my design lib’.

**Creating a schematic cell view:**

1.	In the CIW or library manager, execute file – new – cell viw.
2.	Setup the new file form as follows, Do not edit the library path file and the above might be different from the path shown in your form.
3.	Click ok when done the above setting. A black schematic window for the inverter design appears.

**Adding components to schematic:**

1.	In the inverter schematic window, click the instance fixed menu icon to display the add instance form.
2.	Click on the browse button. This opens up a library browser from which you can select components and the symbol view.
3.	After you complete the add instance form move your cursor to the schematic window and click left to place a component.
4.	This is a table of components for building the inverter schematic.
5.	After entering components, click cancel in the add instance form or press ESC with your cursor in the schematic window.

 ![329845465-ff2e4de9-cd56-4227-8ce4-c9887921b4f2](https://github.com/Jayanth-T/VLSI-LAB-EXP-6/assets/106177371/415fd11e-87b9-4748-b8c4-101ea8aa4ccb)


**Adding pins to schematic:**

1.	Click the pin fixed menu icon in the schematic window. You can execute create pin or press ‘p’.
2.	Add pin form appears. Type the following in the ADD pin form in the next order leaving space between the pin.
3.	Select cancel and then the schematic window enter window file or press the f bind key.
   
**Adding wires to schematic:**

1.	Click the wire (narrow) icon in the schematic window.
2.	In the schematic window click on a pin of one of your components as the first point for your wiring. A diamond shape appears over the starting point of this wire.
3.	Follow the prompts at the bottom of design window and click left on the destination point for your wire. A wire is routed between the source and destination points.
4.	Complete the wiring as shown in the figure and when done wiring press ECS key in the schematic window to cancel wiring.

Saving the design:
	Click the check and save icon in the schematic editor window observe CIW output for any errors.

**BUILDING THE INVERTER TEST DESIGN:**

Creating the inverter test cell view:
1.	In the CIW or library manager, execute file – new – cell view.
2.	Setup the newfile as shown below.
3.	Click ok when done. A blank schematic window for the inverter test design appears.
4.	Using the components list and properties/ comments in this table build the inverter test schematic.
5.	Add the above components using create – instance or by pressing I.
6.	Click the wire (narrow) icon and wire your schematic.
7.	Click create wire name or press c to name the i/p (vsin) and output wires as in below schematic.
8.	Click on the check and save icon to save the design.
 
![329845717-4bf6bbe3-c876-45b8-8d0c-681a2591aa43](https://github.com/Jayanth-T/VLSI-LAB-EXP-6/assets/106177371/dfc84476-6f8f-4314-8968-8e35f9baadaa)


**ANALOG SIMULATION WITH SPECTRA:**

Starting the simulation environment:
1.	In the Inverter-test schematic window execute launch – ADEL. The variable virtuoso analog design environment (ADE) simulation window appears.
Choosing a simulator:
1.	In the simulation window (ADE) execute setup – simulator / directory / host.
2.	In the choosing simulator form, set the simulator field to specra and click ok.
3.	In the simulation window (ADE) execute the setup model libraries.
To complete, move the cursor and click ok.
Choosing Analysis:
1.	Click the choose- Analysis icon in the simulation window (ADE).
2.	The choosing analysis form appears.
3.	To Setup the transient analysis.
a.	In the analysis section select tron.
b.	Set the stop time as 100ns
c.	Click at the moderate or enabled button and the bottom and then click apply.
4.	To set for DC analysis
a.	In the analysis section select DC.
b.	Turn on save DC operating point.
c.	Turn on the component parameters.
d.	Double click the select Vpulse source or Type V0 (capital V zero).
e.	Select the DC voltage in the select window parameter and click in the form start and stop voltages are 0 to 1.8.
f.	Select the enable button and click apply and then click ok.

**Selecting output for plotting:**

1.	Execute the o/p’s to be plotted  -select on sschematic in the simulation window.
2.	Follow the prompt at the bottom. Click on the o/p net vout input vin of the inverter. Press esc with the cursor after selecting.

**Running the simulation:**

1.	Execute the simulation Netlist and run in the simulation window to start the simulation on the icon. This will create the netlist as well as run the simulation.
2.	When the simulation finishes the transient and DC plots automatically will be popped up along with netlist.
 
![329919607-8f23fb7a-a50c-494c-ad5b-769714302e05](https://github.com/Jayanth-T/VLSI-LAB-EXP-6/assets/106177371/463edb76-8d13-4994-9cfa-7c6d359ff6fa)
![329919658-9275159c-4a41-4293-b515-5a81cb48a8bb](https://github.com/Jayanth-T/VLSI-LAB-EXP-6/assets/106177371/1dd66bd6-028f-40f0-8301-4273671b23a1)




***CMOS NAND GATE***

**NAND SCHEMATIC**
![329919725-6b7fa53b-da51-464c-9d31-bc1205519f42](https://github.com/Jayanth-T/VLSI-LAB-EXP-6/assets/106177371/cb456d07-a1bf-4ebb-a0c1-f4b1a353132d)




**NAND TEST CELL VIEW**
![329919780-906e4114-3b94-49ba-a5b9-f5ee8b8eb053](https://github.com/Jayanth-T/VLSI-LAB-EXP-6/assets/106177371/a365176e-2d99-45cc-9305-92dbcdce6e3d)


 
**NAND SIMULATION WITH SPECTRA**
![329919880-2609fa42-f131-44ff-b3e0-86b1bc557853](https://github.com/Jayanth-T/VLSI-LAB-EXP-6/assets/106177371/4729050c-9962-4fc6-9daa-250f228d9bbd)




**CMOS NOR GATE**

**NOR SCHEMATIC**
![329845885-3ec2637c-b359-430d-9642-10b92ebfdedb](https://github.com/Jayanth-T/VLSI-LAB-EXP-6/assets/106177371/4961259f-9c5e-4e9b-8a8e-0749bdadaf07)


**NOR TEST CELL VIEW**

![329845904-cd64ffe6-7ddb-47e3-8f66-256e15c62e45](https://github.com/Jayanth-T/VLSI-LAB-EXP-6/assets/106177371/5d0a25b7-9ee1-4784-96be-7cb6425d545f)


**NOR SIMULATION WITH SPECTRA**
![329919976-dcf02536-14ad-45ac-a1a2-fbe89f25c839](https://github.com/Jayanth-T/VLSI-LAB-EXP-6/assets/106177371/e3f08202-49f1-49f3-912f-3b9fac6d1097)




**RESULT:**

The Implementation of CMOS inverter, CMOS NAND and CMOS NOR gate waveforms are verified.
