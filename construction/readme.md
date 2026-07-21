<h1>CONSTRUCTION</h1>
<h2>TOOLS</h2>
<ul>
  <li>soldering iron
</li> <img width="171" height="228" alt="0" src="https://github.com/user-attachments/assets/320ebfff-aa36-4ffd-9d0b-f234328d0c13" />
   <li>glue gun</li><img width="171" height="228" alt="IMG_5656" src="https://github.com/user-attachments/assets/2a996236-99f4-4a8b-9e5f-80cd7c6e241c" />
<li>pliers</li>
  <li>screwdrivers</li>
  <li>wire cutters</li>
  <li>electrical tape</li>
  <li>jumper wires</li>
</ul>
<h2>COMPONENTS</h2>
<ul>
<li><b>AC Motor:</b> an AC motor to simulate the pendolum's oscillation and test the circuit</li>
<li><b>Bridge rectifier:</b> converts an alternating courrent in pulsating direct courrent, we use the diodes 1N5822 </li>
<li><b> Capacitor 1000µF 25V:</b> it absorbe voltage spike and smooth the voltage to obtain a similar DC voltage </li>
<li><b>Buck-Boost LM2577S LM2596S:</b> stabylize the tension on 5 V,the LM2577S act like a boost converter step up the voltage if is too lower and the LM2577S is a buck converter step down the voltage if is too high </li>
<li><b>Solar Pannel:</b> generate DC courrent when is exposed to sunlight </li>
<li><b>Schottky diode 1N5822:</b> prevent the return of the courrent on the solar pannel with a low voltage drop</li>
<li><b>TP4056:</b> a module use to safe charging the batteries and monitoring the cells voltage to stay under 4,2V. There is two led the first the red one is on if the bactery is on charge the second the blue one is on if the battery is full charge at 4,2V </li> 
<li><b>18650 cells with the holder:</b> a Li-ion batteries utylize to energy storage </li> 
</ul>
<h2>CIRCUIT</h2>
The first thing we want to build is the bridge rectifier. We use four Schottky diodes 1N5822 because we want a low voltage drop ≈ 0,3V. We put two anodes togheter for the DC negative output and two cathodes togheter for the DC positive output, we connect one cathodes and one anodes for the last two nodes, this is the entrance of the pendolum, as shown in this picture      <br>       
 <br> 
<img width="398" height="426" alt="IMG_5563 (1)" src="https://github.com/user-attachments/assets/4844aa12-62c6-4a07-8b76-ff2b87e9e82b" />
 <br>
  <br> 
For the battery pack we put three cells on parallel becouse we want a continuous load capability at least of 2A (becouse the maximum courrent of every TP4056 is 1A), every batterie can supply up 800mA of courrent 3x800mA=2400mA=2,4A<br>
We want to put on parallel the two sources. The first line is the solar pannel a dioed who prevent reverse courrent and a TP4056 who control the charge of the batteries, we connect all with the jumper wires and after this solder every peace.<br>
The second line is the AC motor (the pendolum) connected with the bridge rectifire after this we put the buck-boost, keep attention about the output voltage use the screw on the buck-boost to set on ≈ 5V, after this we connect the TP4056 connect all with the jumper wires and the sold all the pieces. <br>
Put the two TP4056 on parallel and connect all to the battery pack.
