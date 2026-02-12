# 4.-Design-and-Simulation-of-Full-wave-rectifier-controlled-by-a-thyristor
## AIM
To design, simulate and analyse a full wave rectifier controlled by thyristors using MATLAB Simulink.
## APPARATUS REQUIRED
•	MATLAB
## PROCEDURE
1.	Open MATLAB and click on the icon for SIMULINK as shown below
 <img width="522" height="376" alt="image" src="https://github.com/user-attachments/assets/cc714a4d-8634-445d-b8af-21bb59f44617" />

Another way is to open is through START icon of MATLAB Start ⇒ Simulink ⇒ Library  browser. 

2.	Click on NEW MODEL or go to FILE ⇒ NEW ⇒ MODEL and a new blank model is created as shown below
 <img width="572" height="382" alt="image" src="https://github.com/user-attachments/assets/9af61610-084a-4f5d-8e67-0924fd22c890" />

3.	After creating a blank model you need to open the SIMULINK component storeroom/library by going to View ⇒ Library Browser. Select SIMPOWER SYSTEMS then select Power Electronics library and by right clicking on Thyristor and click on add to the model will add the Thyristor in the blank model. Alternatively you can drag the component directly in the model page as shown below
 <img width="940" height="361" alt="image" src="https://github.com/user-attachments/assets/59888715-c4ac-4bf8-8445-30c7c4bd6e31" />

4.	Similarly go to ELECTRICAL SOURCES ⇒ AC Voltage Source and add it to the model. Select Elements and select “SERIES RLC BRANCH” and add it to the model. Simulink do not perform simulation unless and until a measurement block is present in a system. Since we need to measure the input and output voltages and the load current. To add them select Measurement in SIMPOWER SYSTEMS and then add current measurement and voltage measurement blocks to the model. Oscilloscope is not included in SIMPOWER SYSTEMS and is present in the top most block of the left column that is SIMULINK ⇒ Sinks ⇒ Scope. Also add PWM generator from sourced. We can join various blocks by clicking
on their edges and then drag the wire till the other connection terminal.
5.	Construct the circuit by joining them together in the form as given below
 <img width="940" height="369" alt="image" src="https://github.com/user-attachments/assets/09311276-5e10-44b5-afc3-560959183850" />

6.	Now double click the voltage block to set the values of voltage and frequency.
 <img width="349" height="325" alt="image" src="https://github.com/user-attachments/assets/dd8ea140-ab78-482a-8c32-21c464e6b708" />

7.	Double click on Thyristor and you can set various parameters for Thyristor according to the specific data sheet.
8.	Double click on series RLC branch, Select the Branch type as R and set the values for R.
9.	Double click on PWM generator, set the parameter as per the requirement.
 <img width="377" height="443" alt="image" src="https://github.com/user-attachments/assets/4aa1bd69-0587-4063-9746-3507b0d0fdd8" />

10.	In the Scope menu “>” is shown which can only be connected to the inverse icon “<” in the measurement blocks.
11.	Double click on SCOPE and then click on parameter icon as shown
 <img width="838" height="377" alt="image" src="https://github.com/user-attachments/assets/3605a795-2cd1-4746-b5a7-3ab209cb8691" />

12.	Make the number of axes as required.
13.	Before simulation also adjust the data history of scope by following
 <img width="363" height="278" alt="image" src="https://github.com/user-attachments/assets/e8d9af71-b299-4eaa-89c5-d5a41867f375" />

14.	Before running the simulation, we have to configure the parameters. Go to Simulation ⇒ Configuration parameters as shown
 <img width="542" height="399" alt="image" src="https://github.com/user-attachments/assets/a81746fc-b597-42d0-bd2e-77b1dae3e489" />

15.	Select the ode23tb (Stiff/TR-BDF2) or ode15s (Stiff/NDS) or any suitable solver as
shown below 
 <img width="566" height="401" alt="image" src="https://github.com/user-attachments/assets/eedae68e-014b-4c0a-a0ad-fc9e351a4eec" />

16.	Start the simulation by either clicking on Start Simulation icon as shown in below or
by going to Simulation ⇒ Start
 <img width="770" height="308" alt="image" src="https://github.com/user-attachments/assets/4e8dffc2-d1d0-483a-9012-f27cc2cb61f9" />

17.	Double click on scope and observe the graphs.
18.	Left click on any graph and drag to make a rectangle to get the waveforms for a small period of time.
19.	Right click on each graph and select the axes properties and label each graph.
20.	Save the file. ( It should be noted that Simulink do not allow to save files with spaces therefore usually is included in between two words.)
21.	Analyze and record your inference.

## Task
Design, Simulate and analyse single phase full wave rectifier controlled by SCR with the following details 
Vm=100
Frequency = 50Hz
Resistance = 1 ohm
Phase delay or delay angle of Thyristor = 45 degree
After analysing the simulated output,
(i)Draw various simulated waveforms on the graph sheet
(ii) Change the value of resistance to 2 ohm, simulate and draw the current waveform on the graph sheet.
(iii) Change the firing angle to 90 degree, simulate and draw the Output voltage and current waveform on the graph sheet.
(iv)Write your inference.

## Simulation
<img width="1702" height="597" alt="image" src="https://github.com/user-attachments/assets/bcd30710-442c-4e56-891a-5715952c0222" />

## Output
<img width="1897" height="947" alt="image" src="https://github.com/user-attachments/assets/e67237b8-d804-4e4d-8c21-3c4e549de88b" />

## Result
Thus the experiment was simulated and output was verified succesfully
