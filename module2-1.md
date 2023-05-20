# **Basic Electronics for Embedded**

* **Sensors and Actuators**
* **Analog and Digital**
* **Micro-controllers Vs Micro-processors**
* **Introduction to Raspberry Pi**
* **Serial and Parallel**

## **Sensors**
A device which detects or measures a physical property and records, indicates, or otherwise responds to it.

For Example : A microphone is a sensor that takes vibrational energy (sound waves), and converts it to electrical signal for the system to relate it back to the original sound.
sensor is essentially a transducer that converts some form of energy into an electrical signal which upon processing is used to take a reading.

![](https://circuitdigest.com/sites/default/files/projectimage_tut/Basic-Sensors.jpg)

## **Actutators**
A device that causes a machine or other device to operate.

For example: an electric motor, a hydraulic system, and a pneumatic system are all different types of actuators.
![](https://qphs.fs.quoracdn.net/main-qimg-915195d635b850b1d45a42967ffafffc)
![](https://image1.slideserve.com/2043207/types-of-actuators-l.jpg)
## **Sensors Vs Actuators**
![](https://www.avsystem.com/media/top_sensor_types_used_in_iot-02.png)

![](https://microcontrollerslab.com/wp-content/uploads/2019/02/Difference-between-sensors-and-actuators.gif)

# **Analog Vs Digital**



| Analog | Digital |
| ------ | ------ |
| Continuous signals | Discrete signals |
| Represented by sine waves |Represented by square waves  |
| Human voice, natural sound, analog electronic devices are few examples | Computers, optical drives, and other electronic devices |
| Continuous range of values | Discontinuous values |
| Records sound waves as they are | Converts into a binary waveform |
| Only be used in analog devices. | Suited for digital electronics like computers, mobiles and more. |
| ![](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcS7yXp0gxfIQ3mqY0rg-2ZMKErvj0iNidp4BQ&usqp=CAU) | ![](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRT0ZjPnXFQS5pmQxofJ_WmTsA44fbxpJinSg&usqp=CAU) |

![](https://techdifferences.com/wp-content/uploads/2016/08/Analog-Signal-Vs-digital-Signal.jpg) 

# **Microprocessor Vs Microcontroller**
![](https://components101.com/sites/default/files/components/Difference-between-Microprocessor-and-Microcontroller.jpg)

| Microprocessor | Microcontroller |
| ------ | ------ |
| It is used in an application where the task is not predefined and it is assigned by the user. | Micro-controllers are used to do the same assigned task repeatedly. |
| High power consumption | Low power consumption |
| General Purpose | Single Purpose |
| Microprocessors are basic components of personal computers | Microcontrollers are generally used in embedded systems |
| A microprocessor based system can perform numerous tasks | A microcontroller based system can perform single or very few tasks |
![](https://rh6stzxdcl1wf9gj1fkj14uc-wpengine.netdna-ssl.com/wp-content/uploads/2017/10/Fig-1-MicrocontrollerMicroprocesser-300x167-1.png)

# **Raspberry Pi**
The Raspberry Pi is a series of small single-board computers developed in the United Kingdom by the Raspberry Pi Foundation to promote teaching of basic computer science in schools and in developing countries. 

* Mini Computer
* Limited but large power for its size
* No storage
* It is a SOC (System On Chip)
* We can connect shields (Shields - addon functionalities)
* Can connect multiple Pi’s together
* Microprocessor
* Can load a linux OS on it
* Pi uses ARM
* Connect to sensors or actuators

To know more about Raspberry Pi  [read here](https://www.raspberrypi.org/)


**Serial Interfaces**
Uses a single wire to transfer the data bits one at a time.
For example, UART, SPI, I2C, etc.

**Parallel Interfaces**
Uses multiple wires running parallel to each other, and can transmit data on all the wires simultaneously.
For example, GPIO interfaces.
![](https://projects-static.raspberrypi.org/projects/raspberry-pi-getting-started/0e07cfe2a142a41e6c97611e94057de6dddde935/en/images/pi-labelled-names.png)

## **Serial Vs Parallel**
| Serialcommunication | Parallel communication |
| ------ | ------ |
| Data is transmitted bit after the bit in a single line| Data is transmitted simultaneously through group of lines(bus) |
| Data congestion takes place | No congestion takes place |
| Low speed transmission | High speed transmission |
| The bandwith of serial wires is much higher | The bandwith of parallel wires is lower |
| good for longer distance | Good for Shortest distance |
| Work effectively even at high frequencies | Parallel buses are hard  to run at high frequencies |
| The circuit used in Serial Transmission is simple. | The circuit used in Parallel Transmission is relatively complex. |


![](https://techdifferences.com/wp-content/uploads/2016/04/Untitled.jpg)


[**Documentation by shravan**](https://gitlab.com/K_shravan_kumar)


