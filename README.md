# HRMS: Hostel Room Management System

A menu-driven C program for keeping track of hostel students, their rooms and their fees.

Built as the final project for **CL1002 (Programming Fundamentals Lab)** at FAST-NUCES Karachi. Solo project by **Qasim Raza Syed** (26K-0828, BCS-1H).

## What it does

A warden runs the program, picks an option from the menu, and can:

- register students and stop duplicate roll numbers
- put a student in a room, with a capacity check so rooms never overflow
- look up or edit a student's details
- see which rooms are empty, available or full

Fee tracking, record deletion, reports and saving to a file are still being built (see the tracker below).

## Menu

```
===== Hostel Room Management System =====
1. Add Student
2. Allocate Room
3. Search Student
4. Update Student Record
5. Delete Student Record
6. View All Students
7. View Occupancy Status
8. Fee Tracking
9. Generate Report
0. Save and Exit
```

## Build tracker

I'm building this one feature at a time, following the course weeks.

| Week | What I'm adding | Status |
|------|-----------------|--------|
| 7 | Repo setup, feature list, design | Done |
| 8 | Main menu with switch-case | Done |
| 9 | Add student, view all students | Done |
| 10 | Room allocation, occupancy view | Done |
| 11 | Search and update student | Done |
| 12 | Delete record, fee tracking | Planned |
| 13 | Save and load data (file handling) | Planned |
| 14 | Reports: occupied rooms, fee defaulters | Planned |
| 15 | Move records into structs, testing | Planned |
| 16 | Final fixes and submission | Planned |

## C concepts

**In use now:** variables, `printf`/`scanf`, if/else, loops, switch-case, functions with return values, 1D and 2D arrays

**Coming as the course covers them:** string functions (name search), file handling (`fopen`, `fprintf`, `fscanf`), structures (`struct Student`, `struct Room`)

Right now student data is kept in parallel arrays. Once structures are covered in class, the records move into structs.

## Running it

You need GCC installed.

```
gcc src/main.c -o hrms.exe
./hrms.exe
```

On Windows PowerShell: `.\hrms.exe`

## Folder layout

```
src/      C source code
docs/     project documents
output/   screenshots of the program running
```

## Known limits

- 100 students and 30 rooms at most, 3 students per room
- Roll numbers have to be unique
- Names are one word for now (no spaces)
- Nothing is saved yet, so data disappears when the program exits

## Author

Qasim Raza Syed, 26K-0828, BCS-1H, FAST-NUCES Karachi