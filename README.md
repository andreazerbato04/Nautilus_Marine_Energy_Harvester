# Nautilus Marine Energy Harvester #
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Status](https://img.shields.io/badge/Status-Prototype-orange) <br>
The Nautilus project is an open source,hybrid power buoy designed for autonomous monitoring of water, in specific this project is built for the condition of the Venice lagoon. <br>This project combine a pendulum and a solar panel two system give renewable energy to a single harvesting system, this system supplies power to a sensor, which provide real time data collecting without requiring frequent battery replecment or costly maintenace trip. This data is very important because the Venice lagoon and the city are very fragile, and is important to track a lot of information like the pH level the height of the water and the power of the wave. <br>
As an open source platform, Nautilus is designed for collaborative development. All information and file like the circuit and the costruction are open to the community and anyone is free to add more files.
<h2>BUOY ARCHITECTURE</h2>
The two sources combined provide energy to a battery pack, the battery peak combined three Li-ion batteries. This circuit can provide 365 day operational autonomy despite seasonal weather change and this is very important to track any change in the Venice lagoon.<br><br> <br><pre><code>
 ┌───────────────────────────┐         ┌───────────────────────────┐
 │   Solar Panel + Diode     │         │ Electromagnetic Pendulum  │
 └─────────────┬─────────────┘         └─────────────┬─────────────┘
               │                                     │ (AC)
               │                                     ▼
               │                       ┌───────────────────────────┐
               │                       │      AC-DC Rectifier      │
               │                       └─────────────┬─────────────┘
               │                                     │ (DC)
               │                                     ▼
               │                       ┌───────────────────────────┐
               │                       │    DC-DC Buck-Boost       │
               │                       └─────────────┬─────────────┘
               │                                     │
               └───────────────────┬─────────────────┘
                                   │
                                   ▼
                     ┌───────────────────────────┐
                     │ TP4056 Charge Controller  │
                     └─────────────┬─────────────┘
                                   │
                                   ▼
                     ┌───────────────────────────┐
                     │   3x 18650 Battery Pack   │
                     └─────────────┬─────────────┘
                                   │
                                   ▼
                     ┌───────────────────────────┐
                     │     ESP32 Sensor Node     │
                     └───────────────────────────┘
</code></pre>
<h2>REPOSITORY STRUCTURE</h2>
<ul><li>
 <b>assembly:</b> mechanical documentation, circuit diagram and assembling project
</li>
<li>
 <b>component:</b> link to the product and cost of component
</li>
<li>
 <b>concept:</b> hybrid architecture breakdown and theoretical information
</li>
<li>
 <b>future work:</b> planning future work and upgrading part
</li>
<li>
 <b>location:</b> Vanice lagoon deployment analysis and site condition
</li>
<li>
 <b>reference:</b> accademic papers and background literature
</li>
<li>
 <b>readme.md:</b> main repository overview
</li></ul>
