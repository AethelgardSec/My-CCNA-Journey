
## 🛠 Lab 1: Physical Connectivity Challenge
*Applying Day 2 concepts to a complex network topology.*
<img width="1612" height="657" alt="image" src="https://github.com/user-attachments/assets/c498f77a-0449-4575-a144-c2e72b8fec99" />

### **Lab Objectives & Constraints**
To demonstrate a deep understanding of physical layer requirements, I completed a connectivity lab with the following strict conditions:
1.  **Label Compliance:** Connect all devices exactly as labeled in the topology.
2.  **Manual Pinout Selection:** **Auto MDI-X is disabled**. I must manually choose between Straight-through and Crossover cables based on device roles.
3.  **Distance-Aware Media Selection:** Choose between Copper, Multimode Fiber, or Single-mode Fiber based on the distance between nodes.

### **Technical Analysis of My Implementation**

#### **1. Cable Type Selection (Auto MDI-X Disabled)**
Since Auto MDI-X is off, I applied the rule of "Same Layer = Crossover" and "Different Layer = Straight-through":
*   **Crossover Cables (Dashed Lines):** Used for **Router-to-Router** (R1-R2) and **Switch-to-Switch** (SW1-SW2, SW5-SW6, etc.) connections.
*   **Straight-through Cables (Solid Lines):** Used for **Router-to-Switch** (R2-SW1, R4-SW5) and **Switch-to-Host** (SW3-PC1, SW8-SRV1) connections.

#### **2. Media Selection based on Distance**
*   **R1 to R2 (50 meters):** Used **Copper (UTP)** as it is within the 100m limit and cost-effective.
*   **R3 to R4 (250 meters):** Exceeds the 100m limit for Copper. I used **Multimode Fiber (MMF)**, which is ideal for distances up to 550m.
*   **R1 to R3 (3 kilometers):** Significant distance. I used **Single-mode Fiber (SMF)**, as it is the only medium capable of maintaining signal integrity over several kilometers.

> **Note on Packet Tracer:** While the software doesn't visually distinguish between SMF and MMF, I have documented the logical choice here to reflect real-world engineering standards.
