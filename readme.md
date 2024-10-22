def add_student(name,grade):
    student_grades[name] = grade
    print(f"Added {name} with marks {grade} successsfully")

# Updating Students
def update_students(name,grade):
    if name in student_grades:
        student_grades[name] = grade
        print(f"{name} with marks {grade} are updated")
    else:
        print("Name not Found")

def delete_students(name,grade):
    if name in student_grades:
        student_grades.pop(name)
        print(f"Delete The {name} with marks {grade}")
    else:
        print("Name not Found")
def display_all_students():
    if student_grades:
        for name,grade in student_grades.items():
            print(f'{name}:{grade}')
    else:
        print("No students found/added")

