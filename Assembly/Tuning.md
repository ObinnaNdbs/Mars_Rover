# Rover Tuning Parameters Explanation

## Overview
This document details the individual parameters used for tuning the Rover's movement and navigation systems, explaining the role each one plays in the vehicle's performance. Correctly adjusting these values is essential for the Rover's optimal autonomous navigation performance.(all settings are based on connecting the laptop and teh rovers using the radio). Both radio settings must match! 
![image](https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/8b24dac1-ad6c-4b95-be76-78415a7c234f)

## Steering Rate Parameters
These parameters control the response of the Rover's steering system to achieve the desired turn rate.

- **P (Proportional Gain)**: Increases the steering response proportionally to the turn rate error. Higher values make steering more aggressive.
- **I (Integral Gain)**: Addresses the cumulative error over time. Useful for eliminating steady-state error, contributing to maintaining a consistent turn rate.
- **D (Derivative Gain)**: Dampens the steering response to prevent overshooting the desired turn rate. It reacts to the rate of change of the error.
- **IMAX**: Caps the contribution of the I gain to prevent integral windup.
- **FF (Feed-Forward Gain)**: Directly relates the desired turn rate to the steering output, bypassing the error-driven response for a more immediate reaction.
- **Turn Radius**: Specifies the default turning radius when in steering mode, impacting how tight the Rover turns.

## Speed/Throttle Parameters
These parameters are associated with the control of the Rover's speed and throttle outputs.

- **P (Proportional Gain)**: Adjusts the throttle in proportion to the difference between desired and actual speeds.
- **I (Integral Gain)**: Reduces the accumulated error in speed over time, ensuring that the target speed is maintained.
- **D (Derivative Gain)**: Reacts to rapid changes in speed error, helping to stabilize the speed control.
- **IMAX**: Limits the maximum effect of the integral component to prevent excessive build-up.
- **Accel Max (m/s)**: Sets the maximum forward acceleration the Rover will attempt, affecting how quickly it can speed up.
- **Brake**: Determines the braking behavior – if active, the Rover will apply reverse throttle to decelerate.
- **Cruise Speed (m/s)**: The default speed the Rover tries to maintain in auto modes.
- **Cruise Throttle**: The throttle level (as a percentage) that typically achieves the cruise speed.

## Throttle and Motors Parameters
- **Motor Type**: Defines the type of motor used, which can affect the response characteristics.
- **Throttle Min**: The minimum throttle output allowed, potentially used to maintain idle speed or compensate for motor stall.
- **Throttle Max**: The maximum throttle output the Rover will use.

## Navigation Parameters
These parameters influence how the Rover follows a path or reaches a waypoint.

- **WP Speed (m/s)**: The target speed when traveling from one waypoint to the next.
- **WP Radius (m)**: The radius within which the Rover considers it has reached a waypoint. A larger radius makes waypoint transitions smoother.
- **WP Overshoot (m)**: How far past a waypoint the Rover can travel before it's considered a miss and needs to correct.
- **Turn G Max**: The maximum lateral acceleration experienced during a turn, measured in multiples of gravitational acceleration (g).
- **Lat Acc Cntl Pe and Lat Acc Cntl Da**: Parameters for the lateral acceleration controller's P and D gains, affecting how aggressively the Rover corrects for lateral position errors when navigating a path.

## Additional Information
For guidance on how to adjust these parameters or for additional assistance, consult the full [Tuning Guide](https://ardupilot.org/rover/docs/rover-tuning-throttle-and-speed.html).
