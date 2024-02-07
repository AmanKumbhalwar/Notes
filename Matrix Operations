# C++ Code with Notes for Matrix Operations

This markdown file contains C++ code to initialize a matrix, access and display its diagonal elements, lower triangular elements, and upper triangular elements, with zeros for all other elements.

```cpp
#include <iostream>
#include <vector>

// Function to access the diagonal element
int diagonal(const std::vector<int>& A, int i) {
    return A[i - 1];
}

// Function to access the lower triangular element
int lowerTriangular(const std::vector<int>& A, int i, int j) {
    if (j <= i) {
        return A[(i * (i - 1) / 2) + (j - 1)];
    }
    return 0;
}

// Function to access the upper triangular element
int upperTriangular(const std::vector<int>& A, int i, int j) {
    if (j >= i) {
        return A[(i - 1) * i / 2 + (j - 1)];
    }
    return 0;
}

int main() {
    // Define the matrix size
    int n = 4;

    // Define a sample matrix
    std::vector<int> matrix(n * n);
    for (int i = 0; i < n * n; ++i) {
        matrix[i] = i + 1;
    }

    // Display the original matrix with zeros for non-diagonal elements
    std::cout << "Original Matrix with Zeros:" << std::endl;
    for (int i = 1; i <= n; ++i) {
        for (int j = 1; j <= n; ++j) {
            if (i == j) {
                std::cout << diagonal(matrix, i) << " ";
            } else {
                std::cout << "0 ";
            }
        }
        std::cout << std::endl;
    }
    std::cout << std::endl;

    // Display the diagonal elements
    std::cout << "Diagonal Elements:" << std::endl;
    for (int i = 1; i <= n; ++i) {
        std::cout << diagonal(matrix, i) << " ";
    }
    std::cout << std::endl << std::endl;

    // Display the lower triangular matrix with zeros for non-lower triangular elements
    std::cout << "Lower Triangular Matrix with Zeros:" << std::endl;
    for (int i = 1; i <= n; ++i) {
        for (int j = 1; j <= n; ++j) {
            std::cout << lowerTriangular(matrix, i, j) << " ";
        }
        std::cout << std::endl;
    }
    std::cout << std::endl;

    // Display the upper triangular matrix with zeros for non-upper triangular elements
    std::cout << "Upper Triangular Matrix with Zeros:" << std::endl;
    for (int i = 1; i <= n; ++i) {
        for (int j = 1; j <= n; ++j) {
            std::cout << upperTriangular(matrix, i, j) << " ";
        }
        std::cout << std::endl;
    }

    return 0;
}
