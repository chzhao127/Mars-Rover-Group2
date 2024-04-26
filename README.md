# Mars rover

## &bull; Introduction
The Mars Rover is designed to handle various tasks including environmental data collection and autonomous navigation. It incorporates advanced sensors and actuators to measure weather data and navigate through predefined waypoints autonomously.

<img width="324" alt="image" src="https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/f8381d5e-98be-4122-9a9c-842ce9726f7b">

## &bull; Hardware and Construction
The Rover's chassis is assembled from 3D-printed components,  motors are installed within these frames, supported by shock absorbers and wheels attached to motor wheel hubs. The assembly process includes the connection of various bolts and lines and the installation of sensors.

<img width="365" alt="image" src="https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/30321f6c-b857-41da-b170-96cc68af3ba9">

## &bull; Avionics and Electronics
The Mars Rover's electronic systems are built around a Raspberry Pi and Navio2 flight controller. Setup includes software configuration on the Pi, linking to a mission planner, and activating telemetry for data communication. Key elements are motor drivers, a power module, GPS antenna, and sensors for efficient operation control.

<img width="355" alt="image" src="https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/afea94db-e9a4-453c-b0be-554d24bb3636">

## &bull; Functional Capabilities
The Mars Rover employs Ardupilot for navigation, configured via a ground control interface. Data from missions are analyzed to evaluate sensor accuracy and environmental responses, offering insights into Rover performance and sensor reliability.

<img width="375" alt="image" src="https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/498e0616-8534-4779-a58c-c421a20c5f51">

## &bull; Sensors' measurement data and characterists evaluation

#### 1. BARO.Press

![126878e73747b07a9ab38bcfc4a311c](https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/5a2b892f-b0b5-4d45-9a1a-533396106209)

We can see from the picture, the min pressure is 100370.55 Pa, the max pressure is 100489.95 Pa, the mean value is 100410.07 Pa, and standard atmospheric pressure is about 101,325 pascals, which means the pressure measured is very close to the standard atmosphere at the Earth's surface.

#### 2. BARO.Temp

![6e6afa664c6193fe7c514631c07179a](https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/f431a6e3-72b1-4da4-8670-29f3e9caca81)

We can see from the picture, the min temperature is 35.54℃, the max temperature is 41.64℃, and the mean temperature is 39.81℃, this shows that the sensor exhibits good stability and consistency over this temperature range. The average temperature of the sensor is close to 40°C, which means that it is able to maintain a high operating temperature in the test environment. The difference between the peak and peak valley values indicates the sensitivity of the sensor to changes in ambient temperature, which is an important performance indicator for applications that need to operate under dynamic temperature conditions.

#### 3. BARO.Alt

![2c428c6cda200fe7612bba80659496e](https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/0c927346-5e9d-479e-bcc4-432b2a600ad3)

We can see from the picture, the min altitude is -2.77m, the max altitude is 7.95m, the mean altitude is 4.40m. Since we measured in the parking lot, the elevation fluctuation may reflect small fluctuations in the parking lot terrain or due to the location of the sensors. Negative altitude readings can result from inaccurate initial sensor calibration or from low-lying terrain relative to the starting point. These data indicate that the sensor is capable of detecting relatively small changes in height. The stability of the mean altitude shows the reliability of the sensor in a static environment.

4. IMU.T

![33b50c8835c5c6189f5ccfe79e8c34f](https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/d778dc0e-c5ed-409e-ba2b-d020f73345af)

We can see from the picture, 

We can see from the picture, the min
5. 

