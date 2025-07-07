# Queue Management System 🏦

A Python-based simulation for managing queues efficiently using the `deque` module. This project simulates a real-world waiting line, supporting both priority and regular queues, multiple counters, and live service management. Ideal for learning queue logic, priority handling, and basic system simulation.

---

## 🚀 Features

- **Priority & Regular Queues:** Handles both regular customers and those with priority needs.
- **Multiple Counters:** Service multiple customers simultaneously, just like in banks or hospitals.
- **Dynamic Service:** Serve customers based on priority, track wait times, and manage counter status.
- **Interactive CLI:** User-friendly command-line interface for adding, serving, and completing customers.
- **Realistic Simulation:** Tracks each customer’s wait time and provides live status updates.
- **Easy Customization:** Change number of counters and extend logic as needed.

---

## 🛠️ Tech Stack

- Python 3.x
- Standard Library: `collections.deque`, `time`

---

## 📦 How to Run

1. **Clone this Repo:**
   ```bash
   git clone https://github.com/prasath-m21/queue-management-system.git
   cd queue-management-system
   ```

2. **Run the Simulation:**
   ```bash
   python queue_simulation.py
   ```

---

## 🧑‍💻 Usage Demo

```python
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

---

## 📝 Code Highlight

```python
def serve_customer(self):
    for counter, customer in self.counters.items():
        if customer is None:
            # Serve from priority queue first
            if self.priority_queue:
                next_customer = self.priority_queue.popleft()
            elif self.regular_queue:
                next_customer = self.regular_queue.popleft()
            else:
                print("No customers in the queue!")
                return
            self.counters[counter] = next_customer
            wait_time = time.time() - self.customer_times.pop(next_customer, time.time())
            print(f"{next_customer} is being served at {counter}. (Waited {wait_time:.2f} seconds)")
            return
    print("All counters are busy! Please wait.")
```

---

## ✨ Why This Project?

This simulator is a great way to understand queue data structures, priority handling, and multi-counter service logic. It’s perfect for students, interview prep, or anyone looking to learn core Python and system simulation concepts.

---

## 📫 Connect With Me

- **Portfolio:** [prasath-m21.github.io/Profile/](https://prasath-m21.github.io/Profile/)
- **GitHub:** [prasath-m21](https://github.com/prasath-m21)
- **LinkedIn:** [prasathm21](https://www.linkedin.com/in/prasathm21)

---

## ⚡ Fun Fact

> I love playing cricket & watching movies!  
> Always learning something new.

---

Feel free to fork ⭐, contribute, or reach out for collaboration!

