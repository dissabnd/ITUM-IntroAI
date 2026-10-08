# Hands-On Lab 1: Predictive AI & Machine Learning in Google Colab



## Industrial Problem & Learning Objectives
In a polymer/chemical batch synthesis reactor, controlling product quality (viscosity and yield) is critical to avoiding expensive batch rejection. Process variables such as **Cooling Jacket Flow**, **Reactor Temperature**, **Agitator Motor Power**, and **Reaction Time** are candidate drivers of whether a batch passes or fails customer specifications — the lab finds out which ones actually matter.



## Dataset Description (`chemical_batch_process_data.csv`)

| Column | Type | Description | Role in ML |
| :--- | :--- | :--- | :--- |
| `Cooling_Flow_Lpm` | Continuous | Cooling jacket water flow (18.0 – 32.0 L/min) | Input Feature ($X_1$) |
| `Reactor_Temp_C` | Continuous | Peak batch reactor temperature (79.0 – 91.0 °C) | Input Feature ($X_2$) |
| `Agitator_Power_kW`| Continuous | Agitator motor electrical draw (13.5 – 18.5 kW) | Input Feature ($X_3$) |
| `Reaction_Time_min`| Continuous | Reaction cycle duration (50.0 – 75.0 min) | Input Feature ($X_4$) |
| `Product_Viscosity_cP`| Continuous | Final polymer dynamic viscosity | Physical metric |
| `Yield_Percent` | Continuous | Usable chemical yield % | Physical metric |
| **`Quality_Status`** | **Categorical** | **Lab quality verdict (`Pass` vs. `Fail`)** | **Target Label ($y$)** |


