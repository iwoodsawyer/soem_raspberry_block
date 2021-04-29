# Simple EtherCAT Master Block SFunction for Raspberry Pi
The example Simple EtherCAT Slave Driver Block SFunction for Raspberry Pi shows basic usage of the Simple Open EtherCAT Master (SOEM) library by transferring 32 bytes of input and output PDO data.

Usage instructions:
1. Download SOEM library from https://github.com/OpenEtherCATsociety/SOEM
2. Unpack SOEM library to the same map of this simulink model
3. (Optional) Compiled SOEM librray for Raspbian is already included, but for other OS than Raspbian the SOEM library should be recompiled with following substeps.
   3.1. Build the SOEM library on the Raspberry Pi hardware using the instructions on https://github.com/OpenEtherCATsociety/SOEM. 
   3.2. Copy libsoem.a from the build folder to the map of this simulink model.
3. Open Simulink model "raspberrypi_ethercat_master.slx".
4. Open the EtherCAT Master block, and in the "Libraries" tab adjust the INC_PATHs to the correct paths of the SOEM include folders.
5. Build the SOEM_raspberrypi Sfunction.
6. Deploy the model to the Raspberry Pi hardware.
