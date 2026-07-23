<h1>CONSTRUCTION</h1>
<h2>TOOLS</h2>
<ul>
  <li>soldering iron 
</li> <br>  <img width="171" height="228" alt="0" src="https://github.com/user-attachments/assets/320ebfff-aa36-4ffd-9d0b-f234328d0c13" />   <br> 
    <li>glue gun </li> <br> <img width="171" height="228" alt="IMG_5656" src="https://github.com/user-attachments/assets/2a996236-99f4-4a8b-9e5f-80cd7c6e241c" />  <br>  
 <li>pliers</li>
  <li>screwdrivers</li>
  <li>wire cutters</li>
  <li>electrical tape</li>
  <li>jumper wires</li>
</ul>   
<h2>COMPONENTS</h2>
<ul>
<li><b>AC Motor:</b> an AC motor to simulate the pendulum's oscillation and test the circuit</li>
<li><b>Bridge rectifier:</b> converts an alternating courrent in pulsating direct courrent, we use the diodes 1N5822 </li>
<li><b> Capacitor 1000µF 25V:</b> it absorbe voltage spike and smooth the voltage to obtain a similar DC voltage </li>
<li><b>Buck-Boost LM2577S LM2596S:</b> stabylize the tension on 5 V,the LM2577S act like a boost converter step up the voltage if is too lower and the LM2577S is a buck converter step down the voltage if is too high </li>
<li><b>Solar Panel:</b> generate DC voltage when is exposed to sunlight </li>
<li><b>Schottky diode 1N5822:</b> prevent the return of the courrent on the solar pannel with a low voltage drop</li>
<li><b>TP4056:</b> a module use to safe charging the batteries and monitoring the cells voltage to stay under 4,2V. There is two led the first, the red one, is on if the battery is charging, the second, the blue one, is on if the battery is full charge at 4,2V </li> 
<li><b>18650 cells with the holder:</b> a Li-ion batteries utylize to energy storage. </li> 
</ul> 
<h2>CIRCUIT</h2>
The first thing we want to build is the bridge rectifier. We use four Schottky diodes 1N5822 because we want a low voltage drop ≈ 0,3V. We put two anodes togheter for the DC negative output and two cathodes togheter for the DC positive output, we connect one cathode and one anode for the last two nodes, this is for the positive and negative polarity of the pendulum, as shown in this picture      <br>       
 <br> 
<img width="398" height="426" alt="IMG_5563 (1)" src="https://github.com/user-attachments/assets/4844aa12-62c6-4a07-8b76-ff2b87e9e82b" />
 <br>
  <br> 
For the battery pack we put three cells in parallel because we want a continuous load capability at least 2A (becouse the maximum current of every TP4056 is 1A), every battery can supply up 800mA of courrent 3x800mA=2400mA=2,4A<br>
We want to put on parallel the two sources. The first line consist of: the solar panel, a diode who prevent reverse courrent and a TP4056 who control the charge of the batteries,in this order, we connect all with the jumper wires and after a rapid check we solder all component.<br>
The second line consist of: the AC motor (the pendulum) connected with the bridge rectifier and a capacitor in parallel for smooth the voltage ripple, the buck-boost, pay attention to the output voltage use the screw on the buck-boost to set it to ≈ 5V, the TP4056 connect all with the jumper wires and solder all the component. <br>
Put the two TP4056 on parallel and connect all to the battery pack.<br>
This is the rappresentation. The circuit is do on fritzing, we can see the buck-boost converter is the SDB628 in the reality we use the LM2577S+LM2596S<br><br>

<img width="1876" height="797" alt="image" src="https://github.com/user-attachments/assets/317325f4-4d95-4016-8b85-7f95bdfe9d20" /><br><br>


 The circuit was create using fritzing. You can find the file in this folder and downolad it or use this <a href="https://github.com/andreazerbato04/Nautilus_Marine_Energy_Harvester/blob/main/construction/circuit%20with%20AC%20motor.fzz">link </a> <br>
 If you want to see how the circuit change in respond at the input voltage click this <a href="https://github.com/andreazerbato04/Nautilus_Marine_Energy_Harvester/blob/main/construction/test%20circuit.html">link </a>to see and download the code. You can se how the TP4056 respond on different input voltage from the panel and also from the motor. <br>
<h2>OUR PROTOTYPE</h2>
For our prototype, we put a DC motor for this reason we don't need a bridge rectifire and the capacitor because the voltage is just a DC and not an AC. Another modification concern the diode, for space reason is put on the negative line. The other part of the circuit remain unchanged, first line: solar panel, diode, TP4056 second line: DC motor, buck-boost, TP4056 in this order.<br> We built and tested this prototype, confirming it works, in this picture we can see the red led of the first line illuminated, the DC solar panel line, this is because there is sunlight and the panel is charging the batteries. Moreover, if we apply some mechaincal torque to the DC motor also the red led of the second line light up.<br>We mounted the project with the glue gun to a cardobard to phiscally stabylize and secure the project.<br>Finally, we see the solar panel sold with the specific 5V on peak when there is strong sunlight it reach a peak around 6V, since the high voltage can create problem like shut down or lose of efficency can be an idea place a buck converter.<br><br>
<img width="2016" height="1512" alt="IMG_5668" src="https://github.com/user-attachments/assets/5219df6c-582b-4bef-82bf-45c0047870a9" />
<h2>RESULT</h2>
The bench tests of this prototype confirm that both the solar panel and the AC motor (pendulum) effectively feed the battery pack. We can put this circuit in a buoy and test the performance. <br>
It is importanta to analyze the real performance for compare to the energy we wont for the sensor and scale the solar panel and the pendulum to achive the required energy.
