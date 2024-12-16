# trailway-DC-motor-control
MATLAB, Simulink (R2022b) | DC motor simulation | DC motor control tuning

This repository contains the code (MATLAB scripts and Simulink model) and report of the final assignment of a course on [Dynamics of Electrical Machines and Drives](https://www11.ceda.polimi.it/schedaincarico/schedaincarico/controller/scheda_pubblica/SchedaPublic.do?&evn_default=evento&c_classe=837862&__pj0=0&__pj1=52cb81e9c76fcd372f5858307a2f494a). 

## Introduction

<image width=450 height=300 src=https://github.com/user-attachments/assets/69c0d49c-2d90-466f-a51d-66bbb70e54d5>
<image width=450 height=300 src=https://github.com/user-attachments/assets/3c34841f-f26d-4c61-b2f6-871b0456881c>
  
<br/>
<br/>

In this project, I developed **MATLAB** and **Simulink** software to simulate and control the **DC Separately Excited Motor** used in the original "Carrelli 1928" Tram of Milan. 

## Objective 
Given the datasheet of the motor under analysis, and additional data on the load and the railway track: 
- Find the Motor Design parameters
- Tune and Simulate speed/current control (motor driver), showing its reliability on the defined track.

Rely on classical **Bode** theory to analyze control performances, and prove it in simulation. 


For further details on the task and my solution (step by step), look at my [Report](https://github.com/AlePuglisi/trailway-DC-motor-control/blob/main/DC_Motor_Report.pdf)

## Simulink scheme and Simulation

<image width=1200 height=400 src=https://github.com/user-attachments/assets/eb7d8686-83d8-411f-8b51-b7ee24d26fa6>
(Refer to the Report for a description of each part in detail)
<br/>To simulate the system: 

- Run the MATLAB script: DCTractionMotor.m <br/>
    For motor parameter computation, tuning, and Bode diagram analysis.<br/>
    This will upload all the variables used in the Simulink scheme in the Workspace. 
- Run the Simulink scheme: DCTractionMotorScheme.slx

## Conclusion

The Control gains obtained from the dynamic model imposing Loop shaping of the Bode diagram, provide satisfactory performance, with accurate set point tracking in speed and current.<br/>
It is possible to experiment with this Simulink scheme and MATLAB code to check what happens if we change the track, and how different gains affect performances. 




