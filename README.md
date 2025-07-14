# Queue Management System

A simple Python-based Queue Management System that simulates customers joining regular or priority queues and being served at multiple counters. This project is a console-based simulation, ideal for learning about queue data structures, simulation logic, and basic OOP in Python.

## Features

- Separate **Regular Queue** and **Priority Queue**.
- Multiple service counters (configurable).
- Customers can join either queue.
- Priority customers are always served before regular customers.
- Tracks and displays queue status and counter status.
- Shows wait time for each customer served.
- Interactive command-line interface.

## Requirements

- Python 3.x

## How to Run

1. **Clone or download this repository.**
2. Open a terminal or command prompt and navigate to the project directory.
3. Run the following command:

   ```bash
   python Queue_managment.py
   ```

4. Follow the on-screen menu to interact with the system.

## Menu Options

1. **Add Regular Customer**: Adds a new customer to the regular queue.
2. **Add Priority Customer**: Adds a new customer to the priority queue.
3. **Serve Customer**: Assigns the next waiting customer to a free counter (priority queue served first).
4. **Complete Service at Counter**: Marks a customer as served at a specific counter, freeing the counter.
5. **Display Queue**: Shows the current state of both queues.
6. **Display Counters**: Shows which counters are free or serving which customers.
7. **Exit**: Ends the simulation.

## Example Usage

```text
Welcome to the Queue Simulation System!
1. Add Regular Customer
2. Add Priority Customer
3. Serve Customer
4. Complete Service at Counter
5. Display Queue
6. Display Counters
7. Exit

Enter your choice: 1
Customer-1 has joined the Regular queue.

Enter your choice: 2
Customer-2 has joined the Priority queue.

Enter your choice: 3
Customer-2 is being served at Counter-1. (Waited 0.01 seconds)
```

## Customization

- **Number of Counters:** You can change the number of counters by modifying the `num_counters` argument in the `QueueSimulation` class instantiation at the bottom of the script.

  ```python
  simulation = QueueSimulation(num_counters=3)
  ```

## License

This project is open-source and free to use for educational purposes.

---
**Author:** [Prasath]
