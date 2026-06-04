# README - FCFS CPU Scheduling

## Overview

This C program implements the **First Come First Serve (FCFS)** CPU Scheduling Algorithm. It calculates and displays:

* Burst Time (BT)
* Waiting Time (WT)
* Turnaround Time (TAT)
* Average Waiting Time
* Average Turnaround Time

Processes are executed in the same order they are entered by the user.

---

## Features

* Accepts multiple processes.
* Calculates waiting time for each process.
* Calculates turnaround time for each process.
* Displays average waiting time and turnaround time.
* Simple and easy-to-understand implementation.

---

## Algorithm

1. Read the number of processes.

2. Input burst time for each process.

3. Set waiting time of the first process to 0.

4. Calculate waiting time for remaining processes.

5. Calculate turnaround time using:

   WT + BT = TAT

6. Display process details and averages.

---

## Compilation

Use a C compiler such as GCC:

```bash
gcc fcfs.c -o fcfs
```

---

## Execution

Run the program:

```bash
./fcfs
```

---

## Sample Input

```text
Enter number of processes: 3
Enter Burst Time for Process P1: 5
Enter Burst Time for Process P2: 3
Enter Burst Time for Process P3: 8
```

## Sample Output

```text
Process  Burst Time  Waiting Time  Turnaround Time
P1       5           0             5
P2       3           5             8
P3       8           8             16

Average Waiting Time = 4.33
Average Turnaround Time = 9.67
```

---

## Formulae Used

**Waiting Time (WT)**

```text
WT[i] = WT[i-1] + BT[i-1]
```

**Turnaround Time (TAT)**

```text
TAT[i] = WT[i] + BT[i]
```

**Average Waiting Time**

```text
Sum of WT / Number of Processes
```

**Average Turnaround Time**

```text
Sum of TAT / Number of Processes
```

---

## Karan Prajapati

FCFS CPU Scheduling Program implemented in C for Operating Systems laboratory and learning purposes.
