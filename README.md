# *DIGITAL-VLSI-SOC-DESIGN-AND-PLANNING*
# Contents 
 <div class="toc">
  <ul>
    <li><a href="#header-1">Day 1 - Inception of open-source EDA, OpenLANE and sky130 PDK</a></li>
	<ul>
        <li><a href="#header-1_1"> How to talk to computers</a></li>
		<ul>
			<li><a href="#header-1_1_1">Introduction to QFN-48 Package, chip, pads, core, die and IPs</a></li>
		</ul>
		<ul>
			<li><a href="#header-1_1_2">Introduction to RISC-V</a></li>
		</ul>
		<ul>
			<li><a href="#header-1_1_3">From Software Applications to Hardware</a></li>
		</ul>
            </ul>
      <ul>
	           <li><a href="#header-1_2">Soc design and OpenLANE</a></li>
	      <ul>
			</a></li>
		</ul>
      </ul>
	<ul>
        </a></li>
		<ul>
			</a></li>
		</ul>
		<ul>
			</a></li>
		</ul>
		<ul>
			<li><a href="#header-1_3_3">Review files after design prep and run synthesis</a></li>
		</ul>
	      <ul>
			<li><a href="#header-1_3_4">OpenLANE Project Git Link Description</a></li>
		</ul>
		<ul>
			<li><a href="#header-1_3_5">Steps to characterize synthesis results</a></li>
		</ul>
      </ul>
   </div>
  
<div class="toc">
  <ul>
    <li><a href="#header-2">Day 2 - Good floor planning considerations</a></li>
	<ul>
        <li><a href="#header-2_1"> Chip Floor planning consideration</a></li>
		<ul>
			<li><a href="#header-2_1_1">Utilization factor and aspect ratio</a></li>
		</ul>
		<ul>
			<li><a href="#header-2_1_2">Concept of pre-placed cells</a></li>
		</ul>
		<ul>
			<li><a href="#header-2_1_3">De-coupling capacitors</a></li>
		</ul>
	      <ul>
			<li><a href="#header-2_1_4">Power planning</a></li>
		</ul>
		<ul>
			<li><a href="#header-2_1_5">Pin placement and logical cell placement blockage</a></li>
		</ul>
		<ul>
			<li><a href="#header-2_1_6">Steps to run floorplan using OpenLANE</a></li>
		</ul>
		<ul>
			<li><a href="#header-2_1_7">Review floorplan files and steps to view floorplan/a></li>
		</ul>
	      <ul>
		      <li><a href="#header-2_1_8">Review floorplan layout in Magic</a></li>
		</ul>
      </ul>
      <ul>
        <li><a href="#header-2_2">Library building and Placement</a></li>
	      <ul>
			<li><a href="#header-2_2_1">Netlist binding and initial place design</a></li>
		</ul>
		<ul>
			<li><a href="#header-2_2_2">Optimize placement using estimated wire-length and capacitance</a></li>
		</ul>
		<ul>
			<li><a href="#header-2_2_3">Final placement optimization</a></li>
		</ul>
	      <ul>
			<li><a href="#header-2_2_4">Need for libraries and characterization</a></li>
		</ul>
		<ul>
			<li><a href="#header-2_2_5">Congestion aware placement using RePlAce</a></li>
		</ul>
      </ul>
	<ul>
        <li><a href="#header-2_3">Cell design and characterization flows</a></li>
		 <ul>
			<li><a href="#header-2_3_1">Inputs for cell design flow</a></li>
		</ul>
		<ul>
			<li><a href="#header-2_3_2">Circuit design steps</a></li>
		</ul>
		<ul>
			<li><a href="#header-2_3_3">Layout design step</a></li>
		</ul>
	      <ul>
			<li><a href="#header-2_3_4">Typical characterization flow</a></li>
		</ul>
      </ul>
	  <ul>
        <li><a href="#header-2_4">General timing characterization parameters</a></li>
		   <ul>
			<li><a href="#header-2_4_1"> Timing threshold definitions</a></li>
		</ul>
		<ul>
			<li><a href="#header-2_4_2">Propagation delay and transition time</a></li>
		</ul>
      </ul>
</div>
  
  <div class="toc">
  <ul>
    <li><a href="#header-3">Day 3 - Design library cell using Magic Layout and ngspice characterization</a></li>
	<ul>
        <li><a href="#header-3_1"> Labs for CMOS inverter ngspice simulations</a></li>
		<ul>
			<li><a href="#header-3_1_0">IO placer revision</a></li>
		</ul>
		 <ul>
			<li><a href="#header-3_1_1">SPICE deck creation for CMOS inverter</a></li>
		</ul>
		<ul>
			<li><a href="#header-3_1_2">SPICE simulation lab for CMOS inverter</a></li>
		</ul>
		<ul>
			<li><a href="#header-3_1_3"> Switching Threshold Vm</a></li>
		</ul>
	      <ul>
			<li><a href="#header-3_1_4">Static and dynamic simulation of CMOS inverter</a></li>
		</ul>
		<ul>
			<li><a href="#header-3_1_5">Lab steps to git clone vsdstdcelldesign</a></li>
		</ul>
      </ul>
      <ul>
        <li><a href="#header-3_2">Inception of layout ̂A CMOS faabrication process </a></li>
		 <ul>
			<li><a href="#header-3_2_1">Create Active regions</a></li>
		</ul>
		<ul>
			<li><a href="#header-3_2_2">Formation of N-well and P-well</a></li>
		</ul>
		<ul>
			<li><a href="#header-3_2_3"> Formation of gate terminal</a></li>
		</ul>
	      <ul>
			<li><a href="#header-3_2_4">Lightly doped drain (LDD) formation</a></li>
		</ul>
		<ul>
			<li><a href="#header-3_2_5">Source ÃÂ drain formation</a></li>
		</ul>
  		<ul>
			<li><a href="#header-3_2_6">Local interconnect formation</a></li>
		</ul>
		<ul>
			<li><a href="#header-3_2_7"> Higher level metal formation</a></li>
		</ul>
	      <ul>
			<li><a href="#header-3_2_8"> Lab introduction to Sky130 basic layers layout and LEF using inverter</a></li>
		</ul>
		<ul>
			<li><a href="#header-3_2_9">Lab steps to create std cell layout and extract spice netlist</a></li>
		</ul>
      </ul>
	<ul>
        <li><a href="#header-3_3">Sky130 Tech File Labs</a></li>
		<ul>
			<li><a href="#header-3_3_1">Lab steps to create final SPICE deck using Sky130 tech</a></li>
		</ul>
		<ul>
			<li><a href="#header-3_3_2">Lab steps to characterize inverter using sky130 model files</a></li>
		</ul>
		<ul>
			<li><a href="#header-3_3_3"> Lab introduction to Magic tool options and DRC rules</a></li>
		</ul>
	      <ul>
			<li><a href="#header-3_3_4">Lab introduction to Sky130 pdk's and steps to download labs</a></li>
		</ul>
		<ul>
			<li><a href="#header-3_3_5">Lab introduction to Magic and steps to load Sky130 tech-rules</a></li>
		</ul>
  		<ul>
			<li><a href="#header-3_3_6">Lab exercise to fix poly.9 error in Sky130 tech-file</a></li>
		</ul>
		<ul>
			<li><a href="#header-3_3_7"> Lab exercise to implement poly resistor spacing to diff and tap</a></li>
		</ul>
	      <ul>
			<li><a href="#header-3_3_8"> Lab challenge exercise to describe DRC error as geometrical construct</a></li>
		</ul>
		<ul>
			<li><a href="#header-3_3_9">Lab challenge to find missing or incorrect rules and fix them</a></li>
		</ul>
      </ul>
   </div>
	  
<div class="toc">
  <ul>
    <li><a href="#header-4">Day 4 - Pre-layout timing analysis and importance of good clock tree</a></li>
	<ul>
        <li><a href="#header-4_1">Timing modeling using delay tables</a></li>
		 <ul>
			<li><a href="#header-4_1_1">Lab steps to convert grid info to track info</a></li>
		</ul>
		<ul>
			<li><a href="#header-4_1_2">Lab steps to convert magic layout to std cell LEF</a></li>
		</ul>
		<ul>
			</a></li>
		</ul>
	      <ul>
			</a></li>
		</ul>
		<ul>
			</a></li>
		</ul>
		<ul>
			</a></li>
		</ul>
		<ul>
			<li><a href="#header-4_1_7">Lab steps to configure synthesis settings to fix slack and include vsdinv</a></li>
		</ul>
      </ul>
      <ul>
        </a></li>
	       <ul>
			</a></li>
		</ul>
		<ul>
			</a></li>
		</ul>
		<ul>
			<li><a href="#header-4_2_3">Lab steps to configure OpenSTA for post-synth timing analysis</a></li>
		</ul>
	      <ul>
			<li><a href="#header-4_2_4">Lab steps to optimize synthesis to reduce setup violations</a></li>
		</ul>
		<ul>
			<li><a href="#header-4_2_5">Lab steps to do basic timing ECO</a></li>
		</ul>
      </ul>
	<ul>
        <li><a href="#header-4_3">Clock tree synthesis TritonCTS and signal integrity</a></li>
		  <ul>
			</a></li>
		</ul>
		<ul>
			</a></li>
		</ul>
		<ul>
			<li><a href="#header-4_3_3">Lab steps to run CTS using TritonCTS</a></li>
		</ul>
	      <ul>
			<li><a href="#header-4_3_4">Lab steps to verify CTS runs</a></li>
		</ul>
      </ul>
	  <ul>
        <li><a href="#header-4_4">Timing analysis with real clock using openSTA</a></li>
		  <ul>
			</a></li>
		</ul>
		<ul>
			</a></li>
		</ul>
		<ul>
			<li><a href="#header-4_4_3">Lab steps to analyze timing with real clocks using OpenSTA</a></li>
		</ul>
	      <ul>
			<li><a href="#header-4_4_4">Lab steps to execute OpenSTA with right timing libraries and CTS assignment</a></li>
		</ul>
		<ul>
			<li><a href="#header-4_4_5">Lab steps to observe impact of bigger CTS buffers on setup and hold timing</a></li>
		</ul>
      </ul>
</div>
	
<div class="toc">
  <ul>
    <li><a href="#header-5">Day 5 -Final step for RTL2GDS using tritinRoute and openSTA</a></li>
	<ul>
        </a></li>
		<ul>
			</a></li>
		</ul>
		<ul>
			</a></li>
		</ul>
		<ul>
			<li><a href="#header-5_1_3">Design Rule Check</a></li>
		</ul>
      </ul>
      <ul>
        <li><a href="#header-5_2">Power Distribution Network and routing</a></li>
	      <ul>
			<li><a href="#header-5_2_1">Lab steps to build power distribution network</a></li>
		</ul>
		<ul>
			<li><a href="#header-5_2_2">Lab steps from power straps to std cell power</a></li>
		</ul>
		<ul>
			<li><a href="#header-5_2_3">Basics of global and detail routing and configure TritonRoute</a></li>
		</ul>
      </ul>
	<ul>
        <li><a href="#header-5_3">TritonRoute Features</a></li>
		<ul>
			<li><a href="#header-5_3_1">TritonRoute feature 1 - Honors pre-processed route guides</a></li>
		</ul>
		<ul>
			<li><a href="#header-5_3_2">TritonRoute Feature2 & 3 - Inter-guide connectivity and intra- & inter-layer routing</a></li>
		</ul>
		<ul>
			<li><a href="#header-5_3_3">TritonRoute method to handle connectivity</a></li>
		</ul>
	      <ul>
			<li><a href="#header-5_3_4">Routing topology algorithm and final files list post-route</a></li>
		</ul>
      </ul>


	
<div class="toc">
  <ul>
    <li><a href="#header-6">References</a></li>
  </ul>
</div>

<div class="toc">
  <ul>
    <li><a href="#header-7">Acknowledgement</a></li>
  </ul>
</div>

# <h1 id="header-1">Day 1 -Inception of open-source EDA, OpenLANE and sky130 PDK</h1>	 
## <h1 id="header-1_1">How to talk to computers?</h1>
### <h1 id="header-1_1_1">Introduction to QFN-48 Package, chip, pads, core, die and IPs</h1>

**Arduino Board**:- Here We take example of Arduino board.
Here we learn designing of chip from abstract level by RTL to GDSLL. The area which is in yellow circle as shown in below figure is called as chip.This chip is used for joining all other components of the board.

![image](/assets/1.jpg )

#### Components of Chip
(1) **Pads:** This Area is used for passing the signal from inside to outide or vice versa from the chip.

(2) **Core:** This Area is used for placing the logic gates.

(3) **Die:** it represents the size of the entire chip which is present at the corner.
![image](/assets/2.jpg)
Here we see the example of  RISC-V SoC**:- It consist elments of SRAM,SOC,ADC,DAC,PLL,SPI.The componets PLL, SRAM, ADC , DAC  are called foundary IP's.
    ![image](/assets/3.jpeg)



<h1 id="header-1_1_2"> RISC-V</h1>
RISC-V, It is language of the computer used to talk with computer .Here I explain the name abbreviation where five refers to the number of generations of RISC architecture that were developed at the University of California, Berkeley. Chip is placed in the middle as shown in the figure and this is connected to all other components by wiring as shown in the figure below. 

![Image](/assets/4.jpg)

For Example we have a c program as shown in below figure and it should be run on a computer layer as shown in figure . First the c program is complied into its assemply Language then converted into machine language program i.e binary language which will understand by the hardware of the computer and these bits excute in the harware layer as shown in the figure and gives result.
 
![Image](/assets/5.jpeg)


### <h1 id="header-1_1_2"> Software Applications to Hardware</h1>
When you open the app It undergoes the below process:

Here it  involves three stages as shown below 
Application Software - System Software - Hardware chip.

The process when you open App it enters into system software block where in this block the entier prgram converts into machine language program i.e binary language  and runs on the Hardware block.

![Image](/assets/6.jpeg)

There are three layers inside the system software which are as follows

**Operating System, Compiler, Assembler**

 Operating system : It handles input/output (IO) operations and it allocate memory and it also manage the low level system functions.

 Compiler:It converts the operating system's output i.e in the form of C, C++, and Java output into instructions. The type of hardware determines these instructions.

 Assembler :It take the instructions from compiler. Translate the compiler's instructions into the corresponding binary numbers. Now that this binary language has been sent to the hardware, the hardware generates an output according to the function it has received.
 


 ![image](/assets/7.jpg)
 

 ## <h1 id="header-1_2">Soc design and OpenLANE</h1>
### <h1 id="header-1_2_1">Introduction to all components of open-source digital asic design</h1>
For designing Digital ASIC Design ,tools or things which are required These are namely 
RTL IP's
EDA tools
PDK data

RTL design:
It stands for register-transfer level.It is a design abstraction that represents the logical operations carried out on digital signals and the flow of digital signals (data) between hardware registers in a synchronous digital circuit.There are a lot of open sources available for this design. such as github.com, librecores.org, opencores.org, etc.

 EDA tools: It stands for Electronic Design Automation (EDA) which means it describes the instruments used in the design and validation of printed circuit boards (PCBs), integrated circuits (ICs), and electronic systems in general. Numerous open source tools, such as Qflow, OpenROAD, OpenLANE, etc., are accessible.

**What is PDK Data?**
PDK Stand for process design kit. It is interface between FAB and design. This data is collections of files like,




## <h1 id="header-1_3">Get familiar to open-source EDA tools</h1>
### <h1 id="header-1_3_1">OpenLANE Directory structure in detail</h1>
** Here are some Basic Linux Commands**

**cd** : It stand for change directory.

**cd ..** : It is used for coming out of the folder.

**ls** : lists the content of the folder

**pwd** : It shows the present working directory

**less** : It is used for displaying the content in the file.

**command --help** : shows the complete use of the  command

**clear** : clears the terminal screen

We are using the Sky130_fd_sc_hd PDK variant for this project. where "sky130" denotes the node or process name.The foundary name "fd" is for the SkyWater foundary."hd" refers for high density (essentially one type of variable), and "sc" stands for standard cell librery files.

Numerous technology files, including verilog, spice, techlef, meglef, mag, gds,cdl,lib,lef, etc., are present in the Sky130_fd_sc_hd variant (the techlef file includes the layer information).


### <h1 id="header-1_3_2">Design Preparation Step</h1>
Here we work with OpenLane and We use flow.tcl to know flow of the process as shown in below figure and it is followed by interactive command which is used to know the step by step process. with out interactive function it will undergoes the complete from RTL to GDSII.The command is ``` ./flow.tct -interactive```. After executing the command the terminal changes to as shown in below figure


![image](/assets/8.jpg)

Once the you see the Open Lane in blue colour the next step is install the required packages to execute the flow.The command we use for install the package is ```package require openlane 0.9```


![image](/assets/9.jpg)
 
After the package install the next step is Design setup .
The  command is ``` prep -design picorv32a ``` Here we work on picorv32a design file so we mentioned the file name .

![image](/assets/10.jpg)

After executing the design command it is shown that preparation is completed as shown in below figure .

![image](/assets/11.jpg)

### <h1 id="header-1_3_3">Review files after design prep and run synthesis</h1>

Following preparation, the run directory is generated in the picorv32a file. The date for today is created inside the folder. The run folder is empty as we didnt run the sythesis.In run folder there are two files namely result and report.

![image](/assets/12.jpg)


The next is to run the synthesis, The command is ```run_synthesis``` It will take 3-4 mnts to run the synthesis and finally synthesis will completed.

![image](/assets/13.jpg)



### <h1 id="header-1_3_5">Steps to characterize synthesis results</h1>

Ater the sythesis is generated our main objective is calculate the flop ratio.

From the data synthesised , we can know the total number of  D_flip-flops is 1613. and the number of cells is 14876.The flop ratio = (number of flip flops)/(number of total cell). It is 10.84% as shown in figure.

![image](/assets/14.jpg) 



Ater run,  we can see that all the mapping have been done.

![image](/assets/15.JPG)

We can also see when the actual synthesis was completed in the report. and the real statistics synthesis report, which is identical to what we have previously seen, is displayed below.

![image](/assets/16.JPG)


# <h2 id="header-2">Day 2 - Good floor planning considerations</h2>	 
## <h2 id="header-2_1">Chip Floor planning consideration</h2>
### <h2 id="header-2_1_1">Utilization factor and aspect ratio</h2>

We shall attempt to conceal Core and Die's width and height in this section. Determining the width and height is the initial stage in the physical design flow.
![image](/assets/heightandwidth.jpeg)

 Let's begin with a netlist, Consider two flipflops i.e launch flop and capture flop and have a simple combination logic in between. A netlist describes the connectivity of all the components or an elctronic design. Here, we dependent on the dimensions of the logic gates(AND & OR) and particular flipflop. 

 ![image](/assets/flipflop.PNG)

 Now, let's convert the symbols into physical dimensions. We are interested in the dimensions of the Core and Die not in the dimensions of the wires. 

Let's the dimensions of standard cell 1unit*1unit and area= 1 Sq. units and also assume same area for the flipflops too.
with help of these dimensions and netlist let's calculate the area occupied by the netlist on a silicon wafer.

![image](/assets/17.jpeg)

Before that, every wire will be cut, bringing every flip flop and logic gate onto a single plate. Therefore, after adding them together, the width and length will each be 2  units, and the total area will come out to be 4 square units. Thus, we now have an approximate estimate of the smallest space that the netlist takes up.

![image](/assets/18.PNG)

 'Core' and 'Die' section of a chip:

Lets us consider a silicon wafer  on which we implement the logics. The small square inside the silicon wafer is called Die and inside the Die it consits of core section.

A **Die** which consists of core, is small semicondcutor material  specimen on which the fundamental circuit is fabricated.

A '**Core** is the section of the chip where the fundamental logic of the design is placed.



Now, Let's try to place that particular logic inside the core. The netlist will occupy the complete  area inside the core which means it utilizes the core 100%. From this we can calculate the utilisation factor which is given by,

        Utilization Factor = Area occupied by netlist / Total area of the core
  
     lets put the dimensions we have, we get
     
     Utilization factor = 4*1sq.unit / 2unit *2unit
     
		= 4sq unit /  4sq unit

So, utilization factor = 1 (which means core is completely occupied all the area and no spane left)

![image](/assets/19.jpg)

Aspect Ratio = Height /  width =  2 unit /  2unit =  1

Whenever ,
Aspect Ratio = 1 it signifies that chip is square shaped. 
Aspect Ratio != 1 it means the chip is in rectangular shape.

![image](/assets/20.PNG)

For example, Lets take another dimensions of the width= 4unit and height = 2unit. So from the above formula of utilization factor we it equal to 0.5 which means the core is not completely utilised it has space in it and aspect ratio is also 0.5  which means the chip is rectangular in shape.

![image](/assets/21.jpg)



**Define locations of Preplaced Cells**:-  Lets take a combinational logic which performs some amount of function and assume its does a big task such that the output is huge circuit having some N Logic gates so let's devide it into some small numbers of gates. We will cut the whole circuit into two parts, and separate both of them into two blocks and both block will be seperately as shown in the below figure.This two boxes are implemented seperately.

![image](/assets/22.PNG)

In both the blocks lets extend the input output pins and now we will black box the boxes and detached them. After black boxing, the upper portion is invisible from the top or invisible to the one , who is looking into the main netlist. now will seperate them out as two different IP's or modules.

![image](/assets/23.PNG)

Advantage of doing this is we can reuse them multiple times after implimenting once only. Similary there are other IP's also available for eg. Memory, Clock-gating cell, Comporator, MUX  all of these are part of the top level netlist.They recieve some input signals and perform functions and deliver the outputs but the functionality of the cell is implemented only once.
 The arrangement of these IP's in a chip is refferd as **floorplanning**.
These IP's have user-defined locations, and hence are placed in chip before automated placement and routing are called **"pre-placed cells"**. 
These cells are placed in such a way that, the placement and routing tool do not touch the location of the cell.


### <h2 id="header-2_1_3">De-coupling capacitors</h2>

**surround pre-placed cells with Decoupling capacitor**:- Let consider some circuit, which is the part of the blocks which has been described earlier. When some gate (let consider AND gate) switched from Logic0 to logic1 or 1 to 0,there is amount of current demand as it need  basically  this capacitor should be completely charged to represent logic 1 and amount of charge is dupplied from the  supply voltage VSS and when ever any gate switches from logic 1 to logic 0 the VSS is responsible for collecting back the charge (completly discharged to represent logic 0). Consider capacitance to be 0. Rdd,Ldd,and Lss are well defoned values. During switvhing operation, the circuit demands switching current i.e. peak current. Now, due to the presence of Rdd and Ldd, there will be a voltage drop across them and the voltage at Node 'A' would be Vdd' instead of Vdd.

![image](/assets/24.PNG)

So, due to this if ideal logic 1 = 1 volt then here practically it can be less then 1 volt i.e., 0.97 volts (Vdd'). So, for any signal to be considered as Logic '0' and '1' in the NM low and NM high range. It is danger case.

Any volatge which lies between Vol and Vil is called as Logic 0.

Any volatge which lies between Vil and Vih is called as Undefine Region.

Any volatge which lies between Vih and Voh is called as Logic 1.

![image](/assets/25.jpeg)

To solve this problem,, we have to put De-coupling capacitor in parallel with the circuit.It is huge capacitor which filled with a charge. Every time the circuit switches, it draws current from Cd, whereas, the  RL network is used to replenish the charge into Cd. And the amount of current needed for the circuit is supplied by the De- Coupling Capacitor.When ever De-copling capacitor discharges it takes charge from the supply and gets charged.

![image](/assets/26.PNG)

In the chip it will look something like shown below Decoupling capacitors are placed in between the block a, block b and block c. So here in this whole block it has been ensured that supply is being done by the de-coupling capacitor. Once we are done with this we have taken care of the local communication.

![image](/assets/27.PNG)


### <h2 id="header-2_1_4">Power planning</h2>

Let's now examine the local circuitry, which we will treat as a black box. It is repeatable, has logic at its boundaries, and the decoupling of the capacitor solved the issue of current demand. A signal, essentially ranging from logic 0 to logic 1, is sent from the driver to the load. To ensure that the load receives the same signal, we must keep this specific driver to load lines. The power supply is now turned on. Let us now assume that the 16-bit bus must maintain the same signal from the driver to the load. therefore the supply should provide it with enough power. However, there isn't a de-coupling capacitor available at this bus because Capacitors cannot physically be placed anywhere. Since the power supply and the bus are now far apart, there will undoubtedly be a voltage drop between them.

 ![image](/assets/28.PNG)


A specific 16-bit bus line that indicates logic 1 indicates that the capacitor is being charged to Vdd, while a logic 0 line indicates that the capacitor is being discharged to ground.Let's examine this 16-bit bus that is linked to the inverter. Because of the inverter, all of the capacitors that were first charged will now be discharged and vice versa.


![image](/assets/29.PNG)


However, the issue arises because every capacitor is linked to a single ground. The 'ground' tap point will become uneven as a result when the discharge occurs. The term "ground bounce" refers to that bump. The bump may go into an indeterminate state and transition to either logic 1 or logic 0 if its size surpasses the noise margin level. Thus, things get unpredictable at this point.

![image](/assets/30.PNG)


Additionally, using a single "vdd" tap point, all capacitors that were previously at "0" volts must be charged to "V" volts. The voltage at the Vdd tap point will drop as a result of this. We are okay as long as this voltage drop stays within the noise margin threshold, but if it enters an unknown area, then things get unpredictable.

![image](/assets/31.PNG)

The phenomena we saw resulted in a drop in supply voltage; this issue arose from electricity being applied to a single spot. Using numerous power supplies is the solution to the issue. As a result, each block will draw power from the closest power source and release it to the closest ground. The term **mesh** refers to this kind of power supply.

![image](/assets/32.PNG)


And the power planning for the top view is shown below,

![image](/assets/33.PNG)

### <h2 id="header-2_1_5">Pin placement and logical cell placement blockage</h2>

**Pin Placement**

Lets take below designs for example that needs to be implemented. Here first circuit is driven by clk1  and second circuit is driven by clk2 and both has different inputs Din1 and Din2 respectively and outputs as Dout1 and Dout2.Along with that we have some preplaced cells as well as Block a which recieves inputs from Din1 second input from Din2 and output goes to one of the input of combinational gates .This is the circuit to expain the concept of the placement and routing. We have another preplced cell as Blockb Which recieves input from clk1 and clk2 and provides a clk output. So currently we have 4 input ports Din1,Din2,Clk1,Clk2 and 3 output ports Dout1,ClkOut,Dout2

![image](/assets/34.jpg)

let's have one more design that needs to be implemented. 
so this section again as a FF1 and FF2  with  different colour (blue) the FF1 is driven by Din3 and Clk1 as inputs  and clock port of FF2 is clk 2 ,this types of circuits are very much helpful to understand the timing analysis of inter clocks ( which means two FF driven by two different clock inputs is know as inter clocks.)Now Let's have one more design that needs to be implemented. so this section again as a FF1 and FF2  with  different colour (green) the FF1 is driven by Din4 and Clk2 as inputs  and clock port of FF2 is clk 1.So currently we have 2 input ports Din3,Din4,and 3 output ports Dout3,ClkOut,Dout4.Along with that we have some preplaced cells as well as Block c which recieves inputs from Din3 second input from Din4 and output goes to one of the input of combinational gates 

![image](/assets/35.PNG)

Now complete design becomes like given below which has 6 input ports and 5 output ports. The connectivity information between the gates is coded using VHDL/Verilog language and is called as 'Netlist'.

![image](/assets/36.jpg)

Let's put this netlist in the core which we have designed before and let's try to fill this empty area between core and die with the pin information. The frontend team who decides the netlist connectivity input and output and the backend team who done the pin placements. So according to the pin placements, we have to locate the preplaced blocks nearer to the inputs of the preplaced blocks.



Here one thing that we noticed is that clock-in and clock-out pins are bigger in size as compared to Data ports (input and output pins) because the reason behind this is that, input clocks are conntinuously provides the signal to the every elements of the chip and output clock should out the signal as fast as possible because it driven continously. So, we need least resistance path for the clocks inputs and clocks outputs. So, bigger the size, lower the resistance.

![image](/assets/37.jpg)

One more thing is need to take care about is that, this pin placement area is blocked for routing and cell placements. so we nned to do logical cell placement blockage. this blockage is shoown in above image in between pins.

So, floor plan is ready for Placement and Routing step.

![image](/assets/38.jpg)

### <h2 id="header-2_1_6">Steps to run floorplan using OpenLANE</h2>

We needed certain switches before we could begin the floorplanning. These are available to us through the Openlane setup.

As we can see, by default, the aspect ratio is 1 and the core utilization ratio is 50%. In a similar manner, more information is provided. Nevertheless, accepting these values is not required. We must additionally modify these values in accordance with the specifications.


![image](/assets/39.jpg)


Here FP_PDN files are set the power distribution network. These switches are set in the floorplane stage bydefault in OpenLANE.
Here, (FP_IO MODE) 1, 0 means pin positioning is random but it is on equal distance.

In the OpenLANE lower priority is given to system default (floorplanning.tcl), the next priority is given to config.tcl and then priority is given to PDK varient.tcl (sky130A_sky130_fd_sc_hd_congig.tcl).

After setting switches according to our design we are ready to run the floorplan. The command for running floorplan is ```run_floorplan```

![image](/assets/40.jpg) 

After running the command it gives floorplan.

![image](/assets/41.jpg) 

### <h2 id="header-2_1_7">Review floorplan files and steps to view floorplan</h2>

The connfig.tcl file is located in the run folder. All of the configuration that the flow takes is contained in this file. The arguments that are acceptable in the current flow can be seen if we open the config.tcl file.

![image]( /assets/42.jpg)

Here are the default values pictures

![image](/assets/43.jpg)

We need to check at the findings to see how floorplane appears. One def (design exchange format) file is available as a consequence. All of the information regarding die area (0 0) (660685 671405) and unit distance in microns (1000) is visible if we open this file. One micron is equivalent to 1000 databased units. Thus, the units 660685 and 671405 are databased. and the diameters of the chips in micrometers can be obtained by dividing this by 1000. so, the width of chip is 660.685 micrometer and height of the chip is 671.405 micrometer

![image](/assets/44.jpg)


We must open the magic file by adding the command in order to view the actual layout following the flow.The command is  ```magic -T /home/kunalg123/Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130A.tech lef read ../../tmp/merged.lef def read picorv32a.floorplan.def```

And then after pressing the enter, Magic file will open. here we can see the layout.

![image](/assets/45.jpg)


### <h2 id="header-2_1_8">Review floorplan layout in Magic</h2>

In the layout we can see that, input output pins are at equal distance.

![image](/assets/45.jpg)


following the selection (To pick an object, click on it first, then hit the keyboard key's'. The item will be illuminated. Click the object to zoom it in, then hit 'z'; to zoom it out, press'sft+z'. One input pin requires us to enter the Tkcon window and type "what" in order to find its location or determine which layer it is available on. It will display every detail pertaining to that specific pin. indicating that the pin is located in metal 3.We determine that this pin is at metal 2 by doing the same for the vertical pins. vertical pins, we find that this pin is at metal 2.

![image](/assets/46.jpg)


## <h2 id="header-2_2">Library building and Placement</h2>
### <h2 id="header-2_2_1">Netlist binding and initial place design</h2>

**Bind netlist with physical cells**:- Let's look at the netlist of gates and note that each gate's shape corresponds to its purpose. As an illustration, consider the gate, which is actually a box with width and height rather than a tringular shape.Flipfops are square boxes, just like the AND gate, which actually has a box shape.Therefore, we have provided all of the flipflops and gates with their physical measurements. Because certain shapes, such as AND and OR gates, do not exist in the actual world, we will provide a certain shape and set of measurements for each component of the netlist. All of the blocks will also have the appropriate width, height, and shape.

![image](/assets/47.PNG) 

Now lets remove the wires,all the gates, flipflops and blocks are present in the shelf which is called as **Library**.

![image](/assets/48a.PNG)

A library is a place where you can find all kind of books all the gates,f/f are books here. Library also has the timing information of the paticular book like delay of the gates and it also have the required conditions of the gates. Library can be devides into two sublibraries, One library consist of shape and size and other library might consist only of the delay information. Library has the various flavours of each and  every cell. Like same cell can have bigger in size in different self, bigger the size of cell lesser the resestnce path so it will work faster and will have lesser delay. We can pick up from these what we want based on the timing condition and available space on the floorplan.

![image](/assets/48.jpg)

**Placement**:- The next step is to take those specific forms and sizes and position them on the floorplan once we have given each and every gate the right shape and size. We possess the floor design with input and output ports, a certain netlist, and a size assigned to every element in this netlist. Now that we have the logic gates' physical perspective. The netlist must then be positioned on the floorplan. In order to create the physical view gates on the floorplan, we must use the connection information from the netlist.


![image](/assets/50.jpg) 

We now have the correct floorplan with the preplaced cells from before. Plcement will ensure that the preplaced cell placements remain unchanged and that no cell should be placed on top of the preplaced cells. Two other things will be taken care of. The netlist circuit should only be used for connections on the floorplan. The physical view of the netlist must be positioned on the floorplan in a way that maintains logical connectivity and allows the circuit to interact with its input and output ports to maintain timing and minimal delay.

![image](/assets/49.jpg)


The remaining components from the netlist will now be arranged according to the blueprint.All of the components have been arranged so that their input and output pins are closed.
However, FF1 of Stage 4 and Din4 is still quite a distance away from the others. We can fix this issue by placing things as optimally as possible.

![image](/assets/51.jpg)


### <h2 id="header-2_2_2">Optimize placement using estimated wire-length and capacitance</h2>

**Optimize Plecement:-** In optimize placement we will resolve the problem of distancing.Lrt's take the example of FF1 to Din2. There must be a wire going from Din2 to FF1 but before going into routing the desing or wiring we will try to estimate the capacitances. If we lokk the capacitance from Din2 to FF1 it is every huge because wire length is huge in that case even the resutance will also be huge because of that length. If we send the signal from Din2 then it will be difficult for FF1 to catch that input because distance is large. So we can place some intermediate steps to maitain the Signal integrity. By this the input is succesfully driven to the FF1 from Din2. These intermediate steps are called here Repeaters , Repeaters are basically buffers that will recondition the original signal and make a bew signal which replicate the original signal and send it forward this process repeates untill we reach to the actual cell where we want to send the input in this way signal integrity is maintained. By using repeaters we resolve the problem of signal integrity but there will be a loose of area because more and more repeaters are used more area will be used of the particular floorplan.

![image](/assets/52.PNG)

In the stage 1, there is no need of any repeater to transmit the signal. But in stage 2, due to high distance, the lenth of wire is high and signal is not transmitted in perticular range. so we required repeater.

![image](/assets/53.PNG)

### <h2 id="header-2_2_3">Final placement optimization</h2>

As similar to stage 2, in Stage 3 also we required the buffer between gate2 and FF2.

![image](/assets/59.PNG)

Stage 4 is a little more difficult than the others.We must now verify whether or not what we have done is correct. To do this, we must perform a timing analysis taking into account the optimum clocks. Based on the analysis's data, we will be able to determine whether the placement is appropriate or not.

![image](/assets/60.PNG)

### <h2 id="header-2_2_4">Need for libraries and characterization</h2>

Each ICdesign Flow must go through a number of stages. Logic Synthesis is the first step that needs to be completed. For example, if we have functionality that is coded as RTL, we must first turn it into lawful hardware. This process is known as Logic Synthesis. The arrangement of gates that will represent the original functionality that has been defined using an RTL is the output of the logic synthesis. 
The next stage of logic synthesis is floorplanning, where we import the resulting data and determine the dimensions of the die and core. Placement, which comes after floorplaning, involves taking the specific logic cell and arranging it on the chip so that the initial better timing exists. The next phase is Clock Tree Synthesis (CTS), where we ensure that each CLK signal has an equal rise and fall and that it reaches every signal simultaneously.The next stage is routing, which requires following a specific flow based on the flip flop's characteristics.The next step, known as static timing analysis, involves determining the circuit's highest attainable frequency as well as its set up and hold times.'GATES or Cells' is a feature that all levels share.

### <h2 id="header-2_2_5">Congestion aware placement using RePlAce</h2>

We currently face congestion constraints rather than timing constraints. Thus, we are reducing the confusion.

There are two phases to the placement. both worldwide and specific. Legalization is not done in global placement; rather, it is done after thorough placement.

First, global placement takes place when the placement is run. The primary goal of glibal placement is to shorten wire lengths.

To view the actual view of the arrangement of the standerd cells, open the Magic file now.Below is the actual view that can be found in the magic file.

The command used for magic file is ``` magic -T /home/vsduser/Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130A.tech lef read ../../tmp/merged.lef def read picorv32a.placement.def```. 

![image](/assets/61.JPG)

If we zooom into this, we find the buffers, gates, flip flops in this.

![image](/assets/62.JPG)



## <h2 id="header-2_3">Cell design and characterization flows</h2>
### <h2 id="header-2_3_1">Inputs for cell design flow</h2>

In Cell Design Flow, Gates, flipflops, buffers are named as 'Standard Cells'. 

![image](/assets/54.PNG)

These standard cells are being placed in the section called as 'Library'.Library is a place where we place differnt type of books similarly in an IC design flow a library is a place where all standard cells are present. In the library many other cells are available which have same functionality but the size is different.These different sizes are refered as a Drive Strength.Library consists of cells with different functionality, different sizes and differnt thersold volatges.

![image](/assets/55.PNG)

If you go into one of the inverter from the library the cell design flowis as follows

The inverter has to represented in form of the shape, drive strength, power charracteristic and so on.
 
 The cell design flow is devided into three parts.

1. Inputs

2. Design steps

3. Outputs

![image](/assets/56.PNG)

**1)Inputs**:- Inputs required for cell design is PDKs, DRC and LVS rules SPICE models, library and user defined specs and this are provided by foundaries. In DRC& LVS rules tech file is provided which contains design rules and actual values. Rules can be converted in to code. SPICE MODEL tells about threshold voltage equation.

![image](/assets/57.PNG)
![image](/assets/58.PNG)

### <h2 id="header-2_3_2">Circuit design steps</h2>

The seperation between the power rail and the ground rail defines the cell height. Cell width depends upon the timing and drive strength.Supply volate , Metal layers 

**2)design steps**:- Design involves three steps which are circuit design, layout design, characterization.

**In circuit Design** there are two steps.

First step is to implement the function itself and second step is to model the PMOS nad NMOS transistor in such a fashion in order to meet the libraray.

![image](/assets/63.jpg )
![image](/assets/65.jpg )
![image](/assets/64.jpg)

Layout Design step;
![image](/assets/66.jpg)


Characterization:
![image](/assets/67.jpg)
![image](/assets/68.jpg)
![image](/assets/69.jpg)

**3)Outputs**

The typical output what we get from the circuit design is CDL(circuit description language) file,GDSII,LEF,extracted spice netlist(.cir).




### <h2 id="header-2_3_3">Layout design step</h2>

The first step in layout design is to implement the function using a collection of PMOS and NMOS transistors to implement the MOS transistor; the second step is to extract the implemented design's PMOS and nNMOS network graphs.

![image](/assets/63.jpg)

Obtaining the Euler's path comes next after obtaining the network graphs. In essence, Eule's path is the one that is traced just once.

![image](/assets/65.jpg)
Drawing a stick diagram based on the Euler's path is the next stage. The circuit diagram is the source of this stick diagram.

![image](/assets/64.jpg)



The next stage is to turn this stick diagram into a usual layout, a proper layout, and finally the appropriate rule that we previously discussed. As soon as we obtain the specific layout, we will know the cell length and width as well as all the other criteria, such as pin placements and drain current.

![image](/assets/66.jpg)

Extracting the specific layout's parasatics and characterizing it in terms of timing is the next and last stage. Thus, GDSll will be the layout design's output prior to that. We characterize the extracted spice netlist when you receive it. Timing, noise, and power information can be obtained with the use of characterization.


### <h2 id="header-2_3_4">Typical characterization flow</h2>

Let's attempt to construct the characterisation flow using the available inputs.

Firstly, the model must be read; next, the extracted spice netlist must be read; third, the buffer's behavior must be defined or recognized; fourth, the inverter's subcircuits must be read; fifth, the necessary power supplies must be attached; sixth, the stimulus must be applied; seventh, the output capacitance must be provided; and eighth, the necessary simulation commands must be provided. For instance, if transent simulation is being done, the ```.trans``` command. must be given; if DC simulation is being done,  ```.dc``` command.

![image](/assets/67.jpg)
![image](/assets/68.jpg)

The next stage is to give the characterisation software **"GUNA"** with all of these inputs, numbered 1 through 8, in the form of a configuration file.

This program will provide a timing, noise, and power model.

![image](/assets/69.jpg)

## <h2 id="header-2_4">General timing characterization parameters</h2>
### <h2 id="header-2_4_1">Timing threshold definitions</h2>


As was evident in the previous section, there are inverters connected back to back, power sources, and stimulus applied to the inverter. All of these factors contribute to the crucial concept of "timing threshold definitions," which is the understanding of distinct threshold points within a waveform.

The term 'Slew_low_rise-thr' in the figure below represents a value that is near to zero. and while this usually has a value of 20%, it might also have a value of 30%.

![image](/assets/70.jpg)


NOw, taking the waveform of input stimulus which is input of the first buffer and with that taking output of the first buffer.Similar as a slew, thresolds are for delay also available. for that same as slew, we have to take some rise and fall points from the waveforms. this tresolds are almost 50%.

![image](/assets/71.jpg)

![image](/assets/72.jpg)



### <h2 id="header-2_4_2">Propagation delay and transition time</h2>

The values mentioned above will be the basis for our calculations of other parameters, such as propagation latency, current, swings, etc.

To determine the delay of any given calculation, we must deduct the out_rise_thr from the in_rise_thr. Here, we'll use the typical figure of 50%. Let's examine how it functions on this specific waveform.
Time delay = Time(out_thr)-time(in_thr).

![image](/assets/73.jpg)

In the example above, 50% was maintained for both in_rise_thr and out_fall)thr. Negative delays, on the other hand, are not allowed if the threshold point rises and the output appears before the input. Therefore, it is crucial to choose the threshold point carefully because it is the cause of this negative delay.

![image](/assets/74.jpg)



**Transition time**=  time(slew_high_rise_thr)- time(slew_low_rise_thr)

or

transition time = time(slew_high_fall_thr)- time(slew_low_fall_thr)

Let's say we have the waveform to understand the slew calculation.

![image](/assets/75.jpg)

# <h3 id="header-3">Day 3 - Design library cell using Magic Layout and ngspice characterization</h3>	 
## <h3 id="header-3_1">Labs for CMOS inverter ngspice simulations</h3>
### <h3 id="header-3_1_0">IO placer revision</h3>

We have completed run placement and floor planning thus far. However, if we would like to alter the floorplanning, for instance, we may do so by adjusting the pins' equal distance from one another in our floor plan. The```Set``` command.

![image](/assets/92.jpg)

To do that, we must first examine the configuration's switches, and then we must use the syntax "env(FP_IO_MODE) 1". ultimately arrive at "env(FP_IO_MODE) 2". proceed with the floorplanning once more.

Next, use magic-T to verify if the pins' locations have changed.

![image](/assets/93.JPG)

So, here we can see that there are no pins in the upper half side. all pins are in the lower half of the core.


### <h3 id="header-3_1_1">SPICE deck creation for CMOS inverter</h3>

**VTC- SPICE simulations**:-The first step in this process is to generate a SPICE deck, which is essentially a netlist since it contains connectivity information about it.It features deck points that will take the output and inputs that are given to the simulation.

**Component connectivity**:- We must provide the substrate pin's connection in this. The PMOS and NMOS threshold voltages are adjusted by the substrate pin.

![image](/assets/76.jpg)

**Component values**:- Values for the PMOS nad NMOS. We have taken the same size of both PMOS and NMOS.

![image](/assets/77.jpg)

**Identify the nodes**:- Node mean the points between which there is a component.These nodes are required to define the netlist.

![image](/assets/78.jpg)

**Name the nodes**:- Now we wiil name these nodes as Vin, Vss, Vdd, out.

![image](/assets/79.jpg)

Now we will start writing the SPICE deck. It's written like shown below

Drain- Gate- Source-  Substrate

For M1 MOSFET drain is connected to out node, gate is connected to in node, PMOS transistor substrate and Source is connected to Vdd node. 

For M2 MOSFET drain is connected to out node, gate is connected to in node, NMOS source and substrate are connected to 0.

![image](/assets/80.jpg)


### <h3 id="header-3_1_2">SPICE simulation lab for CMOS inverter</h3>

After discussing the CMOS inverter's connectivity up to this point, we will now discuss the connectivity of the other components, such as the load capacitor and source. Let's examine the output load capacitor's connectivity.

It is linked to both node 0 and out. It is also worth 10ff. Similar to the supply voltage (Vdd), which is connected between Vdd and node 0 and has a value of 2.5, we also have an input voltage (Vin), which is connected between Vin and node 0.

![image](/assets/81.jpg)

We now need to provide the simulation commands, which involve swiping the Vin with a stepsize of 0.05 from 0 to 2.5. Considering that we desire Vout while modifying the Vin.

![image](/assets/82.jpg)

Final step is to model files. It has the complete description about NMOS and PMOS.

![image](/assets/83.jpg)



Now we will do the SPICE simulation for the particular values. And will get the graph.

![image](/assets/84.PNG)

Now, doing other simulation in which we change the PMOS width to 3 times of NMOS width. and after diong the simulation, we get the graph like this shown below

![image](/assets/85.PNG)

The difference between these two graphs is that in the second graph the transfer charactoristic is lies in the ecxact middle of the graph where in the first graph it is lies left from the middle of the graph.


### <h3 id="header-3_1_3"> Switching Threshold Vm</h3>

Each of these two models, varying in breadth, has a specific use. By contrasting these two waveforms, we can observe that regardless of the voltage level, they have the same shape.It demonstrates how robust CMOS technology is. The production is at its highest when Vin is low and at its lowest when Vin is high. Consequently, the characteristic is maintained across all CMOS sizes with varying NMOS or PMOS sizes. For this reason, CMOS logic is frequently employed in gate design.

![image](/assets/86.jpg)

One of the parameters that determined the inverter's robustness was the switching threshold, or Vm (the point at which the device shifts levels). Vin=Vout is the moment at which the switch is made.

![image](/assets/87.jpg)

This figure shows that Vin=Vout at Vm~0.9v. Because there is a probability that both PMOS and NMOS are activated at this point, it is a crucial moment for the CMOS. There is a significant risk of leaking current if both are turned on (means current flow direcly from power to earth).

We can understand the idea of switching the threshold voltage by comparing these two graphs.


We can see which region the PMOS and NMOS are in by looking at the graph below. For NMOS and PMOS, the direction of current flow is different.

![image](/assets/88.jpg)


### <h3 id="header-3_1_4"> Static and dynamic simulation of CMOS inverter</h3>
We will learn about the CMOS inverter's rise and fall delays as well as how they change with Vm through dynamic simulation. Everything else in this simulation will remain the same, with the exception of the input, which is a pulse, and the simulation command.trans

This is where the Time vs. Voltage graph will be shown, allowing us to compute the rise and fall delays.

![image](/assets/89.jpg)

![image](/assets/90.PNG)

![image](/assets/91.PNG)



### <h3 id="header-3_1_5"> Lab steps to git clone vsdstdcelldesign</h3>
Copy the clone address from the repository and put it in the openlane terminal after running the command ```git clone``` to obtain the clone. In the openlane directory, this will create the "vsdstdcelldesign" folder.



now, if we open the openlane directory, we find the vsdstdcelldesing folder in the openlane directory.

Now, when we open the vsdstdcelldesign folder, the.mag file, libs file, and other files appear.

![image](/assets/142.jpeg)

Let's open the.mag file now to examine which layers go into creating the inverter. However, we need the tech file before we can open the mag file. therefore we'll copy this file from the site listed below. Additionally, make a copy by ```cp``` instruct to the address shown below.This file is now visible as a copy in the vsdstdcelldesign folder.

![image](/assets/141.jpeg)

We have copied the tech file here, so we don't need to write the entire address in order to view the layout in magic.The CMOS inverter's layout in the magic is now visible to us as follows.

![image](/assets/133.jpeg)


## <h3 id="header-3_2">Inception of layout ̂A CMOS faabrication process</h3>
### <h3 id="header-3_2_1">Create Active regions</h3>

**1) selecting a substrate**:- Our p-type silicon substrate is well doped, has an orientation of 100, and has a high resistivity of 5 to 50 ohm.

![image](/assets/94.jpg)


**2) creating active region for transistor**:- Area where PMOS and NMOS are observed. We will develop a few small pockets on a p-type substrate that we will refer to as the active region. PMOS and NMOS transistors will be created in these pockets. Will create a barrier of separation between every pocket. 

By applying the SiO2 layer (~40 nm) on the substrate, we produce the isolation layer. On top of the Sio2 layer, we are currently depositing the Si3N4 layer (~80 nm).

![image](/assets/95.jpg)

Determine the area where the pocket has to be created before beginning. We are going to apply a layer of photoresist (~1um) and use UV light to produce a mask 1.

![image](/assets/95.jpg)

UV light has been used to expose the unwanted area. And the exposed section is being washed away, giving us a pattern.

![image](/assets/96.jpg)

The mask will be taken off in the following phase, and the exposed Si3N4 layer will be etched.

![image](/assets/97.jpg)

The next stage is to utilize a chemical reaction to remove the photoresist because the Si3N4 layer is now acting as a good protective layer for the Sio2 layer. We're going to put it in the oxidation furnace now. Local oxidation of silicon, or LOCOS, is a process that causes the exposed silicon dioxide portion to expand and forms bird breaks. The ideal separation between two PMOS and NMOS will be provided by this increased sio2. We safeguard two transistors that are in communication with one another in this way.

![image](/assets/98.jpg)

The Si3N4 must then be eliminated using hot phosphoric acid.
![image](/assets/99.jpg)


### <h3 id="header-3_2_2">Formation of N-well and P-well</h3>

**3) Formation of N-well and P-well**: P-well and N-well cannot be formed simultaneously. We must use photoresist to build one of the regions while protecting another. Next, in order to create the P-well, we will pattern the photoresist using mask 2 and UV light.

![image](/assets/100.jpg)
![image](/assets/101.jpg)
The region where the P-well is to be formed is now visible. Now, we take off the mask and use boron to create a P-well using the ion implantation approach (~200kev). However, the implant is still P. It will turn into P-well after the high-temperature annealing is completed.

![image](/assets/102.jpg)

We will use mask 3 and phosphorus ions in a similar procedure to build N-well.

![image](/assets/103.jpg)

Well depths are not yet defined. Thus, we shall determine the well depth by placing into the high temperature furnace (drive-in diffusion).

![image](/assets/104.jpg)
![image](/assets/105.PNG)

### <h3 id="header-3_2_3"> Formation of gate terminal</h3>

**4)Gate formation**:- Since we can only regulate the threshold voltage from the gate terminal, it is the most significant terminal for both PMOS and NMOS. The oxide capacitance and doping concentration will regulate the threshold voltage.Thus, we are going to keep the doping concentration here initially. In order to achieve this, we utilize mask 4 and perform ion implantation of boron ions at a lower energy (~60kev).

![image](/assets/106.PNG)

Using mask 5 and arsenic ion, we will conduct the same procedure for N-well as well.

![image](/assets/107.jpeg)

The oxide layer needs to be fixed as the next stage. However, since the oxide layer is damaged as a result of improper procedures, we must first remove it. Thus, we use HF solution to first remove the layer before growing a high-quality oxide layer again that is the same thickness.

For a low resistance gate terminal, the last step is to deposit a layer of polysilicon over an oxide layer that has more impurities.Afterwards, this polysilicon layer was etched off using photoresist and mask 6.

![image](/assets/109.jpeg)

When the photoresist is removed after etching, the gate terminal appears like this:

![image](/assets/108.jpeg)


### <h3 id="header-3_2_4">Lightly doped drain (LDD) formation</h3>

**5) LDD formation**:- HP+,P-,N and N+,N-,P doping profiles for PMOS and NMOS, respectively, are what we actually want. The explanation for that is

The influence of hot electrons

brief channel impact

We use mask 7 and her to do ion implantation in P-well once again in order to construct LDD.e we use phosphoros as a ion for light doping.

![image](/assets/111.PNG)

We will use the same procedure for N-well. There, BORON Ion and mask 8 are used.

![image](/assets/112.PNG)

We may now safeguard the true structure of P-implant and N-implant by constructing spacers. To do this, we cover the gate threshold with a thick coating of SiO2 or Si3N4.

![image](/assets/110.jpeg)

We now perform anisotropic etching with plasma. Side-wall spacers are created in this way.
![image](/assets/114.PNG)
![image](/assets/113.PNG)


### <h3 id="header-3_2_5">Source ÃÂ drain formation</h3>

**6)source-drain formation**

The next action is to apply a very thin layer of screen oxide to prevent channeling.

![image](/assets/118.PNG)

In order to construct the N+ implant and form the drain and source, we repeat the arsenic ion implantation process at 75 keV, utilizing mask 9 in the P-well to form PMOS.

![image](/assets/117.PNG)


The same procedure will be repeated for NMOS in order to create P-implant, employing mask 10 and boron ions in the N-well at 50 keV.

![image](/assets/116.PNG)

We are now annealing this half-made CMOS at a high temperature of 1000 degrees. Thus, the source and drain are now P+ and N+ implants.

![image](/assets/115.PNG)



### <h3 id="header-3_2_6">Local interconnect formation</h3>

**7)steps tp form contacts and local interconnects**:- Etching is the first step in removing the thin coating of screen oxide. The titanium (Ti) should next be deposited using sputtering. Since Ti has a very low resistance, it is employed here.

![image](/assets/119.PNG)

The next stage is to establish a reaction between the CMOS source, gate, and drain and the Ti layer. For roughly 60 seconds, the wafer is heated to a temperature of between 650 and 700 degrees in an ambient N2 environment. and the titanium siliside is seen over the wafer following the reaction. Between Ti and N, there is one further reaction that produces the TIN, which is utilized for local communication.

![image](/assets/120.PNG)

At this point, we will etch out the TIN and create precise connections using mask 11 and photoresist. RCA cleaning is used to remove TIN.

![image](/assets/121.PNG)

Now that the photoresist has been etched and removed, local interconnects are created.

![image](/assets/122.PNG)


### <h3 id="header-3_2_7"> Higher level metal formation</h3>

**8)Higher level metal formation**:- These actions are quite similar to the earlier ones. The surface's lack of planning is the first thing we notice. Because of the issues with metal disconinuty, it is not advisable to utilize this kind of non-planer surface for metal interconnects. In order to create a less resistant layer, we must plannerize the surface by applying a thick coating of sio2 mixed with various impurities. and after that, we plannerized the surface using the CMP (chemical mechanical polishing) process.

![image](/assets/123.PNG)
![image](/assets/124.PNG)
Now, we etched the SiO2 layer to expose the metal within it using Photorsist and Mask 12.

![image](/assets/125.PNG)

After removing the photoresist, place a thin layer of TIN (~10 nm) on top of the wafer. Due to the fact that TiN functions as a barrier between the top and bottom layers of metal interconnects and as an excellent adsorption layer for SiO2.

![image](/assets/126.PNG)

The wafer must next have the blanket tungsten (W) layer deposited on top of it. and then plannerize the surface here using the CMP.

![image](/assets/127.PNG)

The W in question serves as a contact hole, and it must be connected to the higher metal layer. so the coating of aluminum, or Al, will be deposited.

![image](/assets/128.PNG)

Then by using the mask 13 and photoresist, we etched the W layer out to form the contact at perticular place by Plasma etching.

![image](/assets/129.PNG)

This is our first level of metal interconnets. now we again do the same process as above to deposite the second level of metal interconnect by using mask 14 for etched out the sio2 and using mask 15 for etched out Al leyer.

![image](/assets/130.PNG)

The upper layer of Al is bit thicker as compared to lower layer of Al.Now, again deposite the layer of sio2 or si3N4 to protect the chip.

![image](/assets/131.PNG)

And finally our CMOS is looks like this after the fabrication.

![image](/assets/132.PNG)



### <h3 id="header-3_2_8"> Lab introduction to Sky130 basic layers layout and LEF using inverter</h3>

![image](/assets/133.jpeg)

In sky130, every color is showing the different layer. here the first layer is for local interconnect shown by blue_purple color, then second layer is metal 1 which is shown by light purple color, and the metal 2 is shown by pink color. N-well is shown by solide das line. green is N-diffusion region. and red is for polysilicon gate. similarly the brown color is for P-diffusion.

In tckon window, we can see that the selected area is NMOS and similarly we can chech PMOS also. and that is how we can check that the CMOS is working or not.

similarly we will check for the output terminal also.(by double pressing "S" to select the entire thing at output Y).

![image](/assets/133.jpeg)

so, we can see that "Y" is attached to locali in cell def sky130_inv.

we can check the source of the PMOS is connected to the ground or not. and similarly we can check it for NMOS also.



### <h3 id="header-3_2_9">Lab steps to create std cell layout and extract spice netlist</h3>

To extract the file from here, we have to write the command in tckon window. and the comand is ```extract all```

![image](/assets/134.jpeg)

Now let's go to this location from the terminal. it is exctracted.


we will use this .ext file to create the spice file to be use with our ngspice tool. for that we have apply the command ```ext2spice cthresh 0 rthresh 0```. this will not create anything new. now again we have to type ```ext2spice``` command in tckon window.so, now we are checking the location and at there spice file has been created.

![image](/assets/134.jpeg)



let's see what inside the spice file by "vim sky130_inv.spice".

![image](/assets/135.jpeg)


## <h3 id="header-3_3">Sky130 Tech File Labs</h3>
### <h3 id="header-3_3_1">Lab steps to create final SPICE deck using Sky130 tech</h3>

![image](/assets/135.jpeg)

here, we can see the all details about the connectivity of the NMOS and PMOS and about the power supply also.

X0 is NMOS and X1 is PMOS and both's connectivity is shown as GATE DRAIN SUBSTATE SOURCE.

Now we have to include the PMOS and NMOS lib files. it is inside the libs folder in the vsdstdcellsdesign folder.

![image](/assets/136.jpeg)

so, now we include this file in the terminal by ```.include ./libs/pshort.lib``` and ```.include ./libs/nshort.lib``` command.

And then set the supply voltage "VDD" to 3.3v by ```VDD VPWR 0 3.3V``` command. and similarly set the value of VSS also.

Now, we need to specify the input files. by ```Va A VGND PULSE(0V 3.3V 0 0.1ns 2ns 4ns)```.

Also add the command for the analysis like, ```.tran 1n 20n```, ```.control``` , ```run```,```.endc```,```.end```.

![image](/assets/137.jpeg)


after running this file we get output of ngspice like this,

![image](/assets/138.jpeg)

Now, ploting the graph here by command, ```plot y vs time a```.

![image](/assets/138.jpeg)

NOw if we increase the C3 value from 0.024ff to 2ff the graph will look like this, graph become more smoother.

![image](/assets/139.jpeg)


### <h3 id="header-3_3_2">Lab steps to characterize inverter using sky130 model files</h3>

Here, we have to find value of 4 parameters.
	
<ul>
	<li><a> rise time calculation</a></li>
	</ul>
	
it is time taken to the output waveform to 20% value to 80% value.


so, rise time= (2.2489 - 2.1819)e-09 = 66.92 psec.


<ul>
	<li><a> fall time calculation</a></li>
	</ul>
 
it is the time take by output for transition from 80% to 20%.


so, rise time= (4.09512 - 4.05264)e-09 = 42.51 psec.

<ul>
	<li><a> propagation delay calculation</a></li>
	</ul>

it is the time difference between the 50% of input and 50% of the output.



so, propogation delay =(2.2106 - 2.15012)e-09 =  60.48 psec.


<ul>
	<li><a> cell fall delay calculation</a></li>
	</ul>
 
it is time for output falling to 50% and input is rising to 50%.


so, cell fall delay =(4.07735 - 4.04988)e-09 =  27.47 psec.

We have successfully characterized our inverter.
Our next objective is to create a lef file using the layout and we will plugin this lef file in the picorv32a core

### <h3 id="header-3_3_3">Lab introduction to Magic tool options and DRC rules</h3>

To know more about the Magic DRC we can go to the website:- http://opencircuitdesign.com/magic/Technologyfiles/TheMagicTechnologyFileManual/DrcSection 

Link to Google_Skywaters Design Rules: - https://skywater-pdk.readthedocs.io/en/main/rules/periphery.html

For reference , we can use the github repo of Google-Skywater: - https://github.com/google/skywater-pdk


### <h3 id="header-3_3_4">Lab introduction to Sky130 pdk's and steps to download labs</h3>

Follow the steps:

First go to the home directory.

**To download the lab files for performing DRC corrections**:

```wget http://opencircuitdesign.com/open_pdks/archive/drc_tests.tgz```

**To extract the lab files from the downloaded file:**

```tar xfz drc_tests.tgz```

Then go inside the lab folder drc_tests.

To list all the directories, we can use the command ```ls -al```.

To view the .magicrc file, we can use the command ```gvim .magicrc```. This file serves as the startup script for magic and tells it where to find the technology file. The technology file is already available locally in the same directory, so we can make changes to it if needed.

To start the magic tool with better graphics, we can use the command ```magic -d XR &```.



Content of .magicrc file by using command ```vi .magicrc```




### <h3 id="header-3_3_5">Lab introduction to Magic and steps to load Sky130 tech-rules</h3>

Use the command ```magic -d XR```

to open the magic tool. Open the met3.mag file from the file menu. we will see different layouts with different DRC values, called rule numbers.

![image](/assets/140.jpeg)

These rule number we can found at  Google-Skywater documentation.


Now we will select the any layout area and check drc why in tckon.

![image](/assets/143.jpeg)

Next, select a blank area and hover the mouse pointer over the metal3 contact icon. Press the p button and type 'pek' in the tkcon. Then execute the command ```cif see VIA2``` in the tkcon tab. 



### <h3 id="header-3_3_6">Lab exercise to fix poly.9 error in Sky130 tech-file</h3>

Now, we will open the poly.mag file in the magic tool with the helo of the command  ```load poly.mag``` in the tkcon terminal.

![image](/assets/143.jpeg)

Now consider the rule poly.9 then check the website for that particular rule.


To find the error, we can look at the sky130A.tech file which is present in the drc_tests directory. we can open this file with the text editor of Linux itself.


Search for 'poly.9' in the sky130A.tech file. It appears in both the POLY and uhrpoly sections, where the rules are not set properly. Add a change in both sections.


After making changes to the sky130A.tech file, click on Save and close the editor file.

Next, execute the command ```tech load sky130A.tech``` in the tkcon terminal. Then, run the drc check as shown below.

![image](/assets/143.jpeg)




# <h4 id="header-4">Day 4 - Pre-layout timing analysis and importance of good clock tree</h4>	 
## <h4 id="header-4_1">Timing modeling using delay tables</h4>
### <h4 id="header-4_1_1">Lab steps to convert grid info to track info</h4>

Now, we need to extract the '.lef' file from the '.mag' file to place it into the picorv32a flow.

There are certain guidelines to follow while making standard cells:

- The input and output ports must lie on the intersection of the vertical and horizontal tracks.
 
- The width of the standard cell should be an odd multiple of the track pitch, and the height should be an odd multiple of the track vertical pitch.

Now we can open the track file from ```pdk/sky130/libs.tech /openlane/sky130_fd_sc_hd/track.info``` to get more information on this.


![image](/assets/144.png)


The track is used during the routing stage and is essentially a trace of metal layers such as metal 1, metal 2, etc.

PNR is automated, so we need to specify where we want the routes to go. This specification is given by tracks. Each of the tracks is placed at (0.23, 0.46)um horizontally and (0.17, 0.34)um vertically for li1, metal 1, and metal 2 layers.

In the layout, the ports are on the li1 layer. To ensure that the ports are on the intersection of the tracks, we will need to convert the grid into the tracks.

To do this, we can first open the tracks file and then open the tkcon window and type the ```help grid``` command.

![image](/assets/144.png)

Then again will write command according to the track file required.

![image](/assets/154.jpg)


Now we can see that, the ports has been placed at the intersection of the tracks. But between the boundaries, 3 boxes are covered. so our second requirment also satisfies here.

### <h4 id="header-4_1_2">Lab steps to convert magic layout to std cell LEF</h4>

Now, we will need to decide on the port name and its values. we can set the values for different ports, and for the power and ground port, we will need to make changes in the 'attach to layer' as Metal1.

![image](/assets/156.png)

After these parameters are set once, we are ready to extract the lef file from the mag


Now, we open this file in the magic by the command 

```magic -T sky130A.tech sky130_vsdinv.mag &```

To extract the lef file we have to write the command in the tckon window as given below,

```lef write``` 

so it will create a lef file and we can check it in the vsdstdcellsdesign folder by using command ```ls -ltr```.




### <h4 id="header-4_1_3">Introduction to timing libs and steps to include new cell in synthesis</h4>

Now that the .lef file has been created, the next step is to plug this file into picorv32a. Before that, we will need to move the files to the src folder where all the design files are available at one location.

To do this, we can copy the file using the ```cp``` command.


this is how the library file looks like. We have different library files named as typical,slow ,fast.



Now we will copy it to the src folder

!
Here We need to modify the config.tcl file of picorv32a directory,
 
So open the config.tcl file of picorv32a directory and add the commands shown in below image :

![image](/assets/155.png)


**OPENLANE :-** Now we will go to the open lane directory and execute the docker command.

Will Execute the following commands in a line

    ./flow.tcl -interactive
    package require openlane 0.9
    prep -design picorv32a
    set lefs [glob $::env(DESIGN_DIR)/src/*.lef]      
    add_lefs -src $lefs
    run_synthesis

  ![image](/assets/157.png)

  ![image](/assets/158.png)

  ![image](/assets/159.png)

  

### <h4 id="header-4_1_7">Lab steps to configure synthesis settings to fix slack and include vsdinv</h4>

We will try to modify the parameters of our cell by referring the README.md file in the configuration folder in openlane directory

The README.md file contains information about the parameters of the cell. 

![image](/assets/160.png)

We will give the following commmands in the terminal in openlane directory

  ```prep -design picorv32a -tag 01-04_12-54 -overwrite```
  
  ```set lefs [glob $::env(DESIGN_DIR)/src/*.lef]```
  
  ```add_lefs -src $lefs```

  ```echo $::env(SYNTH_STRATEGY)```
  
  ```set ::env(SYNTH_STRATEGY) "DELAY 3"```
  
  ```echo $::env(SYNTH_BUFFERING)```
  
  ```echo $::env(SYNTH_SIZING)```
  
  ```set ::env(SYNTH_SIZING) 1```
  
  ```echo $::env(SYNTH_DRIVING_CELL)```
  
  ```run_synthesis```
  
 ```prep -design picorv32a -tag 01-04_12-54 -overwrite``` is used to overwrite the existing files with previous values of simulations.

After synthesis, we have observed that the slack is nagative. 

wns(worst negative slack)= -23.89 

tns(total negative slack)= -711.59.

 ![image](/assets/161.png)

 ![image](/assets/162.png)

Now ```run_synthesis``` we will see chip area has incresed and the value of slack has reduced.

Since synthesis of the picorv32a is successful, so we will run the floorplan using command ```run_floorplan```



Since, we are getting the error so first again we have to do the synthesis using the commands mentioned earlier and then we will use following commands to do the floorplan,

  ```init_floorplan```
  
  ```place_io```
  
  ```tap_decap_or```



so now we are good to run the placement using command ```run_placement```



Here placement is succesfull now without any error.




We will run the expand command in the tkcon window 








### <h4 id="header-4_2_3">Lab steps to configure OpenSTA for post-synth timing analysis</h4>

We have do STA on the picorv32a design which had timing violations.First we will run the synthesis using the following commands in openlane directory

    docker
    ./flow.tcl -interactive
    package require openlane 0.9
    prep -design picorv32a
    set lefs [glob $::env(DESIGN_DIR)/src/*.lef]
    add_lefs -src $lefs
    set ::env(SYNTH_SIZING) 1
    run_synthesis

 

Now we have to make a new ```pre_sta.conf``` file. We can do this by vim editor or in simple text editor also.



Now we will create a my_base.sdc file which will have the definitions of environment variables.

Now, we also need to create my_base.sdc file having the data shown in below image in openlane/designs/picorv32a/src directory


Now will go to the openlane directory in a new terminal and execute the ```sta pre_sta.conf``` command.


### <h4 id="header-4_2_4">Lab steps to optimize synthesis to reduce setup violations</h4>

 Now we will change the FANOUT parameter and again do the synthesis,

```prep -design picorv32a -tag 02-04_05-27 -overwrite```

```set lefs [glob $::env(DESIGN_DIR)/src/*.lef]```

```add_lefs -src $lefs```

```set ::env(SYNTH_SIZING) 1```

```set ::env(SYNTH_MAX_FANOUT) 4```

```echo $::env(SYNTH_DRIVING_CELL)```

```run_synthesis```



Now, run the ```sta pre_sta.conf``` command in a new terminal in openlane directory itself,


### <h4 id="header-4_2_5">Lab steps to do basic timing ECO</h4>

OR gate which has a drive strength of 2 is driving 4 fanout.



So we have to replace this OR Gate with another OR Gate having Drive strength of 4 by executing the commands given below,

**To Reports all the connections to a net**

  ```report_net -connections _11672_```

**To Check the command syntax**

   ```help replace_cell```

**To Replace the cell**

   ```replace_cell _14510_ sky130_fd_sc_hd__or3_4```

**To Generate the custom timing report**

   ```report_checks -fields {net cap slew input_pins} -digits 4```


 
 Now we can see theslack has been reduced from -23.89 to -23.51

In above case also OR gate which has a drive strength of 2 is driving 4 fanout.

So we have toreplace this OR Gate with another OR Gate having Drive strength of 4 by following these commands

**To Reports all the connections to a net**

 ```report_net -connections _11675_```

**To Replace the cell**

 ```replace_cell _14514_ sky130_fd_sc_hd__or3_4```

**To Generate the custom timing report**

 ```report_checks -fields {net cap slew input_pins} -digits 4```







### <h4 id="header-4_3_3">Lab steps to run CTS using Triton</h4>

Now we need to replace the old netlist with newly generated netlist which has generated after reducing the slack. And then we will run floorplan , placement and CTS.



The image shown above has the netlist before making the modifications.

So, we need to make a copy of this old netlist and then we will add the newly generated netlist to be used in our openlane flow for further process.

So we will make the copy by following commands.

**To go to the following location**
   
```cd Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/runs/02-04_05-27/results/synthesis/```

**To List the contents**

```ls -ltr```

**To copy the netlist with particular name**

 ```cp picorv32a.synthesis.v picorv32a.synthesis_old.v```

**To List the contents**

```ls -ltr```



Now we will do synthesis again then floorplan , placement and cts in the openlane directory itself by the following commands,

       prep -design picorv32a -tag 02-04_05-27 -overwrite
       set lefs [glob $::env(DESIGN_DIR)/src/*.lef]
       add_lefs -src $lefs
       set ::env(SYNTH_STRATEGY) "DELAY 3"
       set ::env(SYNTH_SIZING) 1
       run_synthesis
       init_floorplan
       place_io
       tap_decap_or
       run_placement

       # Incase getting error will use this command
       unset ::env(LIB_CTS)

       run_cts


Now  .cts file has created in the location as shown the image below,




### <h4 id="header-4_3_4">Lab steps to verify CTS runs</h4>
**OPENROAD**
To create a database in OPENROAD using LEF and TMP files, we can use the following commands:

1. First, make sure we are in the directory where the LEF and TMP files are located.

2. Then, enter the following command to start the OPENROAD tool,

    openroad

3. Once you are in the OPENROAD tool, enter the following command to create the database,

**To Read lef file**

```read_lef /openLANE_flow/designs/picorv32a/runs/02-04_05-27/tmp/merged.lef```

**To Read def file**

```read_def /openLANE_flow/designs/picorv32a/runs/02-04_05-27/results/cts/picorv32a.cts.def```

**To Create an OpenROAD database file named pico_cts.db**

```write_db pico_cts.db```

Now we can see this database file is present in openlane directory.







### <h4 id="header-4_4_3">Lab steps to analyze timing with real clocks using OpenSTA</h4>
Now we can execute the following commands,

**To load the created db file in Openroad**

```read_db pico_cts.db```

**To read the netlist post CTS**

```read_verilog /openLANE_flow/designs/picorv32a/runs/02-04_05-27/results/synthesis/picorv32a.synthesis_cts.v```

**To read the library for design**

```read_liberty $::env(LIB_SYNTH_COMPLETE)```

**To link the design and library**

```link_design picorv32a```

**To read the custom sdc we have created**

```read_sdc /openLANE_flow/designs/picorv32a/src/my_base.sdc```

**To setting all clocks as propagated clocks**

```set_propagated_clock [all_clocks]```

**To Generate the custom timing report**

```report_checks -path_delay min_max -fields {slew trans net cap input_pins} -format full_clock_expanded -digits 4```

**To exit from Openlane flow**

```exit```

![image](/assets/151.jpg)

![image](/assets/152.jpg)

![image](/assets/153.jpg)

### <h4 id="header-4_4_4">Lab steps to execute OpenSTA with right timing libraries and CTS assignment</h4>

**To remove sky130_fd_sc_hd__clkbuf_1 from the list**

```set ::env(CTS_CLK_BUFFER_LIST) [lreplace $::env(CTS_CLK_BUFFER_LIST) 0 0]```

**To check the current value of CTS_CLK_BUFFER_LIST**

```echo $::env(CTS_CLK_BUFFER_LIST)```

**To check the current value of CURRENT_DEF**

```echo $::env(CURRENT_DEF)```

**To set def as placement def**

```set ::env(CURRENT_DEF) /openLANE_flow/designs/picorv32a/runs/02-04_05-27/results/placement/picorv32a.placement.def```

**To run cts**

```run_cts```

**To check the current value of CTS_CLK_BUFFER_LIST**

```echo $::env(CTS_CLK_BUFFER_LIST)```

### <h4 id="header-4_4_5">Lab steps to observe impact of bigger CTS buffers on setup and hold timing</h4>

Now we will follow the same commands we have used earlier to run OPENROAD,

```openroad```

```read_lef /openLANE_flow/designs/picorv32a/runs/02-04_05-27/tmp/merged.lef```

```read_def /openLANE_flow/designs/picorv32a/runs/02-04_05-27/results/cts/picorv32a.cts.def```

```write_db pico_cts1.db```

```read_db pico_cts.db```

```read_verilog /openLANE_flow/designs/picorv32a/runs/02-04_05-27/results/synthesis/picorv32a.synthesis_cts.v```

```read_liberty $::env(LIB_SYNTH_COMPLETE)```

```link_design picorv32a```

```read_sdc /openLANE_flow/designs/picorv32a/src/my_base.sdc```

```set_propagated_clock [all_clocks]```

```report_checks -path_delay min_max -fields {slew trans net cap input_pins} -format full_clock_expanded -digits 4```

```report_clock_skew -hold```

```report_clock_skew -setup```

```exit```

![image](/assets/149.jpg)

![image](/assets/150.jpg)













## <h5 id="header-5_2">Power Distribution Network and routing</h5>
### <h5 id="header-5_2_1">Lab steps to build power distribution network</h5>

Command for the previous terminal are given bellow

```docker```

```./flow.tcl -interactive```

```package require openlane 0.9```

```prep -design picorv32a -tag 30-03)20-42```

```echo $::env(CURRENT_DEF)```

So, till here we have done CTS and now we are going to do the routing. but before routing we have to generate the PDN(power distribution network)file by using the command. 

```gen_pdn```



It seems like the net VGND displays the total number of nodes on the grid matrix, indicating that it has been successfully created. 

The chip receives power from the VDD and GND pads, which then travels through the tracks and ultimately reaches the cells to power them.






### <h5 id="header-5_2_3">Basics of global and detail routing and configure TritonRoute</h5>

The final step of physical design is Routing.

![image](/assets/148.jpg)

The usage of the ```def``` command in the image above is to indicate that the latest completed step was the generation of PDN. 

The resulting file ```17-pdn.def``` contains the information from ```cts.def``` as well as the power distribution network. 

If one wants to learn about the various switches available for routing, they can refer to the README.md file located in the configuration folder of the OpenLANE directory.



By executing specific commands, we can determine the type of global and detailed routing that will be performed.

In case we want to change the routing type, we can use the ```set``` command followed by the parameter names mentioned in the routing section of the README.md file. 

However, in this instance, the default routing types have been utilized.



Now, we will proceed for routing process by using the command

```run_routing```

![image](/assets/148.jpg)







### <h5 id="header-5_3_4">Routing topology algorithm and final files list post-route</h5>


The algorithm requires the determination of the cost associated with each APC and the calculation of the minimum spanning tree between the APCs to find the optimal points between two APCs. 

The next step involves post-routing STA analysis, which requires the extraction of parasitic effects (SPEF). 

Since OpenLANE does not have a SPEF extraction tool, this process needs to be done outside of OpenLANE. 

The resulting .spef file can be located in the routing folder under the results folder.



![image](/assets/147.jpg)

This is the final generated layout.

![image](/assets/146.PNG)




 