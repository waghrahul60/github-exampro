# Github Documentation

## Step 1 - Using CodeBlocks.

Codeblocks in markdown is *very easy* for tech peoplr to **copy** the code. [<sup>[1]</sup>](#references)


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

<img width="400px" src="https://github.com/waghrahul60/github-docs-example/blob/main/image.png" />

Good cloud Enginners use codeblocks for both code and Errors that appers in console


```bash
$ ls /nonexistent_directory
ls: cannot access '/nonexistent_directory': No such file or directory

```

> This is the most import quote // this is used for errors that appers on bash

## Step 3 - Use github flavered Task List

Github extends Markdown to have a list where you cab check off items.
- [x] Finish Step 1
- [] finish Step 2
- [] finish Step 3

## Step 4 - Used imoji

GitHub Flavord Markdoen (GFM) Emojis


| Name  | Shortcode | Emoji |
| ------------- | ------------- | ------------- |
| Cloud  | `:cloud:`  | :cloud: |
| cloud_with_snow | `:cloud_with_snow:` | :cloud_with_snow: |

## Step 4 - Github tables

```md
| Name  | Shortcode | Emoji |
| ------------- | ------------- | ------------- |
| Cloud  | `:cloud:`  | :cloud: |
| cloud_with_snow | `:cloud_with_snow:` | :cloud_with_snow: |
```
Github Extends the functionality of Markdoen tables to provide more alignment and table cellformatting options. [<sup>[2]</sup>](#references)


## References

- [Basic writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)<sup>[1]</sup>
- [Archtrtecture diagram ](https://lucid.app/lucidchart/e3f15b1a-2211-4ddb-8c95-f144c2504db4/edit?invitationId=inv_0873b3c6-c652-463f-9f2b-fa0f1b420823&page=0_0#)
- [GFM - task list](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists)
- [GFM - Emoji sheet](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)
- [GFM - Tables ](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-tables) <sup>[2]</sup>

