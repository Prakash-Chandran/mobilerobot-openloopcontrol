# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

## Step1:
<br/>
Use from robomaster import robot

## Step2:
<br/>
Choose the x,y,z - axis movement distance(meters).

## Step3:
<br/>
Give ep_chassis.move to move straight.

## Step4:
<br/>
Give time.sleep() for a break.

## Step5:
<br/>
Give ep_chassis.drive_speed to have a circular movement.


## Program
```python
from robomaster import robot
import time
from robomaster import camera

if _name_ == '_main_':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis
    ep_led = ep_robot.led
    ep_camera = ep_robot.camera

    print("Video streaming started.....")
    ep_camera.start_video_stream(display=True, resolution = camera.STREAM_360P)

    ep_chassis.move(x=2.5, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=255,b=0,effect="on")

    ep_chassis.move(x=0.5, y=0, z=75, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=255,effect="on")
    

    ep_chassis.move(x=0.9, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=255,b=255,effect="on")

    ep_chassis.move(x=0, y=0, z=70, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")

    ep_chassis.move(x=0.4, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=0,effect="on")

    ep_chassis.move(x=0, y=0, z=20, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")

    ep_chassis.move(x=1.6, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=255,effect="on")


    ep_chassis.move(x=0, y=0, z=-30, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=255,b=255,effect="on")

    ep_chassis.move(x=1.1, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=128,g=0,b=0,effect="on")

    ep_chassis.move(x=0, y=0, z=45, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=128,b=0,effect="on")

    ep_chassis.move(x=1.5, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=128,effect="on")

    ep_chassis.move(x=0, y=0, z=95, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=153,g=153,b=255,effect="on")

    ep_chassis.move(x=2.1, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=255,b=204,effect="on")

    ep_chassis.move(x=0, y=0, z=83, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=102,g=0,b=102,effect="on")

    ep_chassis.move(x=0.7, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=102,b=204,effect="on")


    ep_chassis.move(x=0, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=204,g=204,b=255,effect="on")
    time.sleep(4)
    ep_camera.stop_video_stream()
    print("Stopped video streaming.....")

    ep_robot.close()
```

## MobileRobot Movement Image:

![robo](./img/robomaster.png)

# Captured Images:

![Screenshot 2024-05-15 114027](https://github.com/Prakash-Chandran/mobilerobot-openloopcontrol/assets/147120899/2c25bc13-3201-45a4-95c4-b5d2ee5b8ca6)

![Screenshot 2024-05-15 114046](https://github.com/Prakash-Chandran/mobilerobot-openloopcontrol/assets/147120899/be3769e6-05bc-4f7e-9efa-89404869b411)

![Screenshot 2024-05-15 114100](https://github.com/Prakash-Chandran/mobilerobot-openloopcontrol/assets/147120899/707b55c7-0228-4f14-bcbd-a24b4aadfba3)

![Screenshot 2024-05-15 114117](https://github.com/Prakash-Chandran/mobilerobot-openloopcontrol/assets/147120899/617db5e7-2f47-4c37-8563-d7d8dfc3c84e)

<br/>
<br/>
<br/>
<br/>

## MobileRobot Movement Video:

Upload your video in Youtube and paste your video-id here

[![<iframe width="560" height="315" src="https://www.youtube.com/embed/SwRday7fcR0?si=1dEI_vaTHIl6oeTm" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>)]]

<br/>
<br/>
<br/>
<br/>

## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.


<br/>
<br/>

```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```
