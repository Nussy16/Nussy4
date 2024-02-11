# Python program that keeps track of a student's grades in different subjects using dictionaries, and then calculates the average grade. I incorporate conditional statements to handle different scenarios, such as if a subject's grade is missing or if the user wants to add or remove grades.

def add_grade(subject, grade, grades_dict):
    grades_dict[subject] = grade

def remove_grade(subject, grades_dict):
    if subject in grades_dict:
        del grades_dict[subject]
        print(f"Grade for {subject} removed successfully.")
    else:
        print(f"Grade for {subject} not found.")

def calculate_average(grades_dict):
    total_grades = sum(grades_dict.values())
    average_grade = total_grades / len(grades_dict)
    return average_grade

def main():
    student_grades = {}

    while True:
        print("\n1. Add Grade")
        print("2. Remove Grade")
        print("3. Calculate Average Grade")
        print("4. Exit")

        choice = input("Enter your choice: ")

        if choice == '1':
            subject = input("Enter the subject: ")
            grade = float(input("Enter the grade: "))
            add_grade(subject, grade, student_grades)
        elif choice == '2':
            subject = input("Enter the subject to remove: ")
            remove_grade(subject, student_grades)
        elif choice == '3':
            if not student_grades:
                print("No grades available. Please add grades first.")
            else:
                average = calculate_average(student_grades)
                print(f"The average grade is: {average:.2f}")
        elif choice == '4':
            print("Exiting program.")
            break
        else:
            print("Invalid choice. Please try again.")

if __name__ == "__main__":
    main()

# This program allows the user to add, remove, and calculate the average of the student's grades in different . It uses dictionaries to store the grades for each subject and incorporates conditional statements to handle user input and different scenarios
