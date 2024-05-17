# Assignment 2

#dot method

#Example 1
import numpy as np

A = np.array([[1, 2], [3, 4]])
B = np.array([[5, 6], [7, 8]])

# Matrix multiplication
C = np.dot(A, B )

print(C)

#Example 2
import numpy as np

x = np.array([1, 2, 3])
y = np.array([4, 5, 6])

# Dot product
dot_product = np.dot(x, y)

print(dot_product)

#Example 3
import numpy as np

A = np.array([[1, 2, 3], [4, 5, 6]])
v = np.array([1, 0, 1])

# Matrix-vector multiplication
result = np.dot(A, v)

print(result)

#transpose method
import numpy as np

# Example 1
G = np.array([[11, 21, 23], [41,25, 16]])
result4 = G.transpose()
print("Transpose 1:\n", result4)

# Example 2
H = np.array([[17, 12], [13, 24], [25, 16]])
result5 = np.transpose(H)
print("Transpose 2:\n", result5)

# Example 3
I = np.array([[[12, 22], [31, 14]], [[15, 26], [37, 16]]])
result6 = np.transpose(I, (1, 0, 2))
print("Transpose 3:\n", result6)

# flatten method

# Example 1
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6]])

result = arr.flatten()
print(f'EXAMPLE A:{result}')

# Example 2
import numpy as np

arr = np.array([[[1, 2], [3, 4]], [[5, 6], [7, 8]]])

result = arr.flatten()
print(f'EXAMPLE B:{result}')

# Example 3
import numpy as np

A = np.array([[1, 2], [3, 4]])
B = np.array([[5, 6], [7, 8]])

C = np.dot(A, B)

result= C.flatten()
print(f'EXAMPLE C:{result}')

#linalg.det method

#Example 1
#Calculate determinant of a 2x2 matrix:
import numpy as np

# Define a 2x2 matrix
matrix_2x2 = np.array([[1, 3],
                       [5, 7]])

# Calculate determinant
det_2x2 = np.linalg.det(matrix_2x2)

print("Determinant of 2x2 matrix:")
print(det_2x2)

#Example 2
#Calculate determinant of a 3x3 matrix:
import numpy as np

# Define a 3x3 matrix
matrix_3x3 = np.array([[2, 4, 6],
                       [8, 10, 12],
                       [16, 18, 20]])

# Calculate determinant
det_3x3 = np.linalg.det(matrix_3x3)

print("Determinant of 3x3 matrix:")
print(det_3x3)

#Example 3
#Calculate determinant of a randomly generated square matrix:
import numpy as np

# Generate a random 4x4 matrix
matrix_4x4 = np.random.rand(4, 4)

# Calculate determinant
det_4x4 = np.linalg.det(matrix_4x4)

print("Determinant of randomly generated 4x4 matrix:")
print(det_4x4)

#linalg.inv method

#Example 1
import numpy as np

A = np.array([[1, 2], [3, 4]])

# Finding the inverse of matrix A
A_inv = np.linalg.inv(A)

print(A_inv)

#Example 2
import numpy as np

A = np.array([[1, 2], [3, 4]])
b = np.array([5, 6])

# Finding the inverse of matrix A
A_inv = np.linalg.inv(A)

# Solving for x
x = np.dot(A_inv, b)

print(x)

#Example 3
import numpy as np

A = np.array([[1, 2], [3, 4]])

# Finding the inverse of matrix A
A_inv = np.linalg.inv(A)

# Multiplying A by its inverse
I = np.dot(A, A_inv)

print(I)
