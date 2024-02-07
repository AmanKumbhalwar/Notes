# Matrix Indexing Expressions

## 1. Diagonal
- Expression: `A[i-1]`

## 2. Lower Triangular
### a) Row-major
- Expression: `A[(i*(i-1)/2) + (j-1)]`

### b) Column-major
- Expression: `A[(j-1)*j/2 + (i-1)]`

## 3. Upper Triangular
### a) Row-major
- Expression: `A[(i-1)*i/2 + (j-1)]`

### b) Column-major
- Expression: `A[j*(j-1)/2 + (i-1)]`
