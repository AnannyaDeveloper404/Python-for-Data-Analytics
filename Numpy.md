1. **What is a vector?**  
   A vector is a list of numbers representing a quantity with both magnitude and direction.

2. **How do you represent vectors using a Python list? Give an example.**  
   A vector can be represented using a list of numbers:

   ```python
   vector = [1, 2, 3]
   ```

3. **What is a dot product of two vectors?**  
   The dot product is the sum of the products of corresponding elements in two vectors.

4. **Write a function to compute the dot product of two vectors.**

   ```python
   def dot_product(vec1, vec2):
       return sum(x * y for x, y in zip(vec1, vec2))
   ```

5. **What is Numpy?**  
   Numpy is a Python library for numerical computing, providing support for arrays and mathematical operations.

6. **How do you install Numpy?**  
   Run the command:

   ```bash
   pip install numpy
   ```

7. **How do you import the numpy module?**

   ```python
   import numpy as np
   ```

8. **What does it mean to import a module with an alias? Give an example.**  
   It allows you to use a shorter name for the module. Example:

   ```python
   import numpy as np
   ```

9. **What is the commonly used alias for numpy?**  
   `np`

10. **What is a Numpy array?**  
    A Numpy array is a grid of values, all of the same type, indexed by a tuple of non-negative integers.

11. **How do you create a Numpy array? Give an example.**

    ```python
    arr = np.array([1, 2, 3])
    ```

12. **What is the type of Numpy arrays?**  
    `<class 'numpy.ndarray'>`

13. **How do you access the elements of a Numpy array?**  
    Using index positions:

    ```python
    arr[0]  # Access first element
    ```

14. **How do you compute the dot product of two vectors using Numpy?**

    ```python
    np.dot(arr1, arr2)
    ```

15. **What happens if you try to compute the dot product of two vectors which have different sizes?**  
    It raises a `ValueError` due to incompatible sizes.

16. **How do you compute the element-wise product of two Numpy arrays?**

    ```python
    arr1 * arr2
    ```

17. **How do you compute the sum of all the elements in a Numpy array?**

    ```python
    np.sum(arr)
    ```

18. **What are the benefits of using Numpy arrays over Python lists for operating on numerical data?**  
    Numpy arrays are faster, use less memory, and support more mathematical operations.

19. **Why do Numpy array operations have better performance compared to Python functions and loops?**  
    Numpy arrays are implemented in C, allowing for optimized and vectorized operations.

20. **Illustrate the performance difference between Numpy array operations and Python loops using an example.**

    ```python
    %%time
    arr1_np + arr2_np  # Fast with Numpy

    %%time
    [x + y for x, y in zip(arr1, arr2)]  # Slower with Python lists
    ```

21. **What are multi-dimensional Numpy arrays?**  
    Numpy arrays with more than one dimension (e.g., matrices or higher).

22. **Illustrate the creation of Numpy arrays with 2, 3, and 4 dimensions.**

    ```python
    arr_2d = np.array([[1, 2], [3, 4]])  # 2D
    arr_3d = np.array([[[1], [2]], [[3], [4]]])  # 3D
    arr_4d = np.random.rand(2, 2, 2, 2)  # 4D
    ```

23. **How do you inspect the number of dimensions and the length along each dimension in a Numpy array?**

    ```python
    arr.ndim  # Number of dimensions
    arr.shape  # Length of each dimension
    ```

24. **Can the elements of a Numpy array have different data types?**  
    No, all elements must be of the same data type.

25. **How do you check the data type of the elements of a Numpy array?**

    ```python
    arr.dtype
    ```

26. **What is the data type of a Numpy array?**  
    It's the type of the elements stored in the array, like `int32`, `float64`, etc.

27. **What is the difference between a matrix and a 2D Numpy array?**  
    In Numpy, a matrix is a specialized 2D array, but the 2D array is more general and widely used.

28. **How do you perform matrix multiplication using Numpy?**

    ```python
    np.dot(matrix1, matrix2)
    ```

29. **What is the @ operator used for in Numpy?**  
    It is used for matrix multiplication.

30. **What is the CSV file format?**  
    CSV (Comma-Separated Values) is a file format where data is stored in rows, with each value separated by a comma.
