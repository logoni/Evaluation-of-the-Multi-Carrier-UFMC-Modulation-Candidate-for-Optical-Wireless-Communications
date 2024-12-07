# Evaluation-of-the-Multi-Carrier-UFMC-Modulation-Candidate-for-Optical-Wireless-Communications
The practical part focuses on the construction of UFMC modulation technique for optical wireless communication in Matlab Simulink. 

In the figure, the edited blocks are highlighted in green and red.
The green blocks contain the modified transmitter and receiver structure for the required UFMC modulation technique. 

![image](https://github.com/user-attachments/assets/d68b7650-f8d4-48b2-94bf-0aed4b44cbca)

The red block is the FSO environment in which the 3 basic parameters are counted and changed. 
The first of the main parameters is the adjustment of the laser visibilities for different weather conditions ranging from dense fog to clear sky visibility, these values are determined based on Kim's model which calculates the transmission path attenuation at different transmitter visibility lengths.

![image](https://github.com/user-attachments/assets/25b340dd-6135-4653-8bbb-76dc28361993)

Another factor is the ligatures (turbulence) that arise from the mixing of different air temperatures, which causes the vacuum densities to change during external transmission. The values were calculated using the relationship from the Rytov approximation. 
Strong turbulences have a value of Cn2 = 10-14 m-2/3, medium strong Cn2 = 10-15 m-2/3 and weak Cn2 = 10-16 m-2/3:

![image](https://github.com/user-attachments/assets/582d80ae-cd18-4407-bdbc-54ae6b9bdca1)

The last factor is the geometric losses. The values of these parameters were taken from devices used in practice and used to calculate the power of the transmitters through the relation:

![image](https://github.com/user-attachments/assets/2f8846a8-662c-46db-8d16-05f8f36b629c)

By summing the parameters of turbulence, visibilities and geometrical losses, we obtained the total attenuation of our transmission path in the outdoor environment.
