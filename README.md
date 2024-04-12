# Binary-search.c
 In this program:
- The `binarySearch` function takes three parameters: the array `arr`, the size of the array `n`, and the number to search for `x`.
- It uses a while loop to perform the binary search algorithm.
- The `low` variable is initialized to 0, representing the leftmost index of the array, and the `high` variable is initialized to `n - 1`, representing the rightmost index of the array.
- In each iteration of the while loop, the middle index `mid` is calculated as the average of `low` and `high`.
- If the element at `arr[mid]` is equal to `x`, the function returns `mid`, indicating that the element is found at index `mid`.
- If the element at `arr[mid]` is less than `x`, it means that the element may be present in the right half of the array, so `low` is updated to `mid + 1`.
- If the element at `arr[mid]` is greater than `x`, it means that the element may be present in the left half of the array, so `high` is updated to `mid - 1`.
- If the while loop terminates without finding the element, the function returns -1 to indicate that the element is not found.
- In the `main` function, an array `arr` is defined, and the number of elements `n` is calculated using the `sizeof` operator.
- The user is prompted to enter the number to search for using `printf` and `scanf`.
- The `binarySearch` function is called with the array, its size, and the number to search for.
- The result of the binary search is checked, and an appropriate message is printed to indicate whether the element is found or not.