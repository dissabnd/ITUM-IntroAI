# Hands-On Lab 3: Plant Diagnostics with a Copilot Agent



## Industrial Problem & Learning Objectives
It is 14:30 on a polymer compounding line. Twin-screw extruder **EX-204** (PP + 20% CaCO₃) has six active alarms: melt pressure, motor torque and die temperature are all high. You will build a **Copilot agent** that reads the plant data and the equipment manual, finds the most likely fault, traces it back to a root cause the plant can fix, and recommends safe operator actions. Then you test whether the agent holds its diagnosis when someone insists on a different cause.



## Files

| File | Description | Use in agent |
| :--- | :--- | :--- |
| `instructions.md` | The agent's role and rules | Instructions |
| `Equipment_Troubleshooting_Manual_EX204.pdf` | SOP: operating limits, alarm limits, fault matrix and operator actions | Knowledge |
| `plant_sensor_telemetry.csv` | 30 minutes of 1-minute SCADA data (14:00 – 14:30) | Knowledge |
| `alarm_events_log.txt` | Alarm and event log for the same 30 minutes | Knowledge |
| `prompts.md` | Prompt 1 diagnoses the upset; Prompt 2 tries to break the agent | Chat |



## Dataset Description (`plant_sensor_telemetry.csv`)

| Column | Description |
| :--- | :--- |
| `Timestamp`, `Time_Elapsed_min` | Time of each 1-minute sample |
| `Screw_Speed_RPM` | Extruder screw speed |
| `Motor_Torque_Percent` | Main drive motor torque (% of rated) |
| `Melt_Pressure_bar` | Melt pressure at the screen inlet |
| `Melt_Temp_Die_C` | Melt temperature at the die |
| `Bearing_Vibration_mm_s` | Drive bearing vibration |
| `Bearing_Temp_C` | Motor bearing temperature |
