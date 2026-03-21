# 🚀 Rocker & Differential Bar Subsystem

This repository contains CAD files, renders, and documentation for two essential subsystems of a Mars Rover: the **Rocker** and the **Differential Bar**.

Together they form the core of the **Rocker–Bogie Suspension Mechanism**, enabling the rover to traverse uneven terrain while maintaining stability, traction, and balance.

---

# 🛰️ Rocker–Bogie Suspension Mechanism

The **Rocker–Bogie mechanism** is a passive suspension system widely used in planetary rovers.

Instead of springs or dampers, the system uses **mechanical linkages and a differential mechanism** to keep the rover stable while traveling across rough terrain.

The suspension consists of:

- **Rocker arms**
- **Bogie links**
- **Differential bar connecting both rockers**

When a wheel encounters an obstacle, the linkage redistributes the motion across the suspension so that the rover body remains relatively stable.

---

## 🌍 Advantages of Rocker–Bogie Suspension

- Maintains **continuous wheel contact** with terrain  
- Can climb obstacles up to **1.5× the wheel diameter**  
- Passive system (no springs or active suspension required)  
- Distributes loads efficiently across multiple wheels  
- Maintains rover chassis stability on slopes and rocks  

---

# 🪨 Rocker

The **Rocker** is a suspension arm that connects the rover wheels on one side to the chassis.

Each rocker pivots relative to the rover body and supports a set of wheels. When a wheel encounters an obstacle, the rocker rotates, allowing the wheels to adapt to terrain height differences.

This ensures that the rover maintains **traction and stability** during traversal.

---

## 🔧 Rocker Features

- Lightweight yet structurally strong design  
- Provides vertical articulation for wheel movement  
- Distributes terrain loads across wheels  
- Mounting points for wheels and differential bar  
- Optimized geometry for stiffness and durability  

---

## 🖼️ Rocker Render

<p align="center">
<img src="https://github.com/Team-Deimos-IIT-Mandi/Rocker-and-differential-bar/blob/main/NEW%20ROCKER%20BOGIE%202025/render%20photos/Screenshot%202025-12-25%20223915.png" width="650"/>
</p>

---

# ⚖️ Differential Bar

The **Differential Bar** connects the left and right rocker arms.

Its primary purpose is to **balance the rover body** when one side of the suspension moves over terrain.

When one rocker moves upward due to an obstacle, the differential mechanism transfers motion to the other side so that the rover body remains balanced.

This prevents excessive tilting of the rover.

---

## 🔧 Differential Bar Features

- Connects both rocker arms mechanically  
- Transfers angular motion between rockers  
- Helps maintain rover chassis balance  
- Improves traction on uneven terrain  
- Robust mechanical structure for durability  

---

## 🖼️ Differential Bar Render

<p align="center">
<img src="https://github.com/Team-Deimos-IIT-Mandi/Rocker-and-differential-bar/blob/main/DIFFERENTIAL%20BAR/RENDER%20PHOTOS/DIFFERENTIAL%20BAR%20RENDER.JPG" width="650"/>
</p>

---

# ⚙️ Hollow Differential Shaft Design

The differential bar is implemented as a **hollow shaft** instead of a solid shaft.

This design choice improves **weight efficiency and structural performance** while maintaining sufficient strength for rover suspension loads.

---

## 1️⃣ Weight Reduction

Planetary rovers require strict mass optimization.

A hollow shaft removes unnecessary material from the center where stresses are minimal. This significantly reduces weight while maintaining structural integrity.

Reducing suspension mass improves:

- Rover energy efficiency  
- Mobility over rough terrain  
- Overall payload capacity

---

## 2️⃣ Static Loading Condition

The differential bar primarily experiences **static loading conditions** caused by the rover’s weight and terrain interaction forces.

When the rover is stationary or moving slowly over uneven terrain, loads are transmitted through the suspension links to the differential bar.

Under static equilibrium:

```
ΣF = 0
ΣM = 0
```

Where:

- **ΣF** represents the sum of forces acting on the system  
- **ΣM** represents the sum of moments  

These equilibrium conditions ensure that the rover remains mechanically stable.

When one side of the rover encounters an obstacle, the rocker arm rotates and transfers load through the differential bar to the opposite side. This redistributes the load and helps maintain chassis stability.

---

### Structural Behavior Under Static Load

Under these conditions, the differential shaft mainly experiences:

- **Bending loads** from wheel-ground reaction forces  
- **Shear forces** at the rocker mounting interfaces  
- **Distributed loading** due to rover mass

Bending stress in the shaft can be expressed as:

```
σ = M y / I
```

Where:

- **σ** = bending stress  
- **M** = bending moment  
- **y** = distance from neutral axis  
- **I** = second moment of area  

Since bending stresses are highest near the **outer surface**, the hollow shaft design remains structurally efficient while minimizing mass.

---

# 🔗 Maintaining Rocker Parallelism

The differential bar runs through the rover chassis and connects both rocker arms.

This configuration ensures:

- Both rockers remain **parallel**
- Angular motion is **distributed symmetrically**
- The rover chassis experiences **minimal twisting**

Maintaining rocker alignment is essential for stable rover traversal across uneven terrain.

---

# 🛞 Role in Differential Drive Configuration

The rover uses a **differential drive system**, where the left and right wheels rotate at different speeds to steer the rover.

The suspension system must preserve proper geometry so that traction remains consistent.

The differential bar contributes by:

- Maintaining **balanced load distribution**
- Ensuring **equal wheel–ground contact**
- Preventing uneven traction during turning
- Supporting stable motion while climbing obstacles

This improves rover maneuverability and reliability on rough terrain.

---

# 📊 Finite Element Analysis (FEA)

To validate the structural integrity of the differential bar, a **static structural analysis** was conducted using **SolidWorks Simulation**.

The goal of the analysis was to evaluate:

- Stress distribution
- Structural stability
- Factor of Safety

---

## 🔧 Simulation Setup

The simulation used **static loading conditions** representing forces transferred from the rocker suspension system.

**Boundary Conditions**

- Ends of the shaft constrained at chassis interfaces  
- Loads applied at rocker connection points  
- Forces represent suspension load transfer from rover weight

---

## 📈 Factor of Safety Distribution

<p align="center">
<img src="https://github.com/user-attachments/assets/ab1402da-bffd-42eb-aeed-151d20074353" width="800"/>
</p>

The simulation result shows the **Factor of Safety distribution** along the differential bar.

Key observations:

- Minimum Factor of Safety is **greater than 30**
- Highest stresses appear near **mounting interfaces**
- Majority of the shaft experiences very low stress

---

## 📊 Interpretation

The simulation confirms that the differential bar design is **structurally safe under expected loading conditions**.

Important conclusions:

- The shaft safely withstands suspension loads
- Stress concentrations occur near boundary conditions
- The hollow shaft design provides sufficient stiffness while minimizing weight

This validates the differential bar as a reliable structural component of the rover suspension system.

---

# 📂 Repository Contents

```
CAD/
 ├── rocker/
 │   └── SolidWorks files for rocker subsystem
 │
 ├── differential_bar/
 │   └── SolidWorks files for differential bar
 │
images/
 └── rendered subsystem images

docs/
 └── design explanations and motion studies
```

---

# 🚀 Getting Started

Clone the repository:

```bash
git clone https://github.com/Team-Deimos-IIT-Mandi/Rocker-and-differential-bar.git
```

Open the CAD files using **SolidWorks** to explore the subsystem designs.

---

# 🧠 Design Tools Used

- **SolidWorks** — CAD modeling  
- **SolidWorks Simulation** — structural analysis  
- **Motion Study** — suspension articulation validation  

---

# 📊 Future Improvements

Possible improvements include:

- Suspension kinematics analysis  
- Advanced FEA stress optimization  
- Further weight reduction strategies  
- Dynamic rover terrain simulations  

---

# 🤝 Contributing

Contributions are welcome.

Potential contributions include:

- Improved suspension modeling
- Structural optimization
- Simulation studies
- Documentation improvements

---

# 📜 License

This project is intended for **educational and research purposes related to planetary rover development**.

---

# 🌌 Team

Developed as part of the **Mars Rover Project**

**Team Deimos — IIT Mandi**
