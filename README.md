# Nautilus Marine Energy Harvester #
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Status](https://img.shields.io/badge/Status-Prototype-orange) <br>
The Nautiuls project is an open source,hybrid power buoy designed for autonomous monitoring of water, in specific this project is build for the condition of the Venice lagoon. <br>This project combine a pendulum and a solar panel two system give renewable energy to a single harvesting system, this system supplie power to a sensor, who provide real time data collecting without requiring frequent battery replecment or costly maintenace trip. This data is very important beocuse the Vencice lagoon and the city are very fragile, and is important to track a lot of information like the pH level the height of the water and the power of the wave. <br>
As an open source platform, Nautilus is designed for collaborative develpoment. All information and file like the circuit and the costruction are open to the community and anyone is free to add more file.
<h2>BUOY ARCHITECTURE</h2>
The two source combined provide energy to a battery peak, the battery peak combined three Li-ion battery. This circuit can provide 365 day operational autonomy and this is very important to track any change in the Venice lagoon.<br><br> <br><pre><code>
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

