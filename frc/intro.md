# Introduction to Robot Programming

### What is Robot Programming?
Robot programming is an interface for the drivers to control the robot. Although invisible and intangible, software is one of the most important parts of the robot. As I like to say, "Good software can make a bad robot win but bad software will make a good robot loose".

### Game Structure
Most FRC games are structured into two different periods: a 15 second autonomous period and a 2 minute and 15 second teleoperated period. During the autonomous period, robots act on their own as the drivers must stay clear of the driver station. During the teleoperated period, the drivers step forward and take the controls to direct their robots to victory.

### Code Structure
When it comes to programming robots, Team 687 extends the Java IterativeRobot class. This allows us to use seven built-in functions that initialize and loop through the periods of the game.

Each period of the game, autonomous, teleop, and test (we'll get into this later), has two functions associated with it: `init` and `periodic`. The `init` function is called once as soon as the mode starts. This is where all objects should be constructed and subsystems initialized. The `periodic` function gets called regularly at approximately 40 hertz while the robot is enabled. In addition to these, there is one last function, `robotInit()`. This function gets called as soon as the robot turns on and is first enabled.

### WPILIB
Worchester Polytechnic Institute (WPI) is one of the main sponsors of FRC, and is the college where Dean Kamen, the founder of FIRST, attended before dropping out, inventing the segway, making billions of dollars (go Dean!). WPI has also created WPILIB, a library meant to help control the robot.

WPILIB can be broken down into the following categories:
- Motors
  - Victor
  - Talon
  - CANTalon
- Pneumatics
  - Compressor
  - Solenoid
  - DoubleSolenoid
- Sensors
  - Encoder
  - Gyro
  - Ultrasonic
  - PowerDistributionPanel
- IO
  - DigitalInput
  - DigitalOutput
  - AnalogInput
  - AnalogOutput
  - I2C
  - SPI
- Interface
  - Joystick
  - SmartDashboard

  > Note: There are many more classes to WPILIB, these are just a few commonly used ones.

### Driver Station
> incomplete

### Automation
> incomplete
