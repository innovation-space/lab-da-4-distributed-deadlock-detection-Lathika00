
# Distributed Deadlock Detection

## Description
This project simulates distributed deadlock detection using the Wait-For Graph and probe (edge-chasing) algorithm. It shows how processes detect deadlock without a central controller.

## Technologies Used
- SimPy  
- Streamlit  

## Algorithm
- Each site maintains a Wait-For Graph  
- Edge Pi → Pj means Pi is waiting for Pj  
- A probe <initiator, sender, receiver> is sent  
- If the probe returns to the initiator → Deadlock detected  

## Features
- Works for any number of processes  
- Deadlock / No Deadlock scenarios  
- Execution trace display  
- Message complexity shown  

## Message Complexity
- Depends on number of edges  
- General: O(E)  
- Worst case: O(N)  

## How to Run
pip install -r requirements.txt  
python -m streamlit run wait_for.py  

## Conclusion
Deadlocks are detected by identifying cycles in the Wait-For Graph using probe messages.
