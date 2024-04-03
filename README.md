# Process Scheduler Simulator

This program simulates a process scheduler using different scheduling algorithms: FCFS (First Come, First Served), SRTF (Shortest Remaining Time First), and RR (Round Robin).

## Usage

### Compilation

Compile the program using `gcc`:

gcc -o simulator simulator.c -lm


### Execution

Run the program with the following command-line arguments:

./simulator <algorithm> <lambda> <mu> <quantum> <max_processes>


- `<algorithm>`: Choose the scheduling algorithm.
    - `0`: FCFS (First Come, First Served)
    - `1`: SRTF (Shortest Remaining Time First)
    - `2`: RR (Round Robin)

- `<lambda>`: Average arrival rate (in processes/second).

- `<mu>`: Average service time (in seconds).

- `<quantum>`: Quantum interval for Round Robin algorithm.

- `<max_processes>`: Maximum number of processes to complete before stopping the simulation.

Example:

./simulator 1 0.5 0.8 2 2000


This command will run the simulator with the SRTF algorithm, an arrival rate of 0.5 processes per second, a service time of 0.8 seconds, a quantum of 2 for Round Robin, and it will stop after 2000 processes have been completed.

## Files

- `simulator1.c`: Source code of the simulator.
- `README.md`: This file.
```bash
First you go to terminal
cd downloads (where the code is available on the computer)
then scp simulator.c username@zeus.cs.txstate.edu:~/
then it should show up as downloaded on zeus

to run it on terminal you must apply the steps above to see the process event running

cd downloads
downloads % gcc simulator1.c -o simulator1 -lm
then you can put your choosing of the .simulator1.c
gcc -o simulator1 simulator1.c -lm
