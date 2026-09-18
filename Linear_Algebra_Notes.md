# Linear Algebra

## Column Space

The column space of a linear transformation is the range space or image. This is because any matrix multiplication with a vector can be represented as follows:


```math
Ax = \begin{bmatrix} a_{1,1} & a_{1,2} & a_{1,3} \\  a_{2,1} & a_{2,2} & a_{2,3}  \\  a_{3,1} & a_{3,2} & a_{3,3} \end{bmatrix} \begin{bmatrix} x_1 \\ x_2 \\ x_3 \end{bmatrix} = \begin{bmatrix} a_{1,1} \\  a_{2,1} \\  a_{3,1} \end{bmatrix} x_1 + \begin{bmatrix} a_{1,2} \\  a_{2,2} \\  a_{3,2} \end{bmatrix} x_2 + \begin{bmatrix} a_{1,3} \\  a_{2,3} \\  a_{3,3} \end{bmatrix} x_3
```

The above example shows that any linear transformation is just a linear combination of the column space.

To find the basis vector of the column space, and therefore the basis vector of the range space or the output of the linear transformation, we can simply take the matrix and get it in reduced row echelon form. Once in this form, find the pivot variables (leading zeros) and then find the columns in the ORIGINAL matrix A that correspond with these columns. The original matrix A columns are the basis vectors for the column space / range space. It should be noted that performing elementary row operations does NOT preserve the column space and therefore, we cannot use reduced row echelon form to find the column space. Elementary row operations do however preserve the row space. Therefore, you can use this process to find the row basis for the row space.
