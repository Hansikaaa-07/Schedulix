
# Schedulix — CPU Scheduling & Kernel Architecture Explorer

An interactive **Operating Systems learning simulator** designed to visualize CPU scheduling algorithms and explore different kernel architectures through a simple, intuitive interface.

Schedulix combines process scheduling, performance analysis, visual execution timelines, and kernel architecture concepts into one self-contained web application.

---

## Overview

Understanding operating system concepts becomes easier when they can be visualized. Schedulix allows users to create processes, simulate scheduling algorithms, observe CPU execution through Gantt charts, analyze performance metrics, and explore how different kernel architectures work.

## Features

### CPU Scheduling Simulator
- Add and manage processes with Process ID, Arrival Time, and Burst Time.
- Simulate **FCFS (First Come First Serve)** scheduling.
- Simulate **SJF (Shortest Job First)** scheduling.
- Simulate **Round Robin (RR)** scheduling with configurable Time Quantum.
- Visualize process execution using a Gantt chart.
- Observe execution order and process completion.

### Performance Analysis
- Completion Time (CT)
- Turnaround Time (TAT)
- Waiting Time (WT)
- Average Turnaround Time
- Average Waiting Time
- CPU Utilization
- Throughput
- Context Switches

### Algorithm Comparison
Compare scheduling algorithms using the same set of processes and understand how different algorithms affect waiting time, turnaround time, and CPU performance.

### Kernel Architecture Explorer

Explore the three major kernel architecture approaches:

| Architecture | Description | Example OS |
|---|---|---|
| Monolithic Kernel | Major OS services operate within kernel space. | Linux, UNIX |
| Microkernel | Only essential functions remain in the kernel; other services operate in user space. | MINIX 3, QNX |
| Layered Architecture | OS functionality is organized into hierarchical layers. | THE Operating System |

Learn their structure, important features, advantages, disadvantages, and examples.

---

## Scheduling Algorithms

### 1. First Come First Serve (FCFS)
Processes are executed in the order in which they arrive. FCFS is simple and non-preemptive, but it can cause long waiting times for shorter processes.

### 2. Shortest Job First (SJF)
The process with the shortest burst time among the available processes is selected first. It can reduce average waiting time but may cause starvation for longer processes.

### 3. Round Robin (RR)
Each process is given a fixed time quantum. If a process is not completed within its time quantum, it is placed back into the ready queue. Round Robin provides fair CPU allocation and is commonly associated with time-sharing systems.

---

## Performance Metrics

| Metric | Formula |
|---|---|
| Turnaround Time | TAT = CT − AT |
| Waiting Time | WT = TAT − BT |
| Response Time | RT = First Execution Time − AT |
| Average Waiting Time | Sum of WT / Number of Processes |
| Average Turnaround Time | Sum of TAT / Number of Processes |
| CPU Utilization | (Busy Time / Total Time) × 100 |
| Throughput | Completed Processes / Total Time |

**Abbreviations:**

- CT – Completion Time
- AT – Arrival Time
- BT – Burst Time
- TAT – Turnaround Time
- WT – Waiting Time
- RT – Response Time

---

## Kernel Architectures

### Monolithic Kernel
All major operating system services, such as process management, memory management, file systems, and device drivers, operate within kernel space.

**Features**
- High performance
- Direct communication between kernel components
- Large kernel structure
- Less fault isolation

**Examples:** Linux, traditional UNIX

### Microkernel
Only essential functions are maintained in the kernel, while additional services operate in user space.

**Features**
- Modular design
- Improved fault isolation
- Better reliability
- Easier service maintenance
- Communication through message passing (IPC)

**Examples:** MINIX 3, QNX

### Layered Architecture
The operating system is divided into layers, with each layer interacting with the layers around or below it.

**Features**
- Organized structure
- Easier debugging
- Simplified maintenance
- Clear separation of responsibilities

**Example:** THE Operating System (Dijkstra's layered system)

---

## Technology Stack

- **HTML5** – Application structure
- **CSS3** – Styling, layout, responsive interface
- **JavaScript** – Scheduling logic, process management, simulation, calculations, and interaction

No external libraries, frameworks, APIs, or CDN dependencies are required.

---

## How to Run

### Run Locally

1. Download or clone this repository.
2. Open the project folder.
3. Open `index.html` in any modern browser.
4. Start adding processes and running simulations.

The application works offline.

### Run on GitHub Pages

1. Upload the project files to a GitHub repository.
2. Rename the main HTML file to `index.html`, if required.
3. Open the repository **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)` folder.
6. Click **Save**.
7. Wait for deployment and open the generated GitHub Pages URL.

---

## Project Structure

```text
Schedulix/
│
├── index.html       # Complete simulator and learning interface
└── README.md        # Project documentation
```

The project is self-contained. HTML, CSS, and JavaScript are integrated into a single file for easy execution and portability.

---

## Learning Objectives

- Understand CPU scheduling and process execution.
- Compare different CPU scheduling algorithms.
- Interpret Gantt charts and scheduling timelines.
- Calculate completion, waiting, and turnaround times.
- Analyze CPU utilization and throughput.
- Understand monolithic, microkernel, and layered kernel architectures.
- Relate theoretical Operating Systems concepts to interactive simulations.

---

## Project Scope

Schedulix is an educational simulator intended to help students visualize operating system concepts and understand how scheduling algorithms and kernel architectures work.

It is designed for learning and demonstration purposes and does not represent the actual internal scheduling mechanisms of a running operating system.

---

## Author

**Hansika Keerthi**  
Information Technology  
Vasavi College of Engineering

---

⭐ *Learn. Simulate. Explore.*
