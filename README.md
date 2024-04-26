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

#### 4. IMU.T

![33b50c8835c5c6189f5ccfe79e8c34f](https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/d778dc0e-c5ed-409e-ba2b-d020f73345af)

We can see from the picture, the min temperature is 36.35℃, the max is 42.63℃, and the mean value is 40.86℃. This indicates that the internal temperature of the IMU changes relatively little during the period of data recording, showing good thermal stability. This temperature range may also indicate its own heating and heat dissipation efficiency, which is an important performance indicator for equipment deployed in a closed environment for a long time. The thermal performance of the sensor is shown to be suitable for use in stable and predictable environments, which is critical to ensure measurement consistency and equipment reliability during long-term operation

#### 5. GPS.Alt

![e57ca8daef252ff5bc45da1d7ed70d4](https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/013d52a9-22a1-4532-b4d2-77541174290c)

We can see from the picture, the min altitude is 163.57m, the max altitude is 186.59m, the mean altitude is 171.84m. The data within this range of altitude variation indicates that GPS has good accuracy and consistency in monitoring specific altitude. Considering that GPS systems are commonly used for positioning and navigation, this small elevation variation indicates that the system can provide stable and reliable altitude information under static conditions.

<img width="209" alt="image" src="https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/6205f148-a6cb-4bba-a208-f40d277444e2">

And then I compared the values with the altitude we record when we make the test, I find the record value 168.66m is very close to GPS.Alt and in the interval.

#### 6. NTUN.XTrack

![7dae076c00f70afaabdc1df5c9f370f](https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/f2865542-50ef-4c99-9a64-8c18b75d4161)

We can see from the picture, the min is -2.41, the max altitude is 1.20, the mean altitude is -0.41. These data indicate that the navigation system shows a certain deviation in maintaining a predetermined path. The difference between the minimum and maximum values shows a range of fluctuations in the degree of offset, while the mean deviation is close to zero but slightly negative, indicating that the system tends to shift slightly to the left of the path during the test. I think this offset may be due to inaccurate system calibration, environmental factors, or sensor errors.

#### 7. NTUN.WpDist

![236fcf26aedb74ea7f3b7c1822ffee7](https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/4ffadd66-9532-47b8-abb9-4092af77e603)

We can see from the picture, the minimum distance is 0.00, the maximum distance is 31.36, and the average distance is 11.61, which indicates that the waypoints are set at different distances, or the vehicle speeds are different between waypoints
This zigzag pattern is characteristic of autonomous or semi-autonomous navigation, in which a vehicle moves toward a waypoint, reaches that waypoint, and then continues on to the next waypoint. A sharp increase indicates a momentary reset, possibly the moment when the next waypoint becomes the target. The average distance shows that, on average, waypoints are moderately spaced.

#### 8. RAD.RxErrors
   
![95efa6d16932ab077893076808a441b](https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/30b5c6b4-3891-42a7-8bb9-1dc5e713f4aa)

The data from the RAD.RxErrors graph initially shows a substantial spike in receiver errors, reaching a peak of 25, before dropping to a consistent zero, which indicates an abrupt resolution to reception issues. The mean error rate of 23.21 suggests that the majority of the time captured by the plot was error-free, implying an overall reliable communication after the initial spike.

#### 9. IMU.Accz

![d57094fb7e2a289bfdd55af177bcc5b](https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/202215b0-4d91-4375-b849-67eb99821e84)

The IMU.AccZ graph demonstrates noticeable volatility in the acceleration along the Z-axis, with a mean value of -9.71. The persistent negative acceleration indicates a dominant downward force, likely due to gravity, and the spikes suggest that the vehicle or device is subject to intermittent forces or jolts, which could be indicative of rough terrain or impacts.

#### 10. IMU.Accz, NKF1.PD, NKF1.VD

![b5f2ebab0a936e8541c620960f2c9cc](https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/aadfe19a-dadc-4c0c-93e9-227f2c28ca9a)

In the combined plot of IMU.AccZ, NKF1.PD (Positional Deviation), and NKF1.VD (Velocity Deviation), we see a correlation between the acceleration data and these navigational metrics. NKF1.PD exhibits significant variation, with a mean indicating a tendency toward a negative positional deviation, whereas NKF1.VD is relatively stable, fluctuating slightly around a near-zero mean. This could signify that while there is some positional drift, the velocity remains fairly consistent, which might be expected in a system that compensates for positional errors to maintain a steady course.

## &bull; Path Design

#### Here is the eight waypoints we set: 

<img width="636" alt="3f225d9b7ea08bc627554e5d551a144" src="https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/328cfab6-e4ab-4afe-b8df-675f9b08fcb3">

The distance from waypoint 1 to waypoint 2 is around 30 meters.
The distance from waypoint 2 to waypoint 3 is around 10 meters.
The distance from waypoint 3 to waypoint 4 is around 20 meters.
The distance from waypoint 4 to waypoint 5 is around 10 meters.
The distance from waypoint 5 to waypoint 6 is around 20 meters.
The distance from waypoint 6 to waypoint 7 is around 10 meters.
The distance from waypoint 7 to waypoint 8 is around 30 meters.
The distance from waypoint 8 to waypoint 1 is around 30 meters.

&#x25CF; Firstly, we make sure the distance between each dot in Mission Planner by right-click the dot and choose Map Tool, then choose Measure Distance to test the distance between two dots. It can be shown in the picture below:

<img width="785" alt="image" src="https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/4e740251-b919-47d9-8adf-8551ac562a13">

We can see the distance between two dots like:

![a6a56782dc34da5057a9c31c6395259](https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/2307112a-f068-4d4a-8164-ea558ca216c6)


&#x25CF; Secondly, We make sure the distance between each dot by using the measure app in the iphone to test. It can be seen in the picture below:
![5ce66fc7143b4bf10b031dfe72af338](https://github.com/chzhao127/Mars-Rover-Group2/assets/161892823/b091bb15-9d65-4663-9887-992e454c170b)


## &bull; PID tuning
1
2
3
