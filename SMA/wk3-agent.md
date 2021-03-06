# Agent based modelling

**Summary of operations**

- Steps through time in increments 
- In each increment: adds, updates, and removes agents
- Describes agent behavior with nested switch statements based on modal analysis



**Used to simulate complex systems** 

-  The elements of a system are called agents
- The agents has individual behavior
- Agents can be influenced by other agents
- Agents can change the conditions of the environment where they are located
- Agents can be influenced by the conditions of the environment where they are located



**Advantages** 

- Enables to capture more complex structures and dynamics
- Can simulate problems modeled by System Dynamics and Discrete-Event Simulation
- The modeler defines behavior at individual level, and the global behavior emerges as a result – bottom up approach
- Allow better visualisation of the system

**Drawbacks** 

- Computationally Intensive 
- Time consuming 
- Harder to develop





**Sample [predator-prey](http://netlogoweb.org/launch#http://netlogoweb.org/assets/modelslib/Sample Models/Biology/Wolf Sheep Predation.nlogo) with agent based modelling**

- Environment Rules - Grass turns to mud if eaten, Grass grows back after a certain amount of time 
- Wolf Rules - Needs to eat sheep for energy - Can Reproduce - Will die without energy 
- Prey Rules - Needs grass for energy - Can Reproduce - Will die without energy

![image-20190930094738286](assets/image-20190930094738286.png)





**Sample patient-waiting room with agent based modelling**

![Screenshot 2019-09-30 at 9.50.39 AM](assets/Screenshot 2019-09-30 at 9.50.39 AM.png)

Since we do not give different treatment to Type A patient and Type B patient, in the long run the average time for both patients should be the same.



Modal Analysis

![Screenshot 2019-09-30 at 10.28.03 AM](assets/Screenshot 2019-09-30 at 10.28.03 AM.png)

Each patient has a state - untreated, waiting, staging, intreatment, treated, discharged.

Then the rest of the lecture is an introduction to the Javascript code.
- `filter()`, `map()` and `reduce()`with a 'lambda' function.
- `switch` and `case` to manage different states
- You need to initialise the data as well



**Homework  - Priority Agent Model**

- Change the scheduling rules so that A-type patients get priority
- But be careful: too much priority can lead to an exploding queue of B-type patients 



**Homework - Non-Colliding Agents**

- The basic agent model has no limit on the number of patients in the waiting room (they can stack up wherever they sit)
- If we impose a non-colliding rule, then each cell of the waiting room can hold only one patient 
- What happens if a patient arrives and all cells are occupied?
- We mark that patient as “DISCHARGED” and send them to a different exit (anywhere else on screen) 
- The current code will remove that patient when he/she reaches the exit



**Question: What is D3?**

Functional programming is useful
- For filtering and updating arrays
- For displaying and animating data (eg. D3)
- But, requires mastery of lambda functions and chaining



**Variations of the model**
A more complex version of this model is sufficient for your project. It is copy-pasting parts of your code.

- Shopping at a physical store
  - Random walk in the store before going to the cashier
- Food court model 
  - Consider people coming in groups and sitting together
- Traffic junction
  - What 
- Airport
  - Consider runway and dock constraints



Project idea 
- potential optimisation of smart traffic lights
- modelling the hostel lift in the morning
