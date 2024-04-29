Other Mission Examples
=========

Get coordinate information, Send to desired coordinate
--------------------------------

Before the mission, we will explain how to get the coordinates and how to move to the specified coordinates.

Get Coordinate Information
 - Run the goal_position example on Jupyter Hub.
 - Take a target point using the Start Nav Goal function in the Web GUI.
 - Looking at the picture below, the x, y coordinates are output.

  .. thumbnail:: /_images/course_1/4.slam_navigation/goalpose.png

|
  
Send robot to desired coordinates
 - Open navi example on Jupyter hub
 - Enter the x, y coordinate information of the destination
  .. thumbnail:: /_images/course_1/4.slam_navigation/1point.png

|

 - You can pass through several destinations.
  .. thumbnail:: /_images/course_1/4.slam_navigation/manypoints.png

|
  
Map Examples
----------------------------------------------

.. raw:: html

    <div style="background: #ffe5b4" class="admonition note custom">
        <p style="background: #ffbf00" class="admonition-title">
            Mission via target point
        </p>
        <ul>
            <li><strong></strong> Below are three maps.</li>
            <li><strong></strong> On each map, each waypoint is marked.</li>
            <li><strong></strong> Create a map with structures. After that, the robot is used to draw the map.</li>
            <li><strong></strong> The goal is to start at the start point and return to the start point by passing through the destination in order.</li>
            <li><strong></strong> You can choose from the examples below, or you can create and use your own maps.</li>
            <div>
        </ul>
    </div>
    
**D - MAP**

.. thumbnail:: /_images/course_1/4.slam_navigation/DMAP.png

-----------------------------------------------------------------

**T - MAP**

.. thumbnail:: /_images/course_1/4.slam_navigation/TMAP.png

------------------------------------------------------------------

**WINDMILL - MAP**

.. thumbnail:: /_images/course_1/4.slam_navigation/WINDMILLMAP.png


