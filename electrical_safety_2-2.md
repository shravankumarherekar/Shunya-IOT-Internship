# **Board Electrical Safety Tips**

## **Electrical Safety**
Electrical safety is a system of organizational measures and technical means to prevent harmful and dangerous effects on workers from electric current, electric arc, electromagnetic field and static electricity.



![](https://image3.slideserve.com/6741531/electrical-safety-n.jpg)


**Power Supply**

| Do's | Dont's |
| ------ | ------ |
| Make sure that the output voltage of the power supply matches the input voltage of the board | Do not connect power supply without matching the power rating |
| While turning on the power supply make sure every circuit is connected properly | Never connect a higher output(12V/3Amp) to a lower (5V/2Amp) input |
| Keep all electrical circuit contact points enclosed | Do not store liquids of any sort near electrical equipment |
| When working on electrical devices, only use tools that have official “non-conducting” handles | Do not wear metal of any sort if you are working on electrical equipment |

![](https://www.highspeedtraining.co.uk/hub/wp-content/uploads/2014/01/electrical-hazard-warning-signs.jpg)

## **Handling**

**Do's**

* Treat every device like it is energized, even if it does not look like it is plugged in or operational.
* While working keep the board on a flat stable surface (wooden table) .
* Unplug the device before performing any operation on them.
* When handling electrical equipment, make sure your hands are dry.
* Keep all electrical circuit contact points enclosed.
* If the board becomes too hot try to cool it with a external usb fan .

**Dont's**
* Don’t handle the board when its powered ON.
* Never touch electrical equipment when any part of your body is wet, (that includes fair amounts of perspiration).
* Do not touch any sort of metal to the development board.


![](https://i.pinimg.com/originals/5e/be/e7/5ebee7db77f1cdd81bb3d1614cbc8fb9.png)
## **GPIO**
| Do's | Don’ts |
| ------ | ------ |
| Find out whether the board runs on 3.3v or 5v logic | Never connect anything greater that 5v to a 3.3v pin |
| Always connect the LED (or sensors) using appropriate resistors .| Avoid making connections when the board is running 
| To Use 5V peripherals with 3.3V we require a logic level converter. | Do not connect a motor directly , use a transistor to drive it,Don't plug anything with a high (or negative) voltage |

## **Guidelines for using interfaces**

## **UART**
* Both UARTs must operate at about the same baud rate. 
* The baud rate between the transmitting and receiving UARTs can only differ by about 10% before the timing of bits gets too far off.
* Both UARTs must also must be configured to transmit and receive the same data packet structure.
* Connect Rx pin of device1 to Tx pin of device2 ,similarly Tx pin of device1 to Rx pin of device2.
* If the device1 works on 5v and device2 works at 3.3v then use the level shifting mechanism(voltage divider )
* Genrally UART is used to communicate with board through USB to TTL connection . USB to TTL connection does not require a protection circuit .
* Whereas Senor interfacing using UART might require a protection circuit.

![](https://www.circuitbasics.com/wp-content/uploads/2016/01/Introduction-to-UART-Data-Transmission-Diagram.png)

## **I2C**

* The Inter-Integrated Circuit (I2C) Protocol is a protocol intended to allow multiple "slave" digital integrated circuits ("chips") to communicate with one or more "master" chips.
* In I2C, communication is always started by the master.
* The default state of SDA and SCL line is high.
* A high to low transition of SDA line while the SCL line is high called the **START condition.**
*  A Low to high transition of SDA line while the SCL line is high called the **STOP condition.**
* while using I2c interfaces with sensors SDA and SDL lines must be protected.
* Protection of these lines is done by using pullup registers on both lines.
* If you use the inbuilt pullup registers in the board you wont need an external circuit.
* if you are using bread-board to connect your sensor , use the pullup resistor .

![](https://cdn.sparkfun.com/r/600-600/assets/3/d/1/b/6/51adfda8ce395f151b000000.png)

## **SPI**

* The SPI is normally used for communication between the device and external peripherals.
* The Serial Peripheral Interface is a synchronous serial communication interface specification used for short-distance communication, primarily in embedded systems.
* SPI devices communicate in full duplex mode using a master-slave architecture with a single master.
* Generally ,Spi in development boards is in Push-pull mode.
* Push-pull mode does not require any protection circuit.



![](https://www.totalphase.com/support/article_attachments/200063846/spi-diagram.png)

[**Documentation by Shravan**]()



