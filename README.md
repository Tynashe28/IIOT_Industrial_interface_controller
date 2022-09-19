# IIOT_Industrial_interface_controller

## Introduction

Remote monitoring and controlling systems are designed to collect data about the operations of any given unit or transmit information to the unit to transform its behavior via the cloud. You benefit from leveraging the Industrial Internet of Things (IIoT). OEMs, end-users and systems integrators have already seen the benefits of implementing a remote monitoring system that lead to increased productivity, reduced production costs and enhanced user experience.

Drakula is an Industrial Internet of Things gateway controller which seeks to connect manufacturing processes to the internet with zero effort and unleash the usefulness and power of technology in this field at zero cost. This controller makes it easy for industries to leverage trending and growing technologies like machine learning, IoT, blockchain, web backend services into their day to day operations. The beauty about Drakula is that it integrates on top of existing architectures and virtually no change can be made to existing setups to accommodate it.  

![intro image](https://github.com/Tynashe28/IIOT_Industrial_interface_controller/blob/main/images/Drakula.png/)

### Core Values
•	Zero Effort\
•	Zero Cost\
•	Interactive\
•	Value Addition

## How it works

![how it works image](https://github.com/Tynashe28/IIOT_Industrial_interface_controller/blob/main/images/1.PNG/)

From a high level, the Drakula connects to the plant process and it accesses field parameters about a manufacturing process. It can also be granted privileges to write data to alter the behavior of processes within the plant. Drakula relays this information to a cloud platform via an API where data analytics can also be done.

The ability of this controller to access field parameters and make them accessible over the web opens vast opportunities for manufacturing processes.

![middle functions](https://github.com/Tynashe28/IIOT_Industrial_interface_controller/blob/main/images/2.PNG/)

•	Information can be relayed to mobile phones, desktop or smart watches.\
•	Interacting with manufacturing processes just becomes easy through our day to day devices.\
•	Implementing sophisticated algorithms which can never be done on PLCs’ in the cloud to improve processes.\
•	Ability to build intuitive and interactive SCADA dashboards which can never be offered by PLCs\

### Example Use Case
Let’s take a practical example of defects after “beer” filling 😃. We can make use of the real time number defects of the filler to come up with the REAL-TIME STATE OF THE MACHINE. We can also produce predictions of the number of defects after some time “x” which can open doors to generate a predictive maintenance schedule for the machine.

![Use case example](https://github.com/Tynashe28/IIOT_Industrial_interface_controller/blob/main/images/3.PNG/)

## Motivation in Building This Product
•	All most every software and hardware used in industry is highly proprietary to the company that provides that piece of hardware or software. These services come at a hefty amount which leaves us with no room to be innovative with their products as most companies cannot afford. Building a product for less than USD50 to counter this problem should be enough to motivate engineers to start get their hands dirty with these technologies.

•	A PLC is very excellent at the job it was made for. Problems start when you try to perform computations which require more memory or power from the system like training a Machine Learning model. It even gets more complicated than rocket science when you try to perform a simple HTTP request to the internet from a PLC. One of the core values of Drakula is Zero Effort, you don’t have to worry about the low-level implementations of establishing internet connection. Offering this abstraction layer makes engineers focus more on the task to be achieved rather than implementation details.


•	The way reports are generated in industry today is just primitive, data is organized either at end of a shift or day, meaning we don’t get to visualize real-time plant performances. Manufacturing should be also powered by Interactive and Real-time dashboards.

•	A lot of technologies are being developed over the Internet which can be harnessed in operations and processes to increase manufacturing efficiencies and business profitability

## Considerations made into the design

•	Interoperable – Drakula is compatible with almost every industrial setup. It runs in parallel with existing architectures. Taking advantage that every industrial PLC has a communication channel which can be used as desired with no restriction, forms the point of connectivity for the devices.

•	Robust – Controller components to handle high temperatures, voltage fluctuations, electromagnetic interference and induction.

•	Reliability – Additional components to a system has a consequence of reducing the overall reliability of a process. This controller has been designed in a way that it runs in parallel with the overall plant process in a bid to make the controller have zero effect on the plant process in case of a failure. 

•	Hardware Abstraction – Developers implementing this board should have easy ability to integrate this controller. This is made possible by providing ready-to-use drivers which do all low-level heavy lifting.

•	Security & Industrial Standards – The security of a system is as good as its weakest point. This controller aims to keep the integrity of the data that it is processing. Every web request is done via Web-Sockets over HTTPS. Every component used on the controller is accredited to be industrial grade.

•	Overall System Efficiency – Drakula’s main CPU is a high-performance processor which runs a real-time operating system which manages all tasks and this makes sure the system is seamless and operates without any lag.

•	Maintainability – Ability of controller to connect to Wi-Fi access points gives it the ability to be maintained over the air, incase of software updates and troubleshooting. Incase of a hardware fault, the device can be disconnected from the system without affecting the main production processes.

•	Cost – The total cost of producing 1 controller excluding Labour and Tooling is capped at maximum of USD50.00 (PCB Manufacturing, Components and Assembly).

## Why Implement Drakula

### Improve Productivity
Overall Equipment Effectiveness, or OEE, is a productivity measurement that combines downtime, production rate and quality. OEE has long been the gold standard for increasing productivity, but the Industrial Internet of Things has made OEE much more affordable and easier to implement than ever before. 

### Information at Your Fingertips
Line operators, maintenance crews and production supervisors all have a significant impact on the productivity of the manufacturing lines. Without information readily available, it is more difficult to address the highest priority production issues within a timely manner.

### Data Reliability
It’s very common to see people using clipboards to copy data from gauges, operator interface screens or field sensors. Automated data collection is more efficient, more reliable and more consistent than manual data collection. The IIoT can provide seamless data flow starting at the device level and pushing the data directly to mobile devices, enterprise level software or other reporting systems.

### Reduce Downtime
Emails, push notifications and text alerts can provide immediate downtime alerts allowing you to address the issue as quickly as possible.  Root cause analysis allows you to diagnose the specific cause of a downtime event, and downtime analytics allow you to evaluate the true cost of each type of failure.  A remote monitoring solution is an easy and cost-effective way to incorporate all of these techniques to increase the reliability of your equipment.

### Predictive Maintenance
Predictive maintenance techniques can be used to monitor and analyze vibration, motor current, or temperature patterns and identify potential problems before they cause a shutdown. This can also reduce maintenance costs because maintenance can be performed when it is actually needed rather than simply scheduled.

### Intuitive Dashboards
Your car’s dashboard can tell you the remaining oil life, miles to empty, temperature, and more. Manufacturing lines need much more maintenance than a car, but required maintenance is usually not available from the equipment. User friendly dashboards on mobile and desktop apps also provide quick and easy way to visualize the whole plant.

## General System Architecture

![Architecture image](https://github.com/Tynashe28/IIOT_Industrial_interface_controller/blob/main/images/4.PNG/)

### Main-Features
•	Supports all Ethernet communications (Modbus, Profinet, TCP etc.)\
•	Supports Modbus over RS-485\
•	Wi-Fi connectivity (Supports WebSocket connection)\
•	Bi-Directional Communication\
•	Asynchronous and Non-Blocking routines\
•	3 logical Processing Cores
