# 🏁 Midnight Circuit: Urban Racer

## 📌 Project Title
**Midnight Circuit: Urban Racer**

---

## 👥 Group Members
- Student A – UML & Design  
- Student B – Core Classes (Racer, Player, Rivals)  
- Student C – Interfaces & Item System  
- Student D – Game Logic (Race, LevelBuilder)  
- Student E – Exception Handling & Testing  
- Student F – Shop, UI, Game Controller  
- Student G – Documentation & Report  
- Student H – GitHub Integration & README  

---

## 🎮 Project Description
**Midnight Circuit: Urban Racer** is a turn-based, menu-driven console game developed in **C#** using **Object-Oriented Programming (OOP)** principles.

Players compete in underground street races across **4 progressively challenging levels**, managing resources, using items strategically, and overcoming environmental hazards to win.

---

## 🚀 System Features
- 🔁 Turn-based race loop with player and AI rivals  
- 🏎️ 2 rival types:
  - AmateurRival  
  - ProRival (with Drafting AI)  
- 🧰 3 item types:
  - Nitro Boost  
  - Performance Tires  
  - EMP Jammer  
- ⚠️ 3 hazard types:
  - Engine Overheating  
  - Police Intervention  
  - Road Debris  
- 🏁 4 levels with increasing difficulty  
- 🛒 Pre-race shop system using in-game currency (Cash)  
- ⭐ Reputation-based progression system  
- 🎒 Full inventory management system  

---

## 🧠 OOP Concepts Used

### 🔒 Encapsulation
- Private fields with public properties in all classes  

### 🧬 Inheritance
- `Racer` → Player, AmateurRival, ProRival  
- `Item` → Nitro, PerformanceTires, EmpJammer  
- `Hazard` → EngineOverheat, PoliceIntervention, RoadDebris  

### 🔄 Polymorphism
- `PerformAction()` overridden in Racer subclasses  
- `DisplayStats()` customized in Player and Rivals  
- `Use()` overridden in Item subclasses  

### 🔌 Interfaces
- `IUsable` → Items  
- `IDamageable` → Racers  
- `IDisplayable` → All entities  

### 📚 Collections
- `List<Item>` in Inventory  
- `List<Racer>` in Race  

### ⚠️ Exception Handling
- Implemented using try-catch in:
  - Game  
  - Inventory  
  - Player  
  - Race  

---

## ▶️ How to Run the Program

### 📋 Requirements
- .NET 8 SDK or later  
- Windows / macOS / Linux  

### 🛠️ Steps

```bash
# 1. Navigate to the project folder
cd path/to/MidnightCircuit

# 2. Build the project
dotnet build

# 3. Run the project
dotnet run
