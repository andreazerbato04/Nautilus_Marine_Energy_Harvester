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
<li><b>Solar Panel:</b> generate DC courrent when is exposed to sunlight </li>
<li><b>Schottky diode 1N5822:</b> prevent the return of the courrent on the solar pannel with a low voltage drop</li>
<li><b>TP4056:</b> a module use to safe charging the batteries and monitoring the cells voltage to stay under 4,2V. There is two led the first the red one is on if the bactery is on charge the second the blue one is on if the battery is full charge at 4,2V </li> 
<li><b>18650 cells with the holder:</b> a Li-ion batteries utylize to energy storage </li> 
</ul>
<h2>CIRCUIT</h2>
The first thing we want to build is the bridge rectifier. We use four Schottky diodes 1N5822 because we want a low voltage drop ≈ 0,3V. We put two anodes togheter for the DC negative output and two cathodes togheter for the DC positive output, we connect one cathode and one anode for the last two nodes, this is for the positive and negative polarity of the pendulum, as shown in this picture      <br>       
 <br> 
<img width="398" height="426" alt="IMG_5563 (1)" src="https://github.com/user-attachments/assets/4844aa12-62c6-4a07-8b76-ff2b87e9e82b" />
 <br>
  <br> 
For the battery pack we put three cells in parallel because we want a continuous load capability at least 2A (becouse the maximum current of every TP4056 is 1A), every battery can supply up 800mA of courrent 3x800mA=2400mA=2,4A<br>
We want to put on parallel the two sources. The first line is the solar panel a dioed who prevent reverse courrent and a TP4056 who control the charge of the batteries, we connect all with the jumper wires and after this solder all component.<br>
The second line is the AC motor (the pendulum) connected with the bridge rectifier after this we put the buck-boost, pay attention to the output voltage use the screw on the buck-boost to set it to ≈ 5V, after this we connect the TP4056 connect all with the jumper wires and the solder all the component. <br>
Put the two TP4056 on parallel and connect all to the battery pack.<br>
This is the rappresentation. The circuit is do on fritzing.<br><br>
<img width="1632" height="777" alt="image" src="https://github.com/user-attachments/assets/22fce282-cb86-4b7f-bb91-088a20881fcb" /><br><br>
 The circuit was create fritzing. You can find the file in this folder and downolad it. <a href="https://it.aliexpress.com/item/1005005433899955.html?spm=a2g0o.detail.pcDetailTopMoreOtherSeller.3.74b6bYoubYouSK&gps-id=pcDetailTopMoreOtherSeller&scm=1007.40050.354490.0&scm_id=1007.40050.354490.0&scm-url=1007.40050.354490.0&pvid=e8b352cc-9b29-4987-93db-09e84d06d329&_t=gps-id%3ApcDetailTopMoreOtherSeller%2Cscm-url%3A1007.40050.354490.0%2Cpvid%3Ae8b352cc-9b29-4987-93db-09e84d06d329%2Ctpp_buckets%3A668%232846%238113%231998&pdp_ext_f=%7B%22order%22%3A%2224%22%2C%22eval%22%3A%221%22%2C%22sceneId%22%3A%2230050%22%2C%22fromPage%22%3A%22recommend%22%7D&pdp_npi=6%40dis%21EUR%214.16%210.87%21%21%214.72%210.99%21%402103828617806747149295705e10fe%2112000033058635923%21rec%21IT%21%21ABX%211%210%21n_tag%3A-29910%3Bd%3A20a12571%3Bm03_new_user%3A-29895%3BpisId%3A5000000207395220&utparam-url=scene%3ApcDetailTopMoreOtherSeller%7Cquery_from%3A%7Cx_object_id%3A1005005433899955%7C_p_origin_prod%3A">Buy it</a>
<h2>OUR PROTOTYPE</h2>
