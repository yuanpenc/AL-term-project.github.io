# Smart Bathroom
Xinmiao Liu; Mengmeng Pan; Yuanpeng Cao; Peng Zeng

## Introduction
Our project aims to create a better bathing environment. We use the humidity sensor to detect the humidity in the bathroom and control the switch of the fan and the sound detection sensor to create lights to accompany with music.

## Motivation
When taking a bath, the humidity inside the bathroom will rise. Therefore, no matter when bathing or after bathing should be timely ventilation, that is, should let air flow. This is especially important to the elderly and children to assure their breath open when taking bath. Meanwhile, the moist environment is a breeding ground for bacteria. Accordingly, it is very necessary that let the bathroom return dry and clean as soon as possible. But it takes a while for the bathroom to get dry again, and sometimes people may forget to turn off the fan, so it would be nice if the fan could automatically turn off when the bathroom returns dry. Also, having a bath with music is a pleasure. It would be better if you could play music with cool lighting.

## Goals
* Our goal is to understand the capabilities of the sensors used, implement the concepts learned during the data acquisition process, and learn how to integrate sensors as components into larger systems. 
* Learn how to use humidity sensors to control fan switches.
* Learn how to let the lights flash according to music with sound detection sensor.

# For progress report

## Current Progress
We learnt how to connect the Temperature and & Humidity Sensor Module to the Raspberry pi and test it to get some data through Adafruit.
<p align="center">
  <img src="./img/pr11/WeChat Image_20191015140900.png" width="700">
</p>

The figure below shows what we connect DHT11 to Raspberry Pi.


<p align="center">
  <img src="/img/pr11/circuit1.jpg" width="500">
</p>

This is how we connect DHT11 and CZN15E to Raspberry Pi.

<p align="center">
  <img src="/img/pr11/picture.jpg" width="600">
</p>

This is the code to sample data.

<p align="center">
  <img src="/img/pr11/code1.png" width="600">
</p>


## Problems Encountered
* Coding is complex, we need to keep debugging it.
* We cannot find the datasheet of the Sound Detection Sensor CNZ15E.
* We don't know how to connect two sensors to the Raspberry pi simultaneously.
* We cannot obtain datum from the Humidity Sensor Module. 

<p align="center">
  <img src="/img/pr11/problem1.png" width="600">
</p>

<p align="center">
  <img src="/img/pr11/problem2.png" width="600">
</p>


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

<p align="center">
  <img src="/img/pr11/chart2.png" width="600">
</p>

* CZN15E:

