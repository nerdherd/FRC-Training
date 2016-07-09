# Lesson 1

### Section 1: Github
You will need a GitHub account to complete this lesson.

###### What is Github?
Github is a collaborative version control system. What does this mean? Github allows you to store your code and keeps track of all revisions you make and share it with your team.

###### Github 101
The basic theory of Github is for the user to commit each change made to the code. That means that every change made is stored logically along with a commit message, a description of the change made. These commits are stored in a local repository, a copy of the repository located on your computer. After committing to your local repository, you need to push, or sync, to the remote repository, the copy stored on Github.

###### Using Github
Read [this lesson](../github/egit.md) and complete all the "Try This!"s. 

### Section 2: Downloading code to the RoboRIO
###### Get to know Driver Station
Read the Driver Station section of [this lesson](../frc/intro.md)

###### Prepare the code
1. Clone the [RoboRIO-Training](https://github.com/nerdherd/RoboRIO-Training)
2. Read through the comments of the code and understand what it does.

###### Connecting to the robot
1. Turn on the robot! The robot is not a robot if it is off.
2. Connect to the wifi network hosted on the robot (it will take about a minute to boot up)
3. Open FRC Driver Station and wait for the light to turn green. This is usually the part where programmers will bang our heads on the table so if you need help, come get one of us.

###### Upload the code
1. I hope you finished the `Prepare the code` step
2. Click the green arrow that looks like a play button. 
	a. This will open a pop up menu. Select `WPILib Java Deploy`
3. The program will now start to compile. You will know it is complete when it has a blue message saying "Build Successful: 687 seconds" (or it'll be more like 20 seconds).

###### Test the code
1. Yell CLEAR!!!!!
2. Wait for anyone around the robot to yell CLEAR!! back and move away from the robot.
> These two steps are extrememly important. If you skip these steps and the code malfunctions (or even in the slight offchance where it does function correctly) someone can get hurt.
3. Check one more time to make sure the robot is safe to run
4. Enable the robot.
5. Evaluate
	a. Did it work?
	b. If no, why? Now fix it.

### Section 3: Making modifications to code
###### Prepare the code
Using the existing code repository (from section 2)

1. Make the motor's speed correspond to the Y value of the joystick.
2. Output the value of Joystick Button 4 to the Smart Dashboard.

If you are having trouble with either of these, refer to the [WPILib Documentation](http://first.wpi.edu/FRC/roborio/release/docs/java/)

###### Upload and Test the code
You should know how to do this.