# Distributed Deadlock Detection using Wait-For Graph

## Description
This project simulates distributed deadlock detection using the Wait-For Graph model and edge-chasing (probe) algorithm.

## Technologies Used
- SimPy
- Streamlit

## Algorithm
Each site maintains a local Wait-For Graph.
A probe message <initiator, sender, receiver> is sent.
If the probe returns to the initiator, a deadlock is detected.

## Features
- Dynamic number of processes
- Deadlock / No Deadlock scenarios
- Execution trace visualization
- Message complexity analysis
  
## Message Complexity
- Depends on number of edges  
- General: O(E)  
- Worst case: O(N)  

## How to Run
pip install -r requirements.txt  
python -m streamlit run wait_for.py

## Output
- Wait-For Graph
- Probe execution trace
- Deadlock detection result

## Conclusion
Deadlocks are detected without a central coordinator by identifying cycles in distributed systems.
