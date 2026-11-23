# CSA03 – Data Structures Assignment 4
**CO4: Designing Fast Storage and Ordering of Data**  
Complete C11 reference solution and evidence repository.

## Repository structure
- `Task01_Hashing/` – weak-hash diagnosis and 100,000-key distribution benchmark.
- `Task02_Collision_Strategies/` – linear-probing trace and completed separate-chaining program.
- `Task03_Heaps_Priority_Queues/` – min-heap build trace and stable max-priority triage heap.
- `Task04_Sorting_Forensics/` – Lomuto partition trace, 10,000-item quicksort forensics, and stable merge-sort repair.
- `Task05_Sorting_Parallel/` – completed stable merge, six-algorithm benchmark harness, parallel OpenMP merge sort.
- `Task06_Food_Delivery_Challenge/` – integrated hash-table + indexed-heap simulation.
- `report/` – full assignment answers and complexity analysis in Markdown and Word (`.docx`).
- `evidence/` – captured program outputs and benchmark results.

## Main report
- [Complete answers (Word)](report/CSA03_Assignment4_Complete_Answers.docx)
- [Complete answers (Markdown)](report/Assignment4_Complete_Answers.md)

## Student details (fill before submission)
- Name: Vimal R
- Register Number: [ENTER REGISTER NUMBER]
- Course: Data Structures (CSA03)
- Compiler: GCC [record installed version]
- Compile flags: `-std=c11 -Wall -Wextra -O2`

## Build and run (Windows PowerShell)
Compile an individual file from its folder:
```powershell
gcc -std=c11 -Wall -Wextra -O2 hash_benchmark.c -o hash_benchmark.exe
.\hash_benchmark.exe
```
For the sanitizer task (GCC build must support AddressSanitizer):
```powershell
gcc -std=c11 -Wall -Wextra -g -fsanitize=address chaining_complete.c -o chaining_complete.exe
.\chaining_complete.exe
```
For OpenMP parallel merge sort:
```powershell
gcc -std=c11 -Wall -Wextra -O2 -fopenmp parallel_merge_sort.c -o parallel_merge_sort.exe
.\parallel_merge_sort.exe 10000000 4
```
For food delivery simulation:
```powershell
gcc -std=c11 -Wall -Wextra -O2 food_delivery_simulation.c -o food_delivery_simulation.exe
.\food_delivery_simulation.exe 50000
.\food_delivery_simulation.exe 100000
```

## Important academic integrity / execution note
The assignment explicitly requires each student to execute every program, predict output before execution, measure on their own machine, and commit progressively. This repository supplies complete reference implementations and analytical answers. Replace the student details, run the programs on the actual lab machine, save genuine screenshots and timings, and make task-wise commits. Do not claim supplied benchmark figures are measurements from your own computer.

## Suggested GitHub repository name
`CSA03-<RegisterNumber>-Assignment4`
