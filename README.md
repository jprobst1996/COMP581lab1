# COMP581lab1
The Objective
The primary purpose of this lab is to get some experience with Lego Mindstorms EV3 and the
LeJOS API. You will build your first mobile robot and familiarize yourselves with the motors and
sensors.

Task 1: Read our LeJOS Tutorial
If you have not already set up the Lego Mindstorms EV3 with your laptop, start by reading the
Tutorial on Setting up LeJOS with Java 8 for your Lego Mindstorms EV3:
Sakai → Resources → LeJOS Tutorial - Java 8.pdf
For more information, see:
https://sourceforge.net/p/lejos/wiki/Home/

Task 2: Odometry, Ranging, and Bumping
You should build a robot to accomplish the objectives below. Your robot must be built only using
pieces from your Lego Mindstorms kit. You should design your robot such that the center dark
gray button may be pressed without moving the robot and such that pushing the button does not
disrupt any of the sensors. Your robot should remain in one piece at all times, its diameter with
respect to the ground should not exceed 40 cm, and its diameter shall not change substantially
during the task. All measurements will be made with respect to the measuring point: a distinct
point of your choosing that is on the frontmost surface of your robot. Your robot should be
designed to accomplish the task autonomously without any human intervention (except for
pushing the center dark gray button as required).

All the objectives in this lab are to be completed in a single run, without picking up your robot.

Objective 1 (Odometry): Your robot will be placed behind a starting line on a flat surface (on
carpet in the Robotics Lab) and should wait to begin until you press the center dark gray button.
Upon pressing the button, your robot should move forward in a straight line for 1.2 meters and
stop. Immediately after stopping, the robot should beep. Here we will measure the distance from
the starting line and deviation from the center line (movement left and right) and points will be
awarded based on accuracy. To enable time for measurement, the robot should remain stopped
until the button is pushed.

Objective 2 (Ranging): After completing the first objective, you will press the center dark gray
button and your robot should resume moving forward. Somewhere directly in front of your robot
will be a flat surface (like a wall or large object) that you can assume is at least 17 cm high and
can be detected by the ultrasonic sensor. The robot should stop such that it is 50 cm from the
flat surface (measured from the nearest point on the robot). Your robot should beep and pause
until the center dark gray button is pressed.

Objective 3 (Bumping): After the previous two objectives, you will push the center dark gray
button and your robot should now move forward and approach the surface. It should bump the
surface with a bump sensor placed on the front of the robot. After bumping into the surface, the
robot should move in reverse until it is 50 cm from the wall again.
A visual representation of the workspace looking down from the ceiling:
Points

To complete this lab you will use a subset of the leJOS API:
http://www.lejos.org/ev3/docs/

Important: You may only use classes from the following packages in Java and the leJOS API:
any class in the java.io, java.lang, java.util, lejos.hardware, and lejos.hardware.* packages. Note
that the classes must be implemented in one of these packages; a class that simply inherits
from one of these packages is not permissible. For example, you cannot use a class in
lejos.robotics.

A robot relying on a Java class from a package not listed above will be disqualified.
In the comments at the top of the Java source file containing your main method, please include
the names and PID’s of all team members.
