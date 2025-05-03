#  AI Multi-Agent Self-Driving Car Simulation

This project simulates a 2D grid-based self-driving car environment powered by a modular **multi-agent AI system**. Each agent is responsible for a distinct task—planning, executing, decision-making, or perception—emulating real-world autonomous driving systems. The agents communicate using structured messages, and decisions are generated using a powerful LLM (LLaMA 3 via Groq API).
---
##  Objective

To demonstrate how autonomous vehicles can make intelligent decisions in dynamic environments using a team of AI agents that coordinate in real time.

---

##  **Key Components:**

###  **Agents:**
- **Planner Agent**: Computes optimal paths using user-defined algorithms like A* or Dijkstra.
- **Executor Agent**: Follows the planned path and simulates vehicle movement.
- **Decision Agent**: Evaluates traffic signals and obstacles to update vehicle behavior.
- **Perception Agent**: Simulates object recognition and traffic data.

###  **Environment:**
- 2D grid environment (e.g., 12x12 grid).
- Configurable obstacles and blocked cells.
- Flexible grid initialization and route customization.
  
### **Dynamic Syncing:**
* The grid updates in a loop (simulating traffic changes).
* After each update, the agents re-coordinate:
* The Perceptor observes and sends inputs.
* The Planner recalculates.
* The Decision Agent chooses the action.
* The Executor moves the car accordingly.
* This cycle mimics real-time adaptive autonomy.

### **Technologies:**
- Python (Jupyter Notebook)
- AutoGen multi-agent system
- Groq API with LLaMA 3.3-70B Versatile model
- Matplotlib / Grid visualization (optional)


