## State Machine PID

This project implements a PID control application based on the **Simple State Machine** LabVIEW Sample Project. You can use it as an example of how to modify the Sample Proejct.

There is two ways to run a PID control here: 

* **Simulated** - Just run the control with a simulated plant.
* **Hardware** - you can use a NI-DAQ Hardware with NI-DAQmx to perform the control on a real-world plant.

>Feel free to modify it to accomodate other hardware interfaces, such as a microcontroller. Do a pull request after it so we can keep the project alive.

The image below represents the general diagram for a PID Control.

![PID Control](https://ni.scene7.com/is/image/ni/12fbdcae1635?scl=1)

## The Code

The main code implements a state machine. Find below the state diagram for this project (it is also on the fron panel)

![State Diagram](https://github.com/FloresFelipe/State-Machine-PID/blob/master/Controle%20PID/documentation/StateMachineDiagram.PNG)

Find below the implementation of each of those states in the LabVIEW Code.

![Initialize](/Controle%20PID/documentation/PID_Maind1.png)

![Wait Event](/Controle%20PID/documentation/PID_Maind2.png)

![Update PID Settings](/Controle%20PID/documentation/PID_Maind5.png)

![Start DAQ](/Controle%20PID/documentation/PID_Maind6.png)

![Stop DAQ](/Controle%20PID/documentation/PID_Maind10.png)

![Exit](/Controle%20PID/documentation/PID_Maind11.png)


## How it works

It is actually pretty straightforward. Just run the VI, go to the **Configuração** tab to set the PID Controller constants, choose if you want to run it simulated or using hardware. Go back to the **Monitoramento** tab to run the controller.

See the animation below to check how it works.

![VI Operation](/Controle%20PID/documentation/pidViWorking.gif)

>Yes, the interface is in portuguese. Feel free to translate to your languange :smile:
