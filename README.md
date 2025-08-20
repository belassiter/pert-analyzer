# PERT Network Analyzer

A web-based tool to forecast project completion time using the Program Evaluation and Review Technique (PERT). This application helps project managers and teams to estimate the time required to complete a project by analyzing a network of tasks with 3-point estimates.

## Introduction

The PERT Network Analyzer is a single-page application that allows users to define tasks, their dependencies, and provide optimistic (a), most likely (m), and pessimistic (b) time estimates. It then uses Monte Carlo simulation to generate a probability distribution for the project's completion time and total effort.

## Features

- **Task Management:** Add, remove, and manage project tasks.
- **Dependency Mapping:** Define dependencies between tasks to create a project network.
- **3-Point Estimation:** Use optimistic, most likely, and pessimistic estimates for more accurate forecasting.
- **Monte Carlo Simulation:** Runs thousands of simulations to generate a probability distribution of project outcomes.
- **Network Diagram:** Visualizes the project network, highlighting the critical path.
- **Probability Analysis:** Provides detailed statistics (mean, median, confidence levels) and probability charts for both project duration and total effort.
- **CSV Import/Export:** Import task lists from a CSV file and export the current tasks to a CSV file.
- **Time-Scaled Diagram:** The network diagram is time-scaled, meaning the horizontal position of each task represents its earliest start time.
- **Effort Analysis:** Calculates the total quantity of work (effort) required, which is useful for budgeting and resource planning.

## How to Use

1.  **Open `pertforecast.html` in your web browser.**
2.  **Add Tasks:** Click the "Add Task" button to create a new task row.
3.  **Define Dependencies:** For each task, enter the letters of the tasks that must be completed before it can start (e.g., A,B).
4.  **Provide Estimates:** Enter the Optimistic (a), Most Likely (m), and Pessimistic (b) time estimates for each task.
5.  **Run Analysis:** Click the "Estimate" button to run the Monte Carlo simulation.
6.  **Analyze Results:**
    *   Review the **Network Diagram** to see the critical path (in red).
    *   Examine the **Project Summary** for key statistics on project duration.
    *   Use the **Probability Distribution** chart to understand the likelihood of different completion times.
    *   Analyze the **Total Quantity of Work** section for effort-related insights.
7.  **(Optional) Import/Export:**
    *   Use the "Import CSV" button to load tasks from a `.csv` file.
    *   Use the "Export CSV" button to save the current task list.
    *   Use the "Download CSV Template" to get a sample CSV file.

## Technical Details

- **Frontend:** The application is built with HTML, [Tailwind CSS](https://tailwindcss.com/) for styling, and [D3.js](https://d3js.org/) for data visualization.
- **Methodology:**
    - **PERT (Program Evaluation and Review Technique):** The core methodology for estimating task durations using a weighted average.
    - **Monte Carlo Simulation:** Used to model the uncertainty in task durations and generate a probability distribution for the project timeline and total effort.
    - **Critical Path Method (CPM):** Used to identify the sequence of tasks that determines the total project duration.

## License

This project is not currently licensed. All rights reserved.
