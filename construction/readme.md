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
<li><b>TP4056:</b> a chip use to safe charging the bacteries and monitoring the cells voltage to stay under 4,2V </li> 
<li><b>18650 cells with the holder:</b> a Li-ion batteries utylize to energy storage </li> 
</ul>
<h2>CIRCUIT</h2>
The first thing we want to do is the brige rectifier. We put four Schottky diodes 1N5822 becouse we want a low voltage drop ≈ 0,3V. We put two anhode of the diodes on one side and two cathod on the other side like this.
<img width="598" height="640" alt="IMG_5563 (1)" src="https://github.com/user-attachments/assets/4844aa12-62c6-4a07-8b76-ff2b87e9e82b" />
 
We want to put on parallel the two sources. The first line is a
