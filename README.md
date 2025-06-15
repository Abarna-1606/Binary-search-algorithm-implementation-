Here's how you can combine your idea of a terminal-based Python Unit Converter with Binary Search Algorithm implementation into a single project or program collection. Below is a breakdown of each, followed by the Binary Search implementation in the same style as your Unit Converter idea.


---

✅ Binary Search Tool (Python)

Welcome to the Binary Search Tool written in Python!
This is a simple terminal-based program that allows you to search for a number in a sorted list using the Binary Search algorithm.


---

🧠 How It Works

The user provides a sorted list and a target number.

The program performs a binary search and displays the index of the target number if found.



---

💡 Example Output

Enter sorted list of numbers (space-separated): 2 4 6 8 10 12
Enter number to search for: 10

✅ Element found at index 4


---

🛠️ Requirements

Python 3.x



---

▶️ How to Run

1. Save the file:



nano binary_search.py

2. Paste the code below into the file:



def binary_search(arr, target):
    low = 0
    high = len(arr) - 1

    while low <= high:
        mid = (low + high) // 2

        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            low = mid + 1
        else:
            high = mid - 1

    return -1


def main():
    print("🔍 Binary Search Tool")
    arr_input = input("Enter sorted list of numbers (space-separated): ")
    arr = list(map(int, arr_input.strip().split()))
    target = int(input("Enter number to search for: "))

    index = binary_search(arr, target)

    if index != -1:
        print(f"✅ Element found at index {index}")
    else:
        print("❌ Element not found")


if __name__ == "__main__"
