# WPILib
### What is WPILib?
WPILib is a set of very useful libraries used to control the robot. Many of the classes contained are essential to moving the robot, including the motor controllers and the driver input.

### Movement
Movement is essential to any system. Without movement, the robot is just a fancy paperweight. There are two primary ways to move: Motors and Pneumatics.

###### Motors
Everyone knows what a motor is. It translates electricity to rotational movement. However, it's not that simple. Motors need a lot of power, more power than the roboRIO can output on its own. To combat this, we use motor controllers. Motor controller draw power directly from the PDP, so it can use up to 12V at 99A (please don't try this). It also takes input from the roboRIO, so it can translate PWM or CAN signals into power for the motors. To control the motor controllers, use either the `Victor`, `VictorSP`, `Talon`, or `CANTalon` class, based on which motor controller is actually used. However, all of these classes work quite similarly, using the same functions to set motor speeds.

```java
// Initialization
VictorSP myMotor;
myMotor = new VictorSP(0); // Pass in the port that the Victor is plugged in to

// Interaction
myMotor.set(1); // Full speed forward!
myMotor.set(-1); // Full speed reverse!
mymotor.set(0); // Stop the motor
```

###### Pneumatics
Pneumatics are a bit trickier. The pneumatic system is driven by highly compressed air (60psi = 4atm). The compressed air is sent into channels called Solenoids which direct the flow of air into either the front part of back part of a piston. To use this, two classes are needed.

```java
// Initialization
Compressor compress;
compress = new Compressor(); // Note that there are no arguments needed as there can only be one compressor.
compress.start(); // Make sure you start the compressor

DoubleSolenoid sol;
sol = new DoubleSolenoid(0,1); // Pass in the two ports the solenoid is hooked up to

// Interaction
sol.set(DoubleSolenoid.Value.kForward); // Push!
sol.set(DoubleSolenoid.Value.kReverse); // Retract!
sol.set(DoubleSolenoid.Value.kOff); // This shuts off air flow to the solenoid so that it can be moved manually.
```

### Driver Input
> Incomplete
