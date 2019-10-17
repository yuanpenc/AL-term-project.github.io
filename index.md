# Smart Bathroom

**Course**: 12740

**Group ID** : AL

**Group Member**: Xinmiao Liu; Mengmeng Pan; Yuanpeng Cao; Peng Zeng

### [Progress report 1 （9.28）](https://github.com/yuanpenc/Yuanpeng.github.io/blob/master/progress%20report/progress%20report%201(9.28).md)
### [Progress report 2 （10.3）](https://github.com/yuanpenc/AL-term-project.github.io/blob/master/progress%20report/progress%20report%202(10.3).md)
### [Progress report 3 （10.6）](https://github.com/yuanpenc/AL-term-project.github.io/blob/master/progress%20report/progress%20report%203(10.6).md)
### [Progress report 4 （10.10）](https://github.com/yuanpenc/AL-term-project.github.io/blob/master/progress%20report/progress%20report4(10.10).md)
### [Progress report 5 （10.13）](https://github.com/yuanpenc/AL-term-project.github.io/blob/master/progress%20report/progress%20report5(10.13).md)


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

## Review of the Phenomena of Interest


### Physical Principles
The relative humidity (RH) of an air–water mixture is defined as the ratio of the partial pressure of water vapor in the mixture to the equilibrium vapor pressure of water over a flat surface of pure water at a given temperature. It is normally expressed as a percentage; a higher percentage means that the air–water mixture is more humid. At 100% relative humidity, the air is saturated and is at its dewpoint.
Sound is represented by audio signal, typically using a level of electrical voltage for analog signals, and a series of binary numbers for digital signals. Audio signals have frequencies in the audio frequency range of roughly 20 to 20,000 Hz, which corresponds to the lower and upper limits of human hearing.

### Statistic and Dynamic Behavior
Humidity is a dynamic characteristic since the water content in air is dynamic. In addition,  the unit of humidity we used is relative humidity. Relative humidity (RH) is the ratio of the partial pressure of water vapor to the equilibrium vapor pressure of water at a given temperature. Relative humidity depends on temperature and the pressure of the system of interest.
A sound signal is an example of a continuous signal that is sampled to result in a discrete signal. In this case, sound waves traveling through the air are recorded as a set of measurements that can then be used to reconstruct the original sound signal, as closely as possible. The sampling rate or sampling frequency is the number of samples taken per time unit. Sound signals are usually measured in Hertz (Hz).

### Signal Characteristic
Humidity signal: When the sensor is in the presence of water vapor it is absorbed, causing the functional ionic groups to disassociate, and resulting in increased conductivity. Response times are slow ranging from 10 to 30s. Most resistive sensors use an AC excitation to prevent sensor polarization. The resulting current is rectified and converted to DC where it can then undergo linearization and be amplified as necessary. The AC signal applied to the bridge ranges from 30 Hz to 10 kHz. As an example consider the TDK CHS series of integrated resistive humidity sensors with voltage output.

Sound signal: Sound signal is detected by sound intensity, which is defined as the power carried by sound waves per unit area in a direction perpendicular to that area. Sound intensity level is a logarithmic expression of sound intensity relative to a reference intensity.
The average sound intensity during time T is given by

<p align="center">
  <img src="/img/pr11/fomula1.png" width="200">
</p>
Also,
<p align="center">
  <img src="/img/pr11/fomula2.png" width="200">
</p>
Where,ν is frequency of sound,δ is the amplitude of the sound wave particle displacement,ρ is density of medium in which sound is traveling,c is speed of sound.

### Sensor(s) Used

#### DHT11
<p align="center">
  <img src="/img/pr11/sensor1.png" width="300">
</p>

#####	Physical Principles
It is a type of resistive humidity sensors that measure the resistance conductivity. The principle is the fact that the conductivity in non-metallic conductors is dependent on their water content. The resistive humidity sensor is made up of materials with relatively low resistivity and resistivity changes significantly with changes in humidity. The relationship between resistance and humidity is inverse exponential. The measurement range is 20-90%RH, temperature measurement range is 0-50℃.

##### Static and Dynamic Behavior 
This sensor includes a resistive-type humidity measurement component and an NTC temperature measurement component, and connects to a high- performance 8-bit microcontroller, offering excellent quality, fast response, anti-interference ability and cost-effectiveness. Applying the DHT11 sensor beyond its working range stated in this datasheet can result in 3%RH signal shift/discrepancy. The DHT11 sensor can recover to the calibrated status gradually when it gets back to the normal operating condition and works within its range. 

##### Sensor Characteristics
The ranges and accuracy of the DHT11: 
* Humidity Range: 20-90% RH
* Humidity Accuracy: ±5% RH
* Temperature Range: 0-50 °C
* Temperature Accuracy: ±2% °C
* Operating Voltage: 3V to 5.5V
<p align="center">
  <img src="/img/pr11/final chart1.png" width="500">
</p>

#### 1PCS 3pin Voice Sound Detection Sensor Module
<p align="center">
  <img src="/img/pr11/sound module sensor.png" width="300">
</p>

##### Physical Principles
It can detect the intensity of the sound environment. The sound sensor can identify the presence of (according to the principle of vibration). The sensor provides a digital output when the measured sound increases beyond a set threshold. This threshold level can be adjusted using an onboard potentiometer. The sensor outputs a logic one(+5V) at the digital output when it detects sound and a logic zero(0V), when there is no sound detected

##### Static and Dynamic Behavior 
This is a multipurpose sound sensor which can be used to sense sound and audio. An onboard LED is used to indicate the output status. The onboard potentiometer can be used to set the sound threshold. To set the potentiometer, use a screw driver.

##### Sensor Characteristics
<p align="center">
  <img src="/img/pr11/sound module char.png" width="500">
</p>

* It can detect the intensity of the sound environment. The sensor can only identify the presence of sound, cannot recognize the sound or the size of the particular frequency of sound
* The sensitivity adjustable digital potentiometer to adjust 
* Working voltage of 3.3 V to 5 V
* Output form digital switch output 

When less sensitive, it takes more sound to trigger the device and when more sensitive, it takes less sound to trigger the device. Three instructions Sound module sound intensity is the most sensitive to the environment, commonly used to detect the intensity of the sound of the surroundings. Module in the intensity of the sound environment than set threshold, the OUT output high level, when the intensity of the sound from the outside environment more than set threshold, the module OUT output low level. This sensor can be directly driven relay module, which can form a voice-activated switch.





## Experiments
Several tests were conducted to ensure the project was working as expected:
Focus on the ‘smart fans’ firstly. According to the comfortable range to human body is 30-60%, we set two certain levels---55% and 65%, that is, when the absolute humidity in bathroom rises to 55%, one ventilating fan begin to work; when the humidity rises to 65%, both two fans work. Use portable garment steamer to simulate the steam generated by bathing. As the steam spread to the whole bathroom (box), one of the fans began to work. As the steam continued to increase, the two fans began to work at the same time. Stop using the garment steamer, along with the fans, the humidity in the bathroom continued to drop, and when it reached 65%, one of the fans stopped working and the other continued to work until the humidity drops to a certain value.

Then, for the smart light part. Run the code and play the music, we can see that the light flicker with the music rhythm. We set different sleep time for the two lights in the code. Blue light has shorter sleep time to the sound signal than the red one. Therefore, two lights flicker with different frequency. Now, we can enjoy a fancy shower time! 

More details show in the video!

### Comparison to Original Goals
We basically achieved our original goal of creating a fan that can automatically switch on and off according to humidity, and a light that can flash according to music rhythm. Due to limited conditions, we can only test in the model. If we apply our idea to practice, we need to replace a bigger fan. At the same time, if there are more LED lights, the ‘smart light’ will look fancier.

### Errors

The error in the project comes from three sources. 

* Sensor:Our project uses sound detect sensor, and temperature and humidity sensor. For the temperature and humidity sensor, the error mainly comes from the nonlinearity of transfer function and the poor accuracy. 
* Noise:For the sound detection sensor, it is affected by the noise from both the circuit and the surrounding environment. When the sound sensor is very sensitive, the tiny sound will trigger the flicker of the light. For the temperature and humidity sensor, the situation is better.
* Control:As the test box is very small, when we use the steamer to simulate the shower mist, the air humidity in the box will increase to a high level instantly, making the two fans start to work almost at the same time. 

## Discussion







