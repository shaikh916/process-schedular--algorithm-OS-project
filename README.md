# Process Scheduling Simulator

## Overview
The Process Scheduling Simulator is a graphical application built using PyQt5 and Matplotlib. It allows users to simulate and visualize various CPU scheduling algorithms. The simulator provides an interface to input process details, select a scheduling algorithm, and view the resulting Gantt chart and performance metrics.

## Features
- **Graphical User Interface**: Built with PyQt5, providing an interactive and user-friendly experience.
- **Multiple Scheduling Algorithms**: Includes:
  - First-Come, First-Serve (FCFS)
  - Priority (preemptive and non-preemptive)
  - Shortest Job First (SJF)
  - Longest Job First (LJF)
  - Highest Response Ratio Next (HRRN)
  - Longest Remaining Time First (LRTF)
  - Shortest Remaining Time First (SRTF)
- **Visualization**: Uses Matplotlib to generate Gantt charts, visualizing the process execution over time.
- **Performance Metrics**: Calculates and displays turnaround time, waiting time, and completion time for each process, along with average turnaround and waiting times.

## Project Structure
- **`Scheduler` Class**: Base class for scheduling algorithms. Implements common methods like `visualize`, `create_plot`, and `finish_plot`.
- **Algorithm Classes**: Derived classes (`FCFS`, `Priority`, `Priority_pre`, `SJF`, `LJF`, `HRRN`, `LRTF`, `SRTF`) implement the `run` method specific to each scheduling algorithm.
- **`App` Class**: Main application class, handles the user interface and interactions.

## Requirements
- Python 3.x
- PyQt5
- Matplotlib
- NumPy

## Installation
1. Install Python 3.x.
2. Install the required libraries:
   ```bash
   pip install PyQt5 matplotlib numpy
   ```

## Usage
1. Run the application:
   ```bash
   python main.py
   ```
2. Use the interface to add processes, select an algorithm, and run the simulation.

## Example Usage
1. **Add Processes**: Click "Add Process" to add rows for each process. Enter the arrival time and burst time (and priority if applicable).
2. **Select Algorithm**: Choose a scheduling algorithm from the dropdown menu.
3. **Run Simulation**: Click "Run" to execute the selected algorithm and visualize the results.
4. **View Results**: The Gantt chart will be displayed, and the results table will show the performance metrics for each process.

## Troubleshooting
- **Empty Fields**: Ensure all fields are filled before running the simulation.
- **Invalid Input**: Verify that all input values are valid numbers. Arrival time and burst time must be non-negative, and priority must be greater than zero for priority scheduling.

## License
This project is licensed under the MIT License.

## Team
- Ahmed Sherif Sayed 211001287
- Mohamed Abdelfattah Abozied 211001956
- Youssef Sharaf 211001323
- Mohamed Farag Arnous 211001654
- Ahmed Moussa 211001639

  
**For any questions or feedback, please contact the project maintainer at [a.sherif2187@nu.edu.eg].**

---
