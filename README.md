

# PalletPro - Automated Warehouse Management and Monitoring System

---

## Team  
-  E/19/142, Hashini Illangarathne [email](mailto:e19142@eng.pdn.ac.lk)
-  E/19/264, Pawani Nishantha [email](mailto:e19264@eng.pdn.ac.lk)
-  E/19/304, Sajith Priyankara, [email](mailto:e19304@eng.pdn.ac.lk)
-  E/19/363, Nimnadi Senevirathna [email](mailto:e19363@eng.pdn.ac.lk)
-  E/19/375, Dasun Silva [email](mailto:e19375@eng.pdn.ac.lk)


<!-- Image (photo/drawing of the final hardware) should be here -->

<!-- This is a sample image, to show how to add images to your page. To learn more options, please refer [this](https://projects.ce.pdn.ac.lk/docs/faq/how-to-add-an-image/) -->

<!-- ![Sample Image](./images/sample.png) -->

## Table of Contents
1. [Introduction](#introduction)
2. [Solution Architecture](#solution-architecture )
3. [Hardware & Software Designs](#hardware-and-software-designs)
4. [Testing](#testing)
5. [Detailed budget](#detailed-budget)
6. [Conclusion](#conclusion)
7. [Links](#links)

## Introduction

### About

The world of logistics and warehousing has seen a significant transformation with the integration of automation and robotics. In particular, the use of automated pallet jacks has become increasingly vital for efficient material handling within warehouses, distribution centers, and manufacturing facilities. These automated systems streamline operations by reducing manual labor, enhancing productivity, and ensuring safer working environments.<br><br>
Our project focuses on the design, development, and implementation of an advanced automated pallet jack system. The primary objective is to create a robust, intelligent, and adaptable pallet jack that can autonomously navigate through warehouse environments, pick up, transport, and drop off pallets with precision and efficiency. Incorporating cutting-edge technology and innovative engineering, this project aims to revolutionize material handling processes, contributing to increased operational efficiency and reduced labor costs for businesses.<br>

<p align ="center">
     <img src="docs/asserts/images/WhatsApp Image 2023-11-21 at 20.04.12_2ad850f6.jpg" width=500  />
</p><br>

### Challenges of current system
- Without automated pallet jacks, workers have to do more physical work, which can be tiring and take longer.

- Workers might spend time on simple tasks instead of doing more important jobs that need thinking.

- If a warehouse gets busier, it's harder to handle more goods without hiring lots more people.

- When people move things manually, there might be mistakes or things might not be done the same way each time.

- Moving heavy things can be risky for workers. Even with safety rules, accidents might still happen.

- Proper training for manual pallet jack operation requires time and resources, impacting operational timelines.

- Manual operations might have limitations in speed and efficiency, affecting overall productivity and throughput rates.<br><br>

### Advantages of our system
- Automated pallet jacks work faster and more consistently than manual ones, improving the speed of moving goods from one place to another.

- They decrease the need for human workers to physically move items, freeing up labor for more complex or critical tasks.

- Automated systems are more precise in handling goods, reducing errors and ensuring items are placed or moved accurately.

- They minimize the risk of workplace injuries by reducing manual lifting and handling of heavy items.

- Automated pallet jacks can handle a higher volume of goods in a shorter time, improving overall warehouse productivity.

- Many automated systems can adapt to changes in the warehouse environment or workload, providing flexibility in operations.

- They can be integrated with other systems, such as inventory management or tracking, streamlining warehouse processes and enhancing accuracy.

- Automated pallet jacks can work continuously without breaks, enabling operations to continue around the clock.

- While there's an initial investment, automated systems can lead to long-term cost savings by reducing labor expenses and improving operational efficiency.<br><br>


  
## Solution Architecture
### High level diagram 
<p align ="center">
     <img src="docs/asserts/images/ss.PNG" width=1000  />
</p><br>

The high-level solution architecture for the automated pallet jack comprises three key components.

Ultrasonic Sensors:
- Purpose: Enable obstacle avoidance and mapping.
- Functionality: Emit ultrasonic waves to detect obstacles and map the environment for safe and efficient navigation.
  
Weight Sensors:
- Purpose: Accurately measure the weight loaded onto the pallet jack.
- Functionality: Continuously monitor load weight in real-time, ensuring optimal capacity for safe and efficient material transportation.
  
WiFi Module:
- Purpose: Facilitate precise location tracking.
- Functionality: Scan WiFi beacons and measure signal strength to determine the pallet jack's location, enhancing navigation accuracy.
- But the accuracy of this was quit low than we expected.
- So we decided to use RFID tags for locate the pallet jack.

RFID Tags:
- Purpose: Enable wireless data transmission and facilitate efficient tracking.
- Functionality: RFID tags on pallet jacks emit unique signals when in range of RFID readers placed strategically in the warehouse, allowing for precise and quick 
                 identification of the pallet jack's location within the facility.
  
IR sensors:
- Purpose: Use for optical line following part of the pallet jack.
- Functionality : The IR sensors serve the functionality of detecting and interpreting infrared signals reflected from the floor, enabling the pallet jack to autonomously 
                  follow a predefined path or line.


## Hardware and Software Designs
### Hardware Design
<p align ="center">
     <img src="docs/asserts/images/pp.PNG" width=1000  />
</p><br>
<br>

### Hardware Implementation

<p align ="center">
     <img src="docs/asserts/images/hardware.jpg" width=1000  />
</p><br>
<p align ="center">
     <img src="docs/asserts/images/11.PNG" width=1000  />
</p><br>
<p align ="center">
     <img src="docs/asserts/images/12.PNG" width=1000  />
</p><br>
<p align ="center">
     <img src="docs/asserts/images/13.PNG" width=1000  />
</p><br>
<p align ="center">
     <img src="docs/asserts/images/14.PNG" width=1000  />
</p><br>



## Testing

Software testing using Postman
<p align ="center">
     <img src="docs/asserts/images/Testing using PalletJack.png" width=1000  />
</p><br>

## Hardware Design

<p align ="center">
     <img src="docs/asserts/images/circuit1.png" width=1000  />
</p><br>
<p align ="center">
     <img src="docs/asserts/images/circuit2.png" width=1000  />
</p><br>


## Detailed budget


| Item          | Quantity  | Unit Cost  | Total  |
| ------------- |:---------:|:----------:|-------:|
| ESP32 - Wifi Module   | 1         | 1500 LKR     | 1500 LKR |
| ESP8266 - Wifi Module   | 6         | 700 LKR     | 4200 LKR |
| L298N Motor Driver   | 1         | 430 LKR     | 430 LKR |
| HC-SR04 Ultrasonic Sensor   | 3        | 250 LKR     | 750 LKR |
| Load Cells   | 4        | 300 LKR     | 1200 LKR |
| Motors   | 2         | 3000 LKR     | 6000 LKR |
| Wheels   | 4         | 1000 LKR     | 4000 LKR |
| IR Array   | 1         | 790 LKR     | 790 LKR |
| Thumb joystick   | 1         | 320 LKR     | 320 LKR |
| Jumper wires   | 200         | 5 LKR     | 1000 LKR |
| Other Electronic Materials   | 1         | 2000 LKR     | 2000 LKR |
| Other Non-Electronic Material   | 1         | 3000 LKR     | 3000 LKR |
| Total   |          |      | 25190 LKR |



## Conclusion

What was achieved, future developments, commercialization plans

## Links

- [Project Repository](https://github.com/cepdnaclk/e19-3yp-automated-warehouse-management-and-monitoring-system)
- [Project Page](https://cepdnaclk.github.io/e19-3yp-automated-warehouse-management-and-monitoring-system)
- [Department of Computer Engineering](http://www.ce.pdn.ac.lk/)
- [University of Peradeniya](https://eng.pdn.ac.lk/)

[//]: # (Please refer this to learn more about Markdown syntax)
[//]: # (https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
