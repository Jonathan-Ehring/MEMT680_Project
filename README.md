**TO RUN THE PROGRAM: launch the jupyter notebook FCDI_app.ipynb****

Project Background:

Flow capacitive deionization (FCDI) is a method of water desalination that is electrically driven and more energy efficient compared to reverse osmosis (RO) at lower salt concentrations. Given the high number of inputs (voltage, flow rate, carbon loading, salt concentration, electrolyte (NaCl, NaOH, etc.), temperature, flow field geometry, conductive additive loading, dispersant loading, emulsifier loading, and other materials selection), optimization of FCDI is difficult and tedious to conduct. Previous studies [1] have performed optimization of FCDI under constant voltage, flow rate and salt concentration. There has yet to be a study of FCDI that performs under dynamic conditions. For instance, decreasing the flow rate and voltage towards the end of the desalination process may increase efficiency. 

Project Objectives:
1) Create a dashboard capable of visualizing and packaging the real-time experiments
2) Explore which algorithms would be best suited for the FCDI application
3) Perform active learning (bayesian) optimization

The experimental setup is outlined below: 

![image](https://user-images.githubusercontent.com/14908470/205165257-d47d0086-d475-4ed7-9620-349fa3a55e2a.png)

FCDI experiments can be launched using the Plotly Dashboard (FCDI_app.ipynb) with the following steps:
1) Connect to potentiostat and arduino. The potentiostat will connect and load firmware to channel 1 of the VSP. If you are using a different Biologic potentiostat, the software will detect and upload the firmware, however, if you are connected to another channel other than channel 1, you must change this variable in (). 
2) Enter systems parameters. These are the initial conditions of the experiment. The system will update the user periodically on the state of the system and provide an alert once the initial conditions are reached. 
3) Select an electrochemical technique and input the desired technique parameters. 
4) Begin the experiment and observe the sensors and data output in real time using the Real-Time Plotting Page. 

![image](https://user-images.githubusercontent.com/14908470/205166546-9417acfd-fbaf-482a-bba2-340c2cfeb121.png)

Real-Time Plotting:
1) The systems sensor are plotted in real-time. Dummy data is shown below. 
![image](https://user-images.githubusercontent.com/14908470/205167638-b0dc380c-70f8-457c-ab42-527acf94f982.png)

Data Visualization:
1) Large data sets can be loaded and visualized by selecting parameters to inculde through the dropdown and knob components. 
![image](https://user-images.githubusercontent.com/14908470/205167924-786b3eca-3158-4810-8983-b1ca6036bf3a.png)


ML Training:
TBA 





References
[1] Optimal conditions for efficient flow-electrode capacitive deionization
