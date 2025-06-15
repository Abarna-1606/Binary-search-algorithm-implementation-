def binary_search(arr, target):
    low = 0
    high = len(arr) - 1

    while low <= high:
        mid = (low + high) // 2

        # Check if target is present at mid
        if arr[mid] == target:
            return mid  # Element found

        # If target greater, ignore left half
        elif arr[mid] < target:
            low = mid + 1

        # If target smaller, ignore right half
        else:
            high = mid - 1

    return -1  # Element not found# Binary-search-algorithm-implementation-
