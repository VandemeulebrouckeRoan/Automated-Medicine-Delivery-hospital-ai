# 🤖 Automated Medicine Delivery System

## 📌 Overview
This project is a Unity-based AI simulation where an autonomous robot learns to collect and deliver medicine inside a hospital environment.

The system uses reinforcement learning (Unity ML-Agents) to train an agent that can:
- Navigate through the environment  
- Pick up the correct medicine  
- Deliver it to the correct location  
- Avoid obstacles such as walls  

---

## 🚀 Features
- Autonomous robot agent trained with reinforcement learning  
- Multi-room medicine request system  
- Different medicine types and delivery logic  
- Reward system for correct behavior (pickup, delivery, navigation)  
- Manual control mode for testing (heuristic mode)  

---

## 🛠️ Tech Stack
- Unity (6000.0.38f1 or compatible)  
- C#  
- Unity ML-Agents  
- ONNX (trained model)

---

## ▶️ How to Run

### 1. Open the project
- Open Unity Hub  
- Click "Add project" and select this folder  
- Open it with Unity version **6000.0.38f1** (or closest compatible)

---

### 2. Open the main scene
- Go to: `Assets/Scenes/Project.unity`  
- Open the scene  

---

### 3. Run the simulation
- Press **Play** in Unity  
- The agent will run using the trained model (`.onnx` file)

---

## 🎮 Manual Controls (Testing Mode)

To manually control the robot:

1. Select the agent in the scene  
2. In **Behavior Parameters**, set:
   - Behavior Type → `Heuristic Only`

### Controls:
- **W** → Move forward  
- **A** → Turn left  
- **D** → Turn right  
- **Space** → Interact (pickup/drop)

---

## 🧠 AI Behavior
The agent is trained using reinforcement learning with a reward system:
- ✅ Reward for picking up correct medicine  
- ✅ Reward for successful delivery  
- ❌ Penalty for hitting walls  
- ❌ Penalty for incorrect actions  

---

## 📁 Project Structure (important parts)
- `Assets/Scenes/Project.unity` → Main scene  
- `Assets/Scripts/` → Core logic (agent, environment, requests)  
- `Assets/*.onnx` → Trained AI model  

---

## 📌 Notes
- Make sure ML-Agents is properly installed in Unity  
- If the agent does not move, check the Behavior Parameters and model assignment  

---

## 👨‍💻 Author
Roan Vandemeulebroucke
