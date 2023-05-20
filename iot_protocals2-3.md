# **IOT PROTOCOLS**

## **4-20 mA Current Loop**

1.This protocol is widely used in Industries.

2.It takes the sensor data and then further converts it to a current range between 4 and 20 mA

**Working**

1.To understand this circuit first recall **Ohm's Law** **V=IR**

2.The voltage (V) is equal to the current (I) multiplied by the resistance (R).

3.To understand this better take a look on below circuit.

![](https://www.siyavula.com/read/science/grade-11/electric-circuits/images/3f6732ba0e89331314c8939cec082dd2.png)

4.Here 3 resitors are connected in series manner.

5.To drive the electrons around the circuit a certain power supply of known value is connected.

6.Every element in the loop either provides voltage or has a voltage drop. However, the current, "I" is the same everywhere in the loop. This is the critical principle of the 4-20 mA loop. 

To understand this better look at the below picture.

![](https://www.predig.com/sites/default/files/images/Indicator/back_to_basics/4-20mA_Current_Loops/flow_analogy.jpg)

![](https://ni.scene7.com/is/image/ni/Latest_-_01?scl=1)
 
## **Components of 4-20 mA Current Loop**

![](https://www.azom.com/images/Article_Images/ImageForArticle_15057(1).jpg)

1.sensor - Measures a process Variable

2.Transmitter - Convert's sensor's measurment into a current signal

3.power source - It supplies voltage to the circuit

4.Loop - Wire connecting the sensor to the device receiving the 4-20 mA signal and then back to the Transmitter

5.Receiver - Receives and interrpts the current signal.

| Pro's | Con's |
| ------ | ------ |
| The 4-20 mA current loop is the dominant standard in many industries | Current loops can only transmit one particular process signal. |
| It is the simplest option to connect and configure. | Need for isolation equipments increases. |
| It is less sensitive to background electrical noise.| These isolation requirements become exponentially more complicated as the number of loops increases. |
| Better for traveling long distances | High power consumption compared to other analogue signal types |
| simple to detect a fault in the system. | Increasing circuit load resistance, will reduce the supply voltage available to power the transmitter that is generating the 4-20mA signal.

## **ModBUS**

* Modbus is a communication protocol developed by Modicon systems.

* it is a method used for transmitting information over serial lines between electronic devices.

* The device requesting the information is called the Modbus Master and the devices supplying information are Modbus Slaves. In a standard Modbus network, there is one Master and up to 247 Slaves, each with a unique Slave Address from 1 to 247. 

**How it works?**
* Modbus is transmitted over serial lines between devices. 
* The simplest setup would be a single serial cable connecting the serial ports on two devices, a Master and a Slave.
* The data is sent as series of ones and zeroes called bits. Each bit is sent as a voltage. 
* Zeroes are sent as positive voltages and a ones as negative. The bits are sent very quickly. A typical transmission speed is 9600 baud (bits per second).

![](https://www.bb-elec.com/Images/modbus_faq_dia1.aspx)

To read more [Click here](https://realpars.com/modbus-protocol/)

**ModBus has two interfaces**

* ModBus RTU -RS485,RS232
* ModBus TCP/IP- Ethernet

**Modbus RTU**
1.It is a widely accepted serial level protocol due to its ease of use and reliability. 

2.Modbus RTU is widely used within Building Management Systems (BMS) and Industrial Automation Systems (IAS).

3.Modbus RTU messages are a simple 16-bit structure with a CRC (Cyclic-Redundant Checksum).

4.Due to this simplicity, the basic 16-bit Modbus RTU register structure can be used to pack in floating point, tables, ASCII text, queues, and other unrelated data.

5.This protocol primarily uses an RS-232 or RS-485 serial interfaces for communications and is supported by almost every commercial SCADA, HMI, OPC Server and data acquisition software program in the marketplace.

6.RS232 is a interface which is not widely used becuase of its limitiation of only one slave and master

![](https://theautomization.com/wp-content/uploads/2017/10/Modbus-Plant.png)

**RS485**

RS485 is a serial (like UART) transmission standard, you can put several RS485 devices on the same bus.
RS485 is not directly compatible: you must use the correct type of interface, or the signals won't go through. Mainly done through an easy to use an RS485 to USB.

**working**

![](https://www.rs232-to-rs485.com/images/rs232-rs485-connection-example-2.jpg)

The RS485 signals are floating and each signal is transmitted over a Sig+ line and a Sig- line. The RS485 receiver compares the voltage difference between both lines, instead of the absolute voltage level on a signal line.

## **OPC UA**
OPC UA (short for Open Platform Communications United Architecture) is a data exchange standard for industrial communication (machine-to-machine or PC-to-machine communication). 

**Fundamentals**
* It is a client/server based communication
* Here client plays an important role as it decides when and what data should server fetch from client
* It can work as a pub.sub system where client can subsribe to the topic they want.

**Protocols**

OPC UA supports two protocols.

This is visible to application programmers only via changes to the URL. The binary protocol is opc.tcp://Server and http://Server is for Web Service.

 Otherwise OPC UA works completely transparent to the API.

**Advantages**
- Ease-of-use
-  Plug-and-play
-  High reliability and redundancy
-  Enhanced performance
-  Multiplatform support
-  Easy migration plan for existing OPC products to the OPC UA technology.

**Security Model**
* Security Mode
* Selection of cryptographic algorithms
* User authentication
* Certificate and private key storage
* Using certificates
* Managing and maintaining certificates

![](https://www.mc-mc.com/ASSETS/IMAGES/CMS/STATIC_IMAGES/2018/fm/fm-prosoftOPC-prod.jpg)

## **CLOUD PROTOCOLS**

## **MQTT**(Message Queuing Telemetry Transport)

* MQTT is an open OASIS and ISO standard lightweight, publish-subscribe network protocol that transports messages between devices.

**Architecture**

* MQTT runs on top of TCP/IP using a PUSH/SUBSCRIBE topology. In MQTT architecture, there are two types of systems.
1.Clients
2.Brokers
* A broker is the server that the clients communicate with.
* The broker receives communications from clients and sends those communications on to other clients.
*  Clients do not communicate directly with each other, but rather connect to the broker. Each client may be either a publisher, a subscriber, or both.

![](https://hlassets.paessler.com/common/files/infographics/mqtt-architecture.png)
 
 ## **MQTT Message**

Publish – Sends a block of data containing the message to be sent.

Subscribe – Turns a client into a subscriber of a topic. 

PING – A client may ping the broker. 

DISCONNECT – A subscriber or publisher may send a DISCONNECT message to the broker. 

## **HTTP**(Hypertext Transfer Protocol)

* HTTP is a client-server protocol

* HTTP functions as a request-response protocol in the client-server computing model

**Request**

1.Request line
2.HTTP headrs
3.message body

![](https://mdn.mozillademos.org/files/13687/HTTP_Request.png)

Requests consists of the following elements:

* An HTTP method, usually a verb like GET, POST or a noun like OPTIONS or HEAD

* The path of the resource to fetch

* The version of the HTTP protocol.

* Optional headers that convey additional information for the servers.

* Or a body, for some methods like POST, similar to those in responses, which contain the resource sent.

**Response**

Response is made of 3 parts

1.Status line
2.HTTP header
3.Message body

![](https://mdn.mozillademos.org/files/13691/HTTP_Response.png)

Responses consist of the following elements:

* The version of the HTTP protocol they follow.

* A status code, indicating if the request was successful, or not, and why.

* A status message, a non-authoritative short description of the status code.

* HTTP headers, like those for requests.

* Optionally, a body containing the fetched resource.

![](https://gitlab.com/iotiotdotin/project-internship/iotmodule2/-/wikis/uploads/1dcbcc2c7e58e59a042e55b2b2080405/restful-web-services-with-spring-mvc-28-638.jpg)











