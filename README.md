# Python-Assignment---4-----Questions

Q1. Explain the key features of NumPy and highlight the major differences between NumPy arrays and Python lists with appropriate examples.  
A1. NumPy has various key features:  
    N-dimensional Array Object (ndarray): The core feature, allowing efficient storage and manipulation of large datasets in arrays of arbitrary dimensions.  
    Vectorized Operations: Enables element-wise operations on entire arrays without explicit Python loops, leading to significant performance gains.  
    Broadcasting: A mechanism that allows NumPy to perform operations on arrays of different shapes by automatically aligning their dimensions, eliminating the need for explicit reshaping.  
    Mathematical Functions: Provides a vast collection of high-level mathematical functions for linear algebra, Fourier transforms, random number generation, and more.  
    Memory Efficiency: Arrays store data in contiguous memory blocks, making them more memory-efficient than Python lists, especially for large datasets.  
    
NumPy arrays and python lists find their differences in Data Type Homogeneity, Performance and Memory Usage.  
Data Type Homogeneity: NumPy arrays require all elements to be homogenous in data types, i.e, it can only hold one form of data in an array. Python lists however can store elements of differet data types and are heterogenous.  
Performance: NumPy Arrays are significantly faster for numerical options but python lists are generally slower for numerical computations, especially on large dataset.  
Memory Usage: NumPy Arrays are more memory-efficient due to contiguous storage and fixed data types. Python lists store references to objects which can get scattered in memory, hence, it's less efficient.  

Q2. Develop a Python program using NumPy to create one-dimensional and two-dimensional arrays, and display their shape, dimensions, and data type.  
A2. 

    import numpy as np
    
    array_1d = np.array([1, 2, 3, 4, 5])
    
    print("One-Dimensional Array:")
    print("Array:", array_1d)
    print("Shape:", array_1d.shape)
    print("Dimensions (ndim):", array_1d.ndim)
    print("Data Type (dtype):", array_1d.dtype)
    print("-" * 30)
    
    array_2d = np.array([[10, 20, 30], [40, 50, 60], [70, 80, 90]])
    
    print("Two-Dimensional Array:")
    print("Array:\n", array_2d)
    print("Shape:", array_2d.shape)
    print("Dimensions (ndim):", array_2d.ndim)
    print("Data Type (dtype):", array_2d.dtype)
