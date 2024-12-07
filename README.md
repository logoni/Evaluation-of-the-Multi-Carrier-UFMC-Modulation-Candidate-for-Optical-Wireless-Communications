# Evaluation-of-the-Multi-Carrier-UFMC-Modulation-Candidate-for-Optical-Wireless-Communications
The practical part focuses on the construction of UFMC modulation technique for optical wireless communication in Matlab Simulink. 

In the figure, the edited blocks are highlighted in green and red.
The green blocks contain the modified transmitter and receiver structure for the required UFMC modulation technique. 
The red block is the FSO environment in which the 3 basic parameters are counted and changed. 
The first of the main parameters is the adjustment of the laser visibilities for different weather conditions ranging from dense fog to clear sky visibility, these values are determined based on Kim's model which calculates the transmission path attenuation at different transmitter visibility lengths.

![image](https://github.com/user-attachments/assets/e80f4fcc-5cd3-48a6-9cff-c522cd32a1f6)

Another factor is the ligatures (turbulence) that arise from the mixing of different air temperatures, which causes the vacuum densities to change during external transmission. The values were calculated using the relationship from the Rytov approximation. 
Strong turbulences have a value of Cn2 = 10-14 m-2/3, medium strong Cn2 = 10-15 m-2/3 and weak Cn2 = 10-16 m-2/3:

![image](https://github.com/user-attachments/assets/73b0be88-57ab-4503-b9eb-f146935a40d0)

The last factor is the geometric losses. The values of these parameters were taken from devices used in practice and used to calculate the power of the transmitters through the relation:

![image](https://github.com/user-attachments/assets/c774cf03-74cc-4d70-be71-4cee23e18229)

By summing the parameters of turbulence, visibilities and geometrical losses, we obtained the total attenuation of our transmission path in the outdoor environment.
