# 🏠 Smart Home Automation System (Java)

A reference implementation of a **Smart Home Automation System** in Java, designed with **SOLID principles** and classical design patterns:  
- **Singleton** for central controller instance  
- **Factory** for creating devices (`Lights`, `Thermostat`, `Security Camera`)  
- **Abstract Factory** for device brand families (`PhilipsFactory`, `SamsungFactory`)  
- **Builder** for assembling complex automation scenes (`MorningRoutine`, `NightMode`)  
- **Observer** for updating devices when a scene or mode changes  
- **Strategy** for different energy-saving algorithms  

## ✨ Features

- Centralized **HomeController** (singleton)  
- Pluggable device creation via **Factory Pattern**  
- Brand-specific device families using **Abstract Factory**  
- Complex automation routines assembled with **Builder**  
- Real-time device updates on scene changes (**Observer**)  
- Flexible energy management via **Strategy** algorithms  

## 🧠 SOLID Principles Mapping

- **S**ingle Responsibility → Each class focuses on a single concern (e.g., `SceneBuilder` only builds automation scenes).  
- **O**pen/Closed → Extend system (new devices, scenes, or strategies) without modifying core logic.  
- **L**iskov Substitution → All device subclasses (`Light`, `Thermostat`, etc.) behave as `Device`.  
- **I**nterface Segregation → Small, focused interfaces (`DeviceObserver`, `EnergyStrategy`).  
- **D**ependency Inversion → High-level modules (`HomeController`) depend on abstractions (`DeviceBrandFactory`, `EnergyStrategy`) instead of implementations. 
