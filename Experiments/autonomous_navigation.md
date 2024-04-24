# Autonomous Navigation through Waypoint

## Overview
This document explores the Mars Rover's performance in autonomous navigation, detailing the setup, execution, and results of navigating a pre-defined path using waypoints.

## Navigation Setup
- **PID Settings**: Configured to optimize path accuracy and minimize deviations from the planned trajectory.
- **Throttle Adjustments**: Calibrated to maintain a balance between speed and control during navigation.

## Path Analysis
- The rover effectively followed the designed path with minimal deviations, demonstrating the effectiveness of the PID tuning in maintaining trajectory accuracy.
![image](https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/5d0fdaa9-aa14-4da3-877a-256ffa17fc46)
![image](https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/08fe60df-cfaf-47de-92dd-5b3bbc97f153)

## Performance Results
- **Total Time**: Completed the designed path in 14 minutes and 12 seconds.
  
  ![image](https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/7ac3234b-8c94-41fc-8dff-3c8ef57b4fba)
  15:35 – 1:23 = 14:12min
  ![image](https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/c32bdd8f-03d0-4089-bcb0-bc45d94a636c)

 - **Distance from Waypoints**: Based on the graph you can see the distance from each point to each way point correlates with that in the pathway.
    - Min: 0.00 m
    - Max: 32.94 m
    - Mean: 13.45 m
  ![image](https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/bf9ef120-da37-4935-848e-84133e5ee028)

## Error Metrics
- **Path Deviation**: There is a deviation in a range of apprioximately +/-2m which correlates with the WP radius of 2m.
    - Min: -2.34
    - Max: 2.32
    - Mean: 0.00
  ![image](https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/5e2cf7d2-6331-4eb5-9528-d5395ce8ee88)


## Suggested Improvements
- Focus on refining PID settings and throttle control to further reduce deviations and improve response times.
- Laying more waypoints help improve the accuracy of the path as the rover will know where to accurately make its next move.
- Inflated rubber tires may also help with rough/bumpy terains as they have better traction and flexibility.
