# 🏁 Midnight Circuit: Urban Racer

## 📌 Project Title
**Midnight Circuit: Urban Racer**

---

## 👥 Group Members
- Muhammad Aiman (24005672) – Core Classes, Game Logic, UML & Design
- Luth Adam (25014453) – Exception Handling, Testing, UML & Design
- Ikhwan Haziq (25014483) – Interfaces, Item System, Documentation & Report
- Danish Aiman (24005389) – Exception Handling & Testing
- Muhammad Aisar (25014021) – Exception Handling & Testing
- Fawwaz (24009550) – Shop, UI, Game Controller
- Noor Ilmam (25014255) – GitHub Integration & README

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

## 📂 Project File Structure
```text
MidnightCircuit/
├── Program.cs           # Entry point - starts the Game
├── Game.cs              # Game Controller - controls all flow and menus
├── Racer.cs             # Abstract base class for all racers
├── Player.cs            # Player class (extends Racer)
├── Rivals.cs            # AmateurRival and ProRival classes (extend Racer)
├── Item.cs              # Abstract Item base + specific Item subclasses
├── Interfaces.cs        # IUsable, IDamageable, IDisplayable definitions
├── Inventory.cs         # Manages the player's item collection (List<Item>)
├── Race.cs              # Turn-based race loop manager
├── Hazard.cs            # Hazard hierarchy + HazardFactory
├── Shop.cs              # Pre-race item shop logic
├── LevelBuilder.cs      # Builds rival rosters for each level
├── UI.cs                # Console display and input helpers
└── MidnightCircuit.csproj # C# project configuration file

