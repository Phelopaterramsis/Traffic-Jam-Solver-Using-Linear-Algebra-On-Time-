# 🚦 Traffic Jam Solver Using Linear Algebra – “On Time!”

This folder contains my MATH 201 Linear Algebra project, where I applied Gaussian elimination and augmented matrices to model and solve urban traffic congestion. The project also includes a simple Python GUI prototype that recommends the least-traffic road using real-time flow inputs.

## 📌 Course

- Course: MATH 201 – Linear Algebra  
- University: University of Science and Technology in Zewail City  
- Instructor: Dr. Hatem Adel Fayed  
- TA: Mohamed Hemeda  
- Students: Phelopater Ramsis (202001171), Ereeny Adel (202001761)  

---

## 🧾 Project Overview

The project demonstrates how **linear algebra** can be used to solve one of Egypt’s biggest challenges: **traffic congestion**.  
By treating road intersections as nodes and car counts as variables, we can build a **system of linear equations** that represents car flow in and out of each road.

The work includes:

- Historical overview of Gaussian elimination  
- Explanation of augmented matrices and row reduction  
- Constructing flow-balance equations for intersections  
- Solving the system to obtain car counts for each road  
- Using the results to recommend the best road (least congested)  
- Developing a simple prototype application called **Traffixo**  

All math, screenshots, and results are shown across pages 3–9 of the report.  
:contentReference[oaicite:0]{index=0}

---

## 🧮 1. Linear Algebra Background

Pages 4–5 explain the tools used in the project:

- Coefficient matrices  
- Augmented matrices  
- Row operations (swap, scale, row addition)  
- Reduced echelon form  
- Free vs. pivot variables  
:contentReference[oaicite:1]{index=1}

These tools allow us to solve car-flow equations at each intersection.

---

## 🚗 2. How Linear Algebra Solves Traffic Jams

Each intersection is treated as a **node**.  
For every node:

> **Incoming cars = Outgoing cars**

This gives one linear equation per intersection.  
For example (from page 6), each arrow entering/leaving the node becomes a variable, and the node forms its own balance equation.  
:contentReference[oaicite:2]{index=2}

After constructing all equations, we build the **augmented matrix** (page 7) and perform row reduction.  
The final matrix has:

- **4 pivot columns**  
- **1 free variable**

Meaning the system has **infinitely many solutions**, and the traffic flow can be parameterized.

Using a chosen value for the free variable “t”, we can determine the car count for each road and **recommend the least congested route**.

---

## 🖥️ 3. Real-Life Implementation – Traffixo App

Pages 8–9 show screenshots of the prototype GUI built for the project:

### 🟦 Step 1 — Choose road layout  
Users select how streets are linked.

### 🟦 Step 2 — Enter flow rates  
Users assign incoming/outgoing car counts for each road segment.

### 🟦 Step 3 — Solve the system  
The software constructs the matrix, applies row reduction, and outputs the best road with the lowest flow.

Screenshots of the interface (Street X / Street Y / Street Z layout) appear on page 8.  
:contentReference[oaicite:3]{index=3}

---

## 👍 Advantages

- Eliminates the need for human intervention in data collection  
- Reduces time wasted in congestion  
- Can process large amounts of real-time data quickly  
- Helps drivers choose the optimal route  

## ⚠️ Limitations

- Designed only for **one-directional streets**  
- GUI only supports **limited layouts**  
- Real implementation would require sensors, radars, or Google Maps API  

(Page 9 lists these limitations.)  
:contentReference[oaicite:4]{index=4}

---

## 🧠 Conclusion

Traffic congestion is one of Egypt’s major challenges.  
This project shows that:

- Linear algebra can **model traffic flow**  
- Gaussian elimination can solve real urban problems  
- A simple Python tool can automate route recommendations  

As stated on page 10, the system can minimize congestion and reduce accident risks through automation.  
:contentReference[oaicite:5]{index=5}

---

## 🗂️ Files in This Folder

- `Linear Algebra Project.pdf` — full report with equations, screenshots, and explanations  
- `README.md` — this summary file  

