<img width="1512" height="982" alt="Στιγμιότυπο οθόνης 2026-05-05, 5 19 31 μμ" src="https://github.com/user-attachments/assets/a99970ec-8a2f-4917-93fe-4d2a12deae7a" /># 🎓 Student, Teacher & Lesson Management System

A command-line **CRUD application** built in Python for managing an educational organization. This was my first complete Python project, focusing on Object-Oriented Programming and data persistence.

---

## 📸 Preview

```
===============
     MENU
1 - Create Pupil
2 - Print pupils
3 - Update Pupil
4 - Delete Pupil
5 - Create teacher
6 - Print teacher
7 - Update teacher
8 - Delete teacher
9 - Create lesson
10 - Subscribe to lesson
11 - Print Lessons
12 - Update Lesson
13 - Delete lesson
14 - Exit
```
![Main Menu]<img width="1512" height="982" alt="Στιγμιότυπο οθόνης 2026-05-05, 5 18 21 μμ" src="https://github.com/user-attachments/assets/1c8f2ae7-ab7f-413e-8213-65415279ce6d" />

|--------------------------------------------------------------------------------------------------------------------------|
![A]<img width="1512" height="982" alt="Στιγμιότυπο οθόνης 2026-05-05, 5 19 49 μμ" src="https://github.com/user-attachments/assets/76522891-3b70-48c4-bd28-f4489f665789" />

|--------------------------------------------------------------------------------------------------------------------------|
![B]<img width="1512" height="982" alt="Στιγμιότυπο οθόνης 2026-05-05, 5 19 31 μμ" src="https://github.com/user-attachments/assets/cc78eb66-bf02-49f6-8744-6cc1e1afc28b" />

|--------------------------------------------------------------------------------------------------------------------------|
![C]<img width="1512" height="982" alt="Στιγμιότυπο οθόνης 2026-05-05, 5 18 49 μμ" src="https://github.com/user-attachments/assets/92231610-0f4e-43d1-a3b3-e11f2bcdf5ac" />






---

## ✨ Features

**Pupils (Μαθητές)**
- Create a new pupil with name, surname, father's name, age, class and ID card
- Duplicate detection before adding
- Search by ID or surname
- Update any field (name, age, class, etc.)
- Delete by ID or surname
- View all pupils, one pupil, or names-only list

**Teachers (Καθηγητές)**
- Create, read, update and delete teachers
- Search by teacher ID

**Lessons (Μαθήματα)**
- Create new lessons
- Subscribe a pupil to a lesson
- View all lessons with enrolled pupils
- Update (remove a pupil from a lesson)
- Delete a lesson

**Data Persistence**
- All data is automatically saved to JSON files after every action
- Data is loaded on startup — nothing is lost between sessions

---

## 🏗️ Project Structure

```
main_data_project/
│
├── main.py          # Entry point — menu logic and app flow
│
├── pupil.py         # Pupil model (data class)
├── pupils.py        # Pupils controller (CRUD operations)
│
├── teacher.py       # Teacher model
├── teachers.py      # Teachers controller
│
├── lesson.py        # Lesson model
├── lessons.py       # Lessons controller
│
├── for_pupils.json   # JSON "database" for pupils
├── for_teachers.json # JSON "database" for teachers
└── for_lessons.json  # JSON "database" for lessons
```

---

## ⚙️ How to Run

```bash
# Clone the repository
git clone https://github.com/kwstassrp6991/python.git

# Navigate to the project folder
cd python/main_data_project

# Run the app
python main.py
```

> Requires Python 3.x — no external libraries needed.

---

## 🧠 What I Learned

| Concept | How I used it |
|---|---|
| **OOP** | Separate model and controller classes for each entity |
| **Encapsulation** | Each class manages its own data and logic |
| **JSON serialization** | Converting class objects to/from dicts for file storage |
| **File I/O** | Reading and writing persistent data with `json.load` / `json.dump` |
| **Iterators** | `__iter__`, `__getitem__`, `__str__` on collection classes |
| **Input validation** | Checking for duplicates, digit-only inputs, invalid values |
| **CLI menus** | Building an interactive loop-based menu system |

---

## 🛠️ Technologies

- **Python 3.x**
- **JSON** — for data storage (no database required)
- **OOP** — classes, methods, encapsulation

---

## 🚀 Future Improvements

- [ ] Add a proper database (SQLite)
- [ ] Add a Flask REST API layer
- [ ] Input validation with error handling throughout
- [ ] Unit tests with `pytest`
