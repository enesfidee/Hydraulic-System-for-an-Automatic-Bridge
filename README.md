# Hydraulic-System-for-an-Automatic-Bridge

# 1. Objectives
Design and control a hydraulic system that operates an automated bridge. The system aims to demonstrate efficient lifting and lowering mechanisms using hydraulic components while incorporating control strategies for automation.

# 2. Bridge Specifications
•	Material: Steel
•	Length (L): 20 meters (each side, total span = 40 meters)
•	Width (W): 8 meters
•	Thickness (t): 0.4 meters
•	Density of Steel (ρ) : 7850 kg/m³

  # Weight Calculation
    1.Each bridge side dimensions:
        o	Length (L): 20 meters
        o	Width (W): 8 meters
        o	Thickness (t): 0.4 meters
    2.	Volume of one side of the bridge: V=L×W×t=20×8×0.4=64 m³
    3.	Weight of one side: W=V×ρ×g=64×7850×9.81=4,924,032 N
    4.	Total weight for both sides: W total=2×4,924,032=9,848,064 N

# 3.	Component Selection

 ![image](https://github.com/user-attachments/assets/af645fa7-8a0e-4f46-bae2-095903d675aa)

Figure 1: Hydraulic System


 ![image](https://github.com/user-attachments/assets/1dd7e43e-b076-4ade-88ca-de44f8ec6bad)

Figure 2: Hydraulic Circuit


 ![image](https://github.com/user-attachments/assets/8e6e66f6-2efa-4140-ba4f-d44ebf624c44)

Figure 3: Ladder System


 ![image](https://github.com/user-attachments/assets/649ecb69-aa69-4b04-8c11-7b3a0e9a9dc2)

Figure 4: Electrical Circuit
(Input Simulate) is added to the circuit to simulate only the ship passage data


# Hydraulic Cylinder
  •	Bore Diameter: 485 mm
  •	Stroke Length: 2 m
  •	Pressure Rating: 250 bar (to ensure safety margin)
# Hydraulic Pump
  •	Flow Rate: 36.94 L/min per cylinder (total = 147.76 L/min for 4 cylinders)
  •	Pressure Rating: 250 bar
  •	Power Rating: 3000 kW
# Reservoir
  •	Capacity: At least 1.5 times the total fluid volume (approx. 300 L)
    Valves
  •	Directional control valves (4/3 way) with pressure rating of 250 bar.

# 4. Control System Design and Logic
The control system manages the automatic lifting and lowering of the bridge and ensures safety and efficiency. It includes:
# Control Logic
  1.	Initial State:
    •	Bridge is in the closed position.
    •	All valves are in the neutral position.
  2.	Lifting Sequence:
    •	Activation of the start button sends a signal to the controller.
    •	The controller energizes the directional control valves to extend the hydraulic cylinders.
    •	Position sensors monitor the cylinder stroke to ensure full extension.
  3.	Lowering Sequence:
    •	Activation of the lower button sends a signal to the controller.
    •	The controller reverses the valve positions, retracting the hydraulic cylinders.
    •	Position sensors monitor the retraction to ensure proper closure.

# Sensor and Feedback
  •	Position Sensors: Detect cylinder extension and retraction.
# Controller Design
  •	Ladder Diagram
  •	Ladder logic programming is used to control the sequence of operations.
  •	Inputs: Start, lower buttons, timer, position sensors.
  •	Outputs: Solenoid signals for directional control valves.

# 5. Bridge Inventor Design

 
 
The bridge was modeled in a Inventor to visualize the dimensions and mechanical structure. The drawing includes:
•	The two bridge sides.
•	Hydraulic cylinder mounting positions.
•	Pivot points for the double-opening mechanism.

# 6. Hydraulic Circuit Simulation
The hydraulic system was designed and simulated in Automation Studio. The circuit includes:
•	Hydraulic Pump: Provides pressurized fluid to the system.
•	Directional Control Valves: Controls the flow direction to the cylinders.
•	Hydraulic Cylinders: Operate the lifting mechanism.
•	Reservoir: Stores hydraulic fluid.
# Simulation Results
•	The system successfully lifted each side of the bridge within 10 seconds.
•	The flow rate and pressure were within the specified limits.
•	The safety factor ensured reliability under load conditions.
# 7. Conclusion
The proposed hydraulic system, consisting of four hydraulic cylinders, a pump, control valves, and a Ladder diagram, meets the requirements for lifting the double-opening bridge. The Inventor design, hydraulic simulation, and control logic validate the design's feasibility, ensuring adequate power, force, and reliability for safe operation.


