# AWR6843AOPEVM Project
This repository contains a study performed on Texas Instrument's mmWave radar device- AWR6843AOP evaluation board, used for industrial/ automobile applications. Additionally, a feature is added to extract a small portion of radar data from the enormous radarcube data processed by the board.


## Tools
1. AWR6843AOPEVM
2. UniFlash software
3. TI's mmWave Demo-Visualiser
4. DCA1000EVM
5. CP2105 drivers

## Documentation
The pdf documents provide support documentation on the device, alongwith datasheets. There is user guide documentation provided for the other tools used as well. 

## Objective
Radar sensors transfer data in raw ADC form, which is in a cube format, and hence, called radarcue data. The amount of information shared by the radar sensor is substantial. The objective of this project is to extract a handful
of information from the entire raw ADC data.  
![image](https://github.com/user-attachments/assets/00a9d15f-a8d8-4327-9f1f-0fbdffd0af4d)  
Shared above is the composition of the raw ADC data and its formatting as a radarcube. 

## Setup
The Out-of-Box demo, shared by Texas Instruments as one of the many sample projects, was used as a sample data source generation program. UniFlash was used to dump the binary file onto the program memory built onto the radar device. 
The mmWave Demo Visualiser was used to visualise the sensor data coming from the device, and create a data file to log the data. The configuration files were used to initially configure the Demo Visualiser setup. As the data is in serial format, parsing scripts were used to generate the data in readable format.

