Automatic Charging 
====================================================

Description of components and algorithms required for automatic charging

-------------------------------------------------------------------------------

Component
^^^^^^^^^^^^^^^^^^^^^^

.. thumbnail:: /_images/autocharge/part.png

- Consisting of robot and station
- A system that is charged by combining the charging terminal and the docking part of the station
- IR Camera : Used to detect IR patterns of stations
- Sonar Sensor : Adjust the balance so that it goes in a straight line when charging.
|

.. thumbnail:: /_images/autocharge/part2.png

|

---------------------------------------------------------------------------------------

Process
^^^^^^^^^^^^^^^^

.. raw:: html

    <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe src="https://youtube.com/embed/j11D6wvbykc?si=ctEwIxzU2JO6k73D" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe>
    </div>

|

1. Move to specified charging coordinates
2. Rotate to check station position
3. Move the robot so that the station is located in the exact center of the robot.
4. After confirming that it is located in the center, perform the docking process.
5. After the station's charging LED lights up, the color of the robot LED bar changes to match the robot battery status.

---------------------------------------------------------------------

Algorithm
^^^^^^^^^^^^

.. thumbnail:: /_images/autocharge/process.png

- frame : Default image
- blurred_frame : Removes noise and makes it smooth
- hsv_merge : Change color, saturation, and value(brightness)
- IR_camera : IR signal filtering
- gray_frame : Convert to eliminate noise, speed up computational processing, and improve accuracy
- binary_camera : Extract image features by converting pixel values ​​around each pixel to binary numbers

|

---------------------------------------------------------------

.. thumbnail:: /_images/autocharge/contours.png

- contours : Drawing the outline of an image

|

---------------------------------------------------------------

.. thumbnail:: /_images/autocharge/rectangle.png

- rectangle : Select only the outline of a rectangular shape

|

---------------------------------------------------------------

.. thumbnail:: /_images/autocharge/result.png

- result : Output the resulting image after all processes

|

---------------------------------------------------------------

.. thumbnail:: /_images/autocharge/maker.png
|

- The robot installation environment changes frequently.
- Automatic charging requires a singularity that can detect the station without being affected by the environment.
- Create 6 rectangular patterns to create a singularity.