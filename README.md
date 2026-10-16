# Student Information Dictionary

**Veda Technology - AI & ML Internship | Level 1 - Task 7**

## Overview
A Python program that stores student records in a dictionary and supports **search**, **add** and **update** operations. Built to practice dictionaries and structured data representation.

## Tools Used
- Python
- Jupyter Notebook

## Approach
- Each student is stored as a nested dictionary: the **unique student ID** is the key, and the value holds `name`, `dept`, `year` and `cgpa`.
- Separate functions handle each operation:
  - `search_student(sid)` looks up a record using `.get()`, so a missing ID doesn't crash the program.
  - `add_student(sid, name, dept, year, cgpa)` adds a new record and blocks duplicate IDs.
  - `update_student(sid, **changes)` modifies any fields of an existing record.
- Student records are created manually (no external dataset).

## Example Output
```
Found 102: {'name': 'Priya', 'dept': 'CSE', 'year': 2, 'cgpa': 9.1}
Student ID 999 not found
Student Meena added with ID 104
ID 101 already exists. Use update_student instead.
Updated 103: {'name': 'Karthik', 'dept': 'ECE', 'year': 4, 'cgpa': 8.2}
ID 555 not found. Use add_student first.
```

## Outcome
The notebook demonstrates all three operations along with edge-case handling (missing IDs, duplicate IDs). It shows why dictionaries are a good fit for key-based lookup of structured data.

## How to Run
1. Clone this repository.
2. Open `student_dictionary_task7.ipynb` in Jupyter Notebook.
3. Run all cells (Kernel > Restart & Run All).

## Interview Questions
- **What is a dictionary in Python?** A mutable collection of key-value pairs with fast lookup by key.
- **Why are keys important?** They identify values; they must be unique and hashable.
- **Dictionary vs list?** A list is accessed by index position, a dictionary by key, which is faster and more meaningful for records.

## Author
J Sanjay - AI & Data Science student
