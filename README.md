# insertion_sort_desc.py
def insertion_sort_desc(arr):
    for i in range(1, len(arr)):
        key = arr[i]
        j = i - 1
        # For decreasing order, use key > arr[j]
        while j >= 0 and key > arr[j]:
            arr[j + 1] = arr[j]
            j -= 1
        arr[j + 1] = key

# Example usage
if __name__ == "__main__":
    data = [12, 4, 56, 17, 8, 99, 1]
    print("Original:", data)
    insertion_sort_desc(data)
    print("Sorted (Descending):", data)
    # Added user input functionality
if __name__ == "__main__":
    data = [int(x) for x in input("Enter numbers separated by space: ").split()]
    print("Original:", data)
    insertion_sort_desc(data)
    print("Sorted (Descending):", data)

