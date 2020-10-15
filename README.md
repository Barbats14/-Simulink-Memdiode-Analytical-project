# -Simulink-Memdiode-Analytical-project

1)    Solver:                ode15(stiff/NDF)
      Min step size:         1e-18
      Relative tolerance:    5e-3
      
2)    I am using the pure differential equation (not the discretisized form) of Lamda, as seen in the Analytic Memdiode model file. Specifically, I have not separated the positive and negative voltages (i.e. Reset & Set), as Enrique has suggested becase I thinki it will be better to model it as a normal differential equation. At first, I used a switch to separate the two process but then I decided to do it this way.

3)   Several peculiarities I have identified:   

        -     I have used two 'initial conditions' (IC) blocks to start the simulation with the memory state, i.e. lamda, at 1 (or 0.001). However, I see that this actually makes no difference in the simulation.
        -   Even though the XY graph shows a normal , however far from the goal, behaviour, lamdaS never reaches 1. As you can see by loging the signal to the Simulation Data Inspection panel, it stops at 0.14. 
    
    
