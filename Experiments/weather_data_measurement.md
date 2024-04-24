# Weather Data Measurement

## Overview
This document summarizes the results and methodologies used for measuring weather-related data using the Mars Rover's onboard sensors, primarily focusing on temperature, atmospheric pressure, and altitude calculations.

## Sensor Data Summary
- **Temperature, Pressure and Altitude Measurement**: Utilized the BARO sensor to measure atmospheric pressure and IMU sensor to measure the ambient temperature.

## Results
### Temperature Measurements
- **BARO Sensor Temperature**: The readings are that of the barometer device itself which do not provide 
  - Min: 30.05°C
  - Max: 37.21°C
  - Mean: 33.09°C
  ![image](https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/cfc9faf2-bcab-4a5e-80c1-8989914f69d6)

- **IMU Sensor Temperature**:
  - Min: 31.10°C
  - Max: 36.98°C
  - Mean: 33.59°C
  ![image](https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/ec7ddb60-afc1-40a2-ac0a-4d6574109178)

- **Actual Atmospheric Temperature (from Google Maps)**:
  - Recorded High around: 15.56°C
![image](https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/4e5766b7-b361-43c3-a27b-d144c2e5ab97)

**Analysis**:
- The IMU sensor readings are significantly higher than the actual temperatures recorded during the experiment. This variance suggests potential influences from internal rover components or improper sensor placement.

### Pressure Measurements
- **BARO Sensor Pressure**: The pressure sensor is not functioning properly leading to accassional jumps in the graph and wrong pressure data.
  - Min: 97942.80 Pa
  - Max: 100631.42 Pa
  - Mean: 100460.67 Pa
  ![image](https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/b7d8e44c-0773-4826-ab62-231cc82aa2da)

### Altitude Measurements
- **BARO Sensor Derived Altitude**: The pressure sensor is not functioning properly leading to accassional jumps in the graph and wrong altitude data.
  - Min: -4.77 m
  - Max: 237.64 m
  - Mean: 10.56 m
![image](https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/3f16b27e-9aca-4e50-9aec-3adcf51b4c7c)

- **GPS Altitude**:
  - Min: 167.39 m
  - Max: 182.12 m
  - Mean: 172.82 m
  ![image](https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/28d55b38-c1ea-4fc5-ac43-05a4b4bbad25)

- **Actual Altitude (from Google Maps)**:
  - Min: 166 m
  - Max: 168 m
  - Mean: 167 m
  ![image](https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/c3d950ee-90ed-407a-8a8c-567d82777632)
  
**Analysis**:
- The GPS readings show a reasonable correlation with the actual altitude data from Google Maps, with a slight variation that could be attributed to GPS accuracy limitations under certain environmental conditions.

## Suggested Improvements
### For Temperature Measurement
1. **Sensor Shielding and Placement**:
   - Implement shielding for the IMU sensor to reduce heat transfer from the rover's internal components.
   - Reevaluate the sensor placement to avoid areas prone to heating or direct sunlight exposure.


### For Altitude Measurement
1.  **Environmental Considerations**:
    - Record environmental conditions that may affect GPS signals, such as atmospheric pressure or heavy cloud cover, and adjust data collection methods accordingly.
2. **GPS Enhancement**:
    - Regularly update GPS firmware and check settings to ensure optimal performance.
    
