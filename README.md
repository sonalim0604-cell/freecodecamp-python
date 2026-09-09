# freecodecamp-python 
sonali
rows = int(input("Enter number of rows: "))
columns = int(input("Enter number of columns: "))

matrix = []

for i in range(rows):
    row = []
    for j in range(columns):
        value = int(input(f"Enter element [{i}][{j}]: "))
        row.append(value)
    matrix.append(row)

print("Matrix:")

for row in matrix:
    print(row)

sum_diagonal = 0

for i in range(rows):
    sum_diagonal += matrix[i][i]
    sum_diagonal += matrix[i][columns - 1 - i]

print("Addition of diagonal elements:", sum_diagonal)
        
    





