# Github Documentation

## Step 1 - Using CodeBlocks.

Codeblocks in markdown is *very easy* for tech peoplr to **copy** the code.


In order to create code block you need to used backtiks.

```
def merge_sort(arr):
    if len(arr) <= 1:
        return arr

    # Split the input array into two halves
    middle = len(arr) // 2
    left_half = arr[:middle]
    right_half = arr[middle:]

    # Recursively sort both halves
    left_half = merge_sort(left_half)
    right_half = merge_sort(right_half)

    # Merge the sorted halves
    return merge(left_half, right_half)

def merge(left, right):
    result = []
    left_idx, right_idx = 0, 0

    while left_idx < len(left) and right_idx < len(right):
        if left[left_idx] < right[right_idx]:
            result.append(left[left_idx])
            left_idx += 1
        else:
            result.append(right[right_idx])
            right_idx += 1

    # Append the remaining elements from both lists (if any)
    result.extend(left[left_idx:])
    result.extend(right[right_idx:])

    return result

# Example usage:
if __name__ == "__main__":
    unsorted_list = [12, 11, 13, 5, 6, 7]
    sorted_list = merge_sort(unsorted_list)
    print("Sorted array is:", sorted_list)

```

- when you can highlite the syntex for language

```python
def merge_sort(arr):
    if len(arr) <= 1:
        return arr

    # Split the input array into two halves
    middle = len(arr) // 2
    left_half = arr[:middle]
    right_half = arr[middle:]

    # Recursively sort both halves
    left_half = merge_sort(left_half)
    right_half = merge_sort(right_half)

    # Merge the sorted halves
    return merge(left_half, right_half)

def merge(left, right):
    result = []
    left_idx, right_idx = 0, 0

    while left_idx < len(left) and right_idx < len(right):
        if left[left_idx] < right[right_idx]:
            result.append(left[left_idx])
            left_idx += 1
        else:
            result.append(right[right_idx])
            right_idx += 1

    # Append the remaining elements from both lists (if any)
    result.extend(left[left_idx:])
    result.extend(right[right_idx:])

    return result

# Example usage:
if __name__ == "__main__":
    unsorted_list = [12, 11, 13, 5, 6, 7]
    sorted_list = merge_sort(unsorted_list)
    print("Sorted array is:", sorted_list)

```

- add an image 

![Alt text](image.png)

- image with image tag

<img width="400px"src="https://github.com/waghrahul60/github-docs-example/blob/main/image.png" />