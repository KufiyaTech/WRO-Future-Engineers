
***
## <p align="center"> Hey we are team Astra we are 3, Rym, Adam, and Youssef, 15-year-old coders, and this is our repository. It comprises all the engineering materials for our autonomus vehicle model participating in the 2024 WRO Future Engineers competition. </p>


<div align=center>

  
***

## This is our team :
![WhatsApp Image 2024-05-18 at 17 59 31](https://github.com/youssefelbaitar/WRO-Future-Engineers/assets/168293228/a29da0b3-5f08-4e1f-a1ec-4250f79eeb3c)


<div align=center>

  
![WhatsApp Image 2024-05-18 at 17 59 33](https://github.com/youssefelbaitar/WRO-Future-Engineers/assets/168293228/eb98efcf-f1fc-4408-a98d-319810468f3d)



<div align=center>


![Astra_robotics__2_-removebg-preview](https://github.com/youssefelbaitar/WRO-Future-Engineers/assets/168293228/a604f669-20ef-4af0-9544-f86272edc464)


<p align="center">!
</p>
</div>

***
## The microcontroller:
<body>
  <div align=center>
    <h1>LEGO Mindstorms EV3 Brick</h1>
</div>
</body>

<table>
  <thead>
    <tr>
      <th>Feature</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Processor</td>
      <td>ARM9 processor running at 300 MHz</td>
    </tr>
    <tr>
      <td>Memory</td>
      <td>64 MB RAM, 16 MB flash storage</td>
    </tr>
    <tr>
      <td>Ports</td>
      <td>Four motor ports, four sensor ports</td>
    </tr>
    <tr>
      <td>Connectivity</td>
      <td>USB port, SD card slot, Bluetooth</td>
    </tr>
    <tr>
      <td>Display</td>
      <td>Monochrome LCD display</td>
    </tr>
    <tr>
      <td>Controls</td>
      <td>Buttons for navigation and control</td>
    </tr>
    <tr>
      <td>Software</td>
      <td>LEGO Mindstorms EV3 software, supports languages like Python and C++</td>
    </tr>
    <tr>
      <td>Use Cases</td>
      <td>Robotics education, hobbyist projects, competitions</td>
    </tr>
    <tr>
      <td>Community</td>
      <td>Large online community, resources, tutorials</td>
    </tr>
  </tbody>
</table>

***
<p align="center">
  <img width="320" height="300" src="https://m.media-amazon.com/images/I/31uzGocdrPL._AC_UF894,1000_QL80_.jpg">
</p>


  


***
## Our vehicle: 

We used the EV3 MINDSTORMS Educational kit. We chose to use a racing car shape so it could move fluidly and dodge the obstacles

A 3D model of our first robot version in Studio 2.0 :

![finalfirstproduct](https://github.com/youssefelbaitar/WRO-Future-Engineers/assets/164657596/dbaef324-04d2-4831-9cfe-4c9155e96a13)

This was our first version but the issue it that it wasn't really stable
![f2584cbe-6115-41a7-b710-c312dd14e4d2-removebg-preview](https://github.com/youssefelbaitar/WRO-Future-Engineers/assets/164657596/20b291f2-d3e5-4f2c-8db0-7427d46e603a)

And this is our last version way more efficient and stable


###The Open Challenge code for our autonomous vehicle : 

Script Breakdown
Imports and Initialization:

The script imports necessary classes and functions from the pybricks library.
Initializes two motors, several sensors (ultrasonic and gyro), and sets the gyro sensor angle to zero.
Initializes the EV3 brick for feedback and control.

![image](https://github.com/youssefelbaitar/WRO-Future-Engineers/assets/164654010/ec371415-06b1-43b8-ae90-3c962796c29b)

Motor and Sensor Setup:

Two motors are configured: a large motor on port D and a smaller motor on port B.
Ultrasonic sensors are attached to three ports: front (S1), right (S3), and left (S4).
A gyro sensor is attached to port S2.

![image](https://github.com/youssefelbaitar/WRO-Future-Engineers/assets/164654010/6d5a596c-a874-4f37-9595-b2552c53f574)

Function Definitions:

Functions Turn_Right and Turn_Left are defined to control the small motor for turning the robot.

![image](https://github.com/youssefelbaitar/WRO-Future-Engineers/assets/164654010/3bcdfbcc-2d30-46fe-a6ed-33d2b1b17100)

Main Loop:

The main loop continuously runs, making decisions based on sensor readings.
The robot moves forward if there is no obstacle within 165 mm in front.
If the ultrasonic sensors detect obstacles on the right or left, it triggers the respective turning function.
If the gyro sensor detects that the robot has turned more than 90 degrees in either direction, it adjusts the turn and resets the gyro angle.
When an obstacle is detected within 165 mm in front, it reverses and turns in the direction with more space.

![image](https://github.com/youssefelbaitar/WRO-Future-Engineers/assets/164654010/dd157978-20c1-46f9-bdc8-0da0267b12bb)





***
## Mobility Management

### Motor Selection and role
Choosing the motors is an important step to build the vehicle. We used only 1 big motor for the main movemement so the robot can be smaller and a mid motor for the steering mechanism so it allows the robot to turn easily while moving forward.

<body>
    <table>
        <tr>
            <th>Aspect</th>
            <th>EV3 Big Motor</th>
            <th>EV3 Mid Motor</th>
        </tr>
        <tr>
            <td>Size</td>
            <td>Large</td>
            <td>Medium</td>
        </tr>
        <tr>
            <td>Power</td>
            <td>High torque</td>
            <td>Medium torque</td>
        </tr>
        <tr>
            <td>Speed</td>
            <td>Lower</td>
            <td>Higher</td>
        </tr>
        <tr>
            <td>Applications</td>
            <td>Best suited for heavy-duty tasks like driving large wheels or lifting heavy objects.</td>
            <td>Well-suited for medium-duty tasks like controlling arms, gears, or small wheels.</td>
        </tr>
        <tr>
            <td>Weight</td>
            <td>Heavier</td>
            <td>Lighter</td>
        </tr>
    </table>

  
### Chassis 

We tried to copy f1 vehicles shape.The steering mechanism is located in the front, utilizes smaller wheels. Additionally, positioning the larger wheels as close to each other as possible, for more stability and agility.
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

</head>
<body>
    <h3>Advantages of Different F1 Car Shapes</h3>
    <table>
        <tr>
            <th>Shape</th>
            <th>Advantages</th>
        </tr>
        <tr>
            <td>Aerodynamic</td>
            <td>
                <ul>
                    <li>Improved airflow over and around the car, reducing drag and increasing straight-line speed.</li>
                    <li>Enhanced downforce generated, improving grip and cornering stability.</li>
                    <li>Efficient cooling of engine and components due to optimized airflow.</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>Compact</td>
            <td>
                <ul>
                    <li>Reduced frontal area, minimizing air resistance and drag.</li>
                    <li>Improved agility and responsiveness in tight corners and chicanes.</li>
                    <li>Lower weight distribution, enhancing acceleration and braking performance.</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>Streamlined</td>
            <td>
                <ul>
                    <li>Smooth airflow around the car, reducing turbulence and drag.</li>
                    <li>Improved fuel efficiency and reduced fuel consumption.</li>
                    <li>Enhanced stability at high speeds, minimizing aerodynamic disturbances.</li>
                </ul>
            </td>
        </tr>
    </table>
</body>

<p align="center">

  ![Diseño sin título](https://github.com/youssefelbaitar/WRO-Future-Engineers/assets/164657596/3ec9081c-b8d5-4fd0-8456-c5bd9a1cc773)




</p>

***
<h1> Sensors </h1>

Our vehicle is simple,with only two color sensor crucial for obstacle avoidance and turns.


  
### Vehicle Sensors Overview Version 1

<body>
    <table>
        <tr>
            <th>Sensor</th>
            <th>Purpose</th>
            <th>Functionality</th>
        </tr>
        <tr>
            <td>Color Sensor 1</td>
            <td>Turn Identification</td>
            <td>Reads colored lines (orange or blue) on the competition field to determine driving direction.</td>
        </tr>
        <tr>
            <td>Color Sensor 2</td>
            <td>Obstacle Detection</td>
            <td>Identifies obstacles by detecting red or green colors.</td>
        </tr>
    </table>
  </body>
<p align="center">
  
![1](https://github.com/youssefelbaitar/WRO-Future-Engineers/assets/164657596/a5cf38b7-1196-4f77-b6f1-67d52d299269)

</p>

### Vehicle Sensors Overview Version 2
<body>
    <table>
        <tr>
            <th>Sensor</th>
            <th>Purpose</th>
            <th>Functionality</th>
        </tr>
        <tr>
            <td>UltraSensor 1</td>
            <td>Obstacle detection</td>
            <td>Reads colored lines (orange or blue) on the competition field to determine driving direction.</td>
        </tr>
        <tr>
            <td>UltraSensor 2/3 </td>
            <td>Walls Detection</td>
            <td>the robot keeps going straight when there are walss from both side but when he detects a big distance it means there is no inner wall so he will turn</td>
        </tr>
              <tr>
            <td>4 Gyro </td>
            <td>Turn detection</td>
            <td> It helps the robot to turn in stable way </td>
        </tr>
    </table>
  </body>

![1](https://github.com/youssefelbaitar/WRO-Future-Engineers/assets/164657596/87ed17b8-d04a-4fbf-a233-6cbe88795520)




