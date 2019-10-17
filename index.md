# Smart Bathroom

**Course**: 12740

**Group ID** : AL

**Group Member**: Xinmiao Liu; Mengmeng Pan; Yuanpeng Cao; Peng Zeng

### [Progress report 1 （9.28）](https://github.com/yuanpenc/Yuanpeng.github.io/blob/master/progress%20report/progress%20report%201(9.28).md)
### [Video]()

## Introduction
With the rapid development of science and technology, our life is becoming more and more convenient, the intelligent level of household is also improving. The bathroom, a place we use every day, naturally attracts us to make more efforts to make it smarter. 

Our project aims to create a better bathing environment through ‘smart fans’ and ‘smart lights’. The ‘smart fan’ can switch on and off automatically. So, we don't have to worry about forgetting to turn off the fan after a shower. Many people like to play music in the shower, our ‘smart light’ will flash to the rhythm of music, which make your shower time more fun.


## Motivation
When taking a bath, the humidity inside the bathroom will rise. Therefore, no matter when bathing or after bathing should be timely ventilation, that is, should let air flow. This is especially important to the elderly and children to assure their breath open when taking bath. Meanwhile, the moist environment is a breeding ground for bacteria. Accordingly, it is very necessary that let the bathroom return dry and clean as soon as possible. But it takes a while for the bathroom to get dry again, and sometimes people may forget to turn off the fan, so it would be nice if the fan could automatically turn off when the bathroom returns dry. Taking shower is usually boring, and bathrooms are often decorated in a simple style. Our ‘smart lights’ will make the bathroom more colorful, and the flashing lights along with the rhythm makes shower time fun.

## Specific Goals
The overall goal of our project is to use temperature and humidity sensor to detect the humidity in the bathroom and control the switch of the fans through the relay module. Also, sound detection sensor to detect the music sound that plays while you are in the shower.
The specific goals to be achieved in the process of reaching the final goal are as follows:

* Using a sound detect sensor to detect the playing music. 
* Using DHT11 to detect the humidity and temperature in the environment.
* Using codes to let DHT11 control the switch of fans.
*	Connect all the sensors and actuators to the raspberry pi simultaneously.

# For progress report

## Current Progress
We learnt how to connect the Temperature and & Humidity Sensor Module to the Raspberry pi and test it to get some data through Adafruit.


<p><![image](https://user-images.githubusercontent.com/55899142/65842276-61145500-e2f8-11e9-9516-e40d15a4782c.png)></p>


The figure below shows what we connect DHT11 to Raspberry Pi.

![image](https://user-images.githubusercontent.com/55899142/65842366-16dfa380-e2f9-11e9-8db9-3f5d33ddacee.png)

This is how we connect DHT11 and CZN15E to Raspberry Pi.

![image](https://user-images.githubusercontent.com/55899142/65842421-658d3d80-e2f9-11e9-8a61-b1206f1710d5.png)

This is the code to sample data.

![image](https://user-images.githubusercontent.com/55899142/65842463-cd438880-e2f9-11e9-9462-57326dc6fab4.png)



## Problems Encountered
* Coding is complex, we need to keep debugging it.
* We cannot find the datasheet of the Sound Detection Sensor CNZ15E.
* We don't know how to connect two sensors to the Raspberry pi simultaneously.
* We cannot obtain datum from the Humidity Sensor Module. 

![image](https://user-images.githubusercontent.com/55899142/65842630-d84ae880-e2fa-11e9-9137-83ec19d3b4a4.png)

![image](https://user-images.githubusercontent.com/55899142/65842701-50191300-e2fb-11e9-9c07-b612a381fe75.png)

## Future Plan
* Keep improving our code.
* Connect the lines correctly and completely and test them.

# Methodology
## Phenomena of Interest
### Physical principles
The relative humidity (RH) of an air–water mixture is defined as the ratio of the partial pressure of water vapor in the mixture to the equilibrium vapor pressure of water over a flat surface of pure water at a given temperature. It is normally expressed as a percentage; a higher percentage means that the air–water mixture is more humid. At 100% relative humidity, the air is saturated and is at its dewpoint.
Sound is represented by audio signal, typically using a level of electrical voltage for analog signals, and a series of binary numbers for digital signals. Audio signals have frequencies in the audio frequency range of roughly 20 to 20,000 Hz, which corresponds to the lower and upper limits of human hearing.
### Statistic and Dynamic Behavior
Humidity is a dynamic characteristic in that the water content in air is dynamic. In addition,  the unit of humidity we used is relative humidity. Relative humidity (RH) is the ratio of the partial pressure of water vapor to the equilibrium vapor pressure of water at a given temperature. Relative humidity depends on temperature and the pressure of the system of interest.
A sound signal is an example of a continuous signal that is sampled to result in a discrete signal. In this case, sound waves traveling through the air are recorded as a set of measurements that can then be used to reconstruct the original sound signal, as closely as possible. The sampling rate or sampling frequency is the number of samples taken per time unit, for example, per second. Sound signals are usually measured in Hertz (Hz).Signal Characteristics
### Signal Characteristic
Humidity signal: When the sensor is in the presence of water vapor it is absorbed, causing the functional ionic groups to disassociate, and resulting in increased conductivity. Response times are slow ranging from 10 to 30 s for a 63 percent step change. Most resistive sensors use an AC excitation to prevent sensor polarization. The resulting current is rectified and converted to DC where it can then undergo linearization and be amplified as necessary. The AC signal applied to the bridge ranges from 30 Hz to 10 kHz. As an example consider the TDK CHS series of integrated resistive humidity sensors with voltage output.
Music signals is a type of sound that has some stable frequencies in a time period. Music can be more complicated than human vocal sound, occupying a wider band of frequency. Music signals are time-varying signals; while the classic Fourier transform is not sufficient to analyze them, time–frequency analysis is an efficient tool for such use. Time–frequency analysis is extended from the classic Fourier approach. Short-time Fourier transform (STFT), Gabor transform (GT) and Wigner distribution function (WDF) are famous time–frequency methods, useful for analyzing music signals such as notes played on a piano, a flute or a guitar.

## Sensor(s) Used
### Physical Principles:
* DHT11: It is a type of resistive humidity sensors that measure the resistance conductivity. The principle is the fact that the conductivity in non-metallic conductors is dependent on their water content. The resistive humidity sensor is made up of materials with relatively low resistivity and resistivity changes significantly with changes in humidity. The relationship between resistance and humidity is inverse exponential. The measurement range is 20-90%RH, temperature measurement range is 0-50℃.
* CZN15E: 

### Static and Dynamic Behavior 
* DHT11: This sensor includes a resistive-type humidity measurement component and an NTC temperature measurement component, and connects to a high- performance 8-bit microcontroller, offering excellent quality, fast response, anti-interference ability and cost-effectiveness. Applying the DHT11 sensor beyond its working range stated in this datasheet can result in 3%RH signal shift/discrepancy. The DHT11 sensor can recover to the calibrated status gradually when it gets back to the normal operating condition and works within its range. 
* CZN15E: 
### Sensor Characteristics
* DHT11:

![image](https://user-images.githubusercontent.com/55899142/65845050-9f187580-e306-11e9-923b-ffbff0fd51d3.png)

* CZN15E:

