name:Bhukya Sravanthi
Company:Codtech IT solutions
id:CT08DS622
Domain:python programming
Duration:12/12/2024 to 12/01/2025

#code
def calculate_gpa(average):
    if average >= 90:
        return 4.0
    elif average >= 80:
        return 3.0
    elif average >= 70:
        return 2.0
    elif average >= 60:
        return 1.0
    else:
        return 0.0

def calculate_letter_grade(average):
    if average >= 90:
        return "A"
    elif average >= 80:
        return "B"
    elif average >= 70:
        return "C"
    elif average >= 60:
        return "D"
    else:
        return "F"

def track_grades():
    print("Welcome to the Student Grade Tracker!")
    grades = []
    num_subjects = int(input("Enter the number of subjects/assignments: "))
    for i in range(num_subjects):
        grade = float(input(f"Enter grade for subject/assignment {i+1}: "))
        grades.append(grade)
    average_grade = sum(grades) / len(grades)
    letter_grade = calculate_letter_grade(average_grade)
    gpa = calculate_gpa(average_grade)
    print("\n--- Grade Report ---")
    print(f"Grades: {grades}")
    print(f"Average Grade: {average_grade:.2f}")
    print(f"Letter Grade: {letter_grade}")
    print(f"GPA: {gpa:.2f}")
track_grades()
