# Initial Programming Instructions

## Overview
This document describes the initial programming steps necessary for getting the Mars Rover operational. This involves loading the firmware onto the Raspberry Pi and setting up basic operational parameters.

## Steps

### 1. Install ArduPilot Firmware:
- **Access the Raspberry Pi via SSH**: Connect to your Raspberry Pi using SSH.
- **Install ArduPilot**:
  - Fetch the latest version of ArduPilot compatible with Navio2 by running:
    ```bash
    wget https://firmware.ardupilot.org/Rover/stable/navio2/ardurover.apj
    ```
  - Use the Emlid Tool to install the firmware:
    ```bash
    emlidtool ardupilot
    ```
  
### 2. Configure ArduPilot:
- **Modify Configuration Files**:
  - Edit the `ardupilot.env` file to set vehicle-specific parameters:
    ```bash
    nano /etc/default/ardupilot
    ```
  - Add or modify lines to set parameters like `TELEM1`, `GPS_TYPE`, and others as needed.

### 3. Test Basic Functions:
- **Start ArduPilot**:
  - Manually start the ArduPilot software to test its operation:
    ```bash
    sudo systemctl start ardupilot
    ```
- **Check for Basic Response**:
  - Connect Mission Planner or another ground control software to ensure the Rover is responding correctly.

### 4. Mission Planner Setup:
- **Connect to Mission Planner**: Ensure that your Rover is connected to the same network as your PC running Mission Planner.
- **Download and Configure Mission Planner**:
  - Download from [Mission Planner Installation](https://ardupilot.org/planner/docs/mission-planner-installation.html).
  - Set up initial parameters and calibrate sensors as outlined in the guide.

For detailed programming instructions and advanced configurations, please consult the full [ROV Avionics Instructions PDF](https://github.com/ObinnaNdbs/Mars-Rover/blob/main/Documents/ROV_Avionics_instructions.pdf).

# IMAGES
<img width="363" alt="f5c585bb904a65383c13b7ad762eda2" src="https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/e64ecc08-0eb4-47c1-bb5b-e44e1083334e">
<img width="224" alt="c172db9c1a4207907664e5a3ea088ab" src="https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/551d5225-48c6-4de4-94e1-6c883ec10ad9">
<img width="611" alt="707502d3d256394f6c20bf9a6e94ac4" src="https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/f39bfd0e-5a64-484a-9de8-0004bca12208">
<img width="509" alt="5df5961ba5c4779e7d03f84a789e2ac" src="https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/cfafac41-572f-4938-95b0-25ae28837cc8">
<img width="630" alt="5df5961ba5c4779e7d03f84a789e2ac" src="https://github.com/ObinnaNdbs/Mars-Rover/assets/159606096/24aaa93f-3403-4414-866e-20b3882f11ae">

