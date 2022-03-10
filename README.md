# UR-Scripting by example (by Helge)

A short GitHub to give en example how to write and use UR-script in the UR-Polyscope enviorment.

## Test platform
All code have been tested on version polyscope version:

CB3: 3.15.4

E-series: 5.11

Robot platform : UR3 and UR3e

You can either test it on the Offline simulator (download that from UR Homepage or [here (updated last 02022022)](https://ucndk-my.sharepoint.com/:f:/g/personal/hgr_ucn_dk/Ei5tqgtmOvFCqEWAVZdYMiABk1DubYUFo2dtYdXqdPlfDw?e=bKitJm)
## Code and examples
Under the folder [UR Script](UR_Script) you will finde the script files used in the following examples.
Under the folder [UR Code](UR_Code) you will finde a file with all files to load into polyscope.
Under the folder [Manual](Manual) you will find UR-script manual in pdf format.

## How to run use functions in polyscope
Step 1:
Press "robot program" and mark the field "add Before Start Sequence", this will make first run the will not be looped. In this tab of the programming you can set up a start position, functions and other values that you want global access to.
![GettingStarted](Pic/GettingStarted0.png)
To add a function, go to the "advanced" tab in programming, choose "Script", change the dropdown menu to "file" and press "edit". From here you can now load a file writen in UR-script ("filename".txt or .script) and you can edit the file directly in the polyscope editor (remember to press save)
![GettingStarted](Pic/GettingStarted1.png)
When the function are loaded into the "BeforeStart" you can call it in the "Robot program" (see picture with red)

## Example 1: Function for Control Outputs from a local script file.
Hallo world in the HW world, is to control an LED, try to implement this code
```:https://github.com/glinvad/UR_Scripting/blob/main/UR_Script/1_Ex_Led_blik.script

```
![Example 1](Pic/ex1.png)

## Example 2: Function with parameter transfer
Using parameteres to control a function can be importent, in this example it is used to make a "Pause" function"
```:UR_Script\2_Ex_CountDown_Pause.script

```
![Example 2](Pic/ex2.png)

## Example 3: Function with parameter transfer and make calculation and return result.
Usnge parameteres and math with return functions
```:UR_Script\3_Ex_Math.script

```

![Example 3](Pic/ex3.png)

## Example 4: Function with move command and calculate new position for move.
Using the UR script control the robots movement, in the picture it can be seen that the robot is moved with a movej to a start position. This way of moving a UR robot eliminates the start function of robots, where a user actively needs to press on the teach pendant to move the robot into a position. At the same time, there are no safety net to help the programmer from putting the robot into an illigal position, except an error message.
```:UR_Script\4_Ex_Move.script

```

![Example 4](Pic/ex4.png)

## Example 5: Function with If condition.
Using a IF condition to move the robot.

```:UR_Script\5_Ex_if.script

``` 
![Example 5](Pic/ex5.png)

## Example 6: Function with 2 lists of poses (Each list contain 6 poses i.e. a total of 12 poses).
Using a function to run though multiple lists of postions, the position are saved in sub-programs and are loaded into the main robot program (see the picture or the example file)
```:UR_Script\6_ex_Going_Though_a_list_of_poses.script

``` 
![Example 6](Pic/ex6.png)

## REMEMBER
Have fun !! :) 

## Links

[Universal Robots download page](https://www.universal-robots.com/download)
 
[Zacobria Automation](https://www.zacobria.com/automation/) 
