Source: [Difference between DC, Servo and Stepper Motors](https://thepihut.com/blogs/raspberry-pi-roundup/whats-the-difference-between-dc-servo-amp-stepper-motors)
## DC Motors
- DC Motors are two wire (power and ground) **continuous rotation motors**. They spin at high RPM
- When power is supplied, the DC motor will start spinning until power is removed.
- **Speed can be controlled using PWM**. The percentage duty cycle will determine the speed of the motor. If the duty cycle is 50%, the motor will spin at half the speed at 100%.
- They are used in computer cooling fans and RC car wheels.
- Suitable for anything that spins at high RPM
## Servo Motors
- They are usually 3-wire (power, ground and control). Power is constantly applied. 
- Usually constructed using an assembly of a DC motor, gearing set, control circuit and position-sensor(usually potentiometer).
- The position of the motor can be controlled precisely, and do not rotate freely like standard DC motors. **Angle of rotation is limited to about 180 degrees** back and forth from the centre position. The control circuit applies power to the DC motor inside until the shaft turns to the correct position, determined by the position sensor. 
- Note: Servo motors usually have a position error due to dead band caused by friction in the motor.
- Similar to DC motors, the motor can be controlled using PWM. However, instead of controlling the speed, the **PWM control signal determines the position**.
	- The PWM control signal tells the servo where to go, which includes staying the same position. **Depending on the servo motor, the PWM frequency should be chosen**
	- A neutral pulse depending on the servo will keep the servo in the centre position. Increasing/decreasing the pulse width will make the servo turn clockwise/anticlockwise
- High performance alternative to stepper motors. Suitable to robotic arms/legs, boat rudder control etc. But position is less accurate than stepper motors.
## Stepper Motor
- Similar to servo motor in which the position is controlled, but stepper motors uses multiple toothed electromagnets arranged around a central gear to define position.
- Requires an external control circuit to individually energise each electromagnet to turn the motor shaft.
- Stepper motor controls position via rotation by fractional increments.
- Slow, precise, easy setup and control. More accurate than servo motors. Suitable for 3D printers etc.