
def calculate_average(marks):
    return sum(marks) / 
def get_grade(avg):
    if avg >= 90:
        return "A"
    elif avg >= 80:
        return "B"
    elif avg >= 70:
        return "C"
    elif avg >= 60:
        return "D"
    else:
        return "F"


marks = []

for i in range(5):
    mark = float(input("Enter mark: "))

    while mark < 0 or mark > 100:
        print("Invalid mark! Enter between 0 and 100.")
        mark = float(input("Enter mark: "))

    marks.append(mark)

average = calculate_average(marks)
grade = get_grade(average)

print("Average Marks =", average)
print("Grade =", grade)# Mark-grade-calculation-