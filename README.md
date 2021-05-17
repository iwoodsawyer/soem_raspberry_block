[![View Simple EtherCAT Master Block SFunction for Raspberry Pi on File Exchange](https://www.mathworks.com/matlabcentral/images/matlab-file-exchange.svg)](https://www.mathworks.com/matlabcentral/fileexchange/75376-simple-ethercat-master-block-sfunction-for-raspberry-pi)

# Simple EtherCAT Master Block SFunction for Raspberry Pi
The example Simple EtherCAT Slave Driver Block SFunction for Raspberry Pi shows basic usage of the Simple Open EtherCAT Master (SOEM) library by transferring 32 bytes of input and output PDO data.

Usage instructions:
1. Download SOEM library from https://github.com/OpenEtherCATsociety/SOEM
2. Unpack SOEM library to the same map of this simulink model
3. (Optional) Compiled SOEM librray for Mathworks Raspbian R21 is already included, but for other OS than Raspbian the SOEM library should be recompiled with following substeps.
   - Build the SOEM library on the Raspberry Pi hardware using the instructions on https://github.com/OpenEtherCATsociety/SOEM. 
   - Copy libsoem.a from the build folder to the map of this simulink model.
6. Open Simulink model "raspberrypi_ethercat_master.slx".
7. Open the EtherCAT Master block, and in the "Libraries" tab adjust the INC_PATHs to the correct paths of the SOEM include folders.
8. Build the SOEM_raspberrypi Sfunction.
9. Deploy the model to the Raspberry Pi hardware.
