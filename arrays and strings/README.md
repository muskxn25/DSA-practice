# 📚 Arrays and Strings

This folder contains detailed explanations and examples of array and string data structures.

## 📂 Contents

1. [Static Arrays](./StaticArrays/README.md)
   - Fixed-size arrays
   - Memory allocation
   - Basic operations

2. [Dynamic Arrays](./DynamicArrays/README.md)
   - Resizable arrays
   - Amortized analysis
   - Common operations

3. [Strings](./Strings/README.md)
   - String manipulation
   - Common operations
   - Implementation examples

## 🎯 Learning Path

1. Start with Static Arrays to understand basic array concepts
2. Move to Dynamic Arrays to learn about resizable data structures
3. Finally, explore Strings to understand character sequence manipulation

## 📝 Notes

- All examples are implemented in Python
- Each section includes time complexity analysis
- Code examples are provided with detailed comments

# 📂 Static Arrays

### ✨ Concept

- Fixed-size collection of elements of the same type.
- Memory allocated once at creation (static).
- Elements stored in contiguous memory.
- Indexed access.

### 🕒 Time Complexity

| Operation     | Time Complexity |
|---------------|-----------------|
| Access        | O(1)            |
| Search        | O(n)            |
| Insert/Delete | O(n)            |

### 🧑‍💻 Example (Python)

```python
arr = [10, 20, 30, 40, 50]

# Access
print(arr[2])  # Output: 30

# Search
if 40 in arr:
    print("Found!")

# Insert (simulate by creating a new array)
arr = arr[:2] + [25] + arr[2:]

# Delete
arr.remove(20)
print(arr)

---

### 📂 DynamicArrays/README.md

```markdown
# 📂 Dynamic Arrays

### ✨ Concept

- Resizable array — size can change at runtime.
- Backed by a static array with dynamic reallocation.
- Efficient for append-heavy use cases.

### 🕒 Time Complexity

| Operation     | Time Complexity |
|---------------|-----------------|
| Access        | O(1)            |
| Search        | O(n)            |
| Insert/Delete | O(n)            |
| Append        | O(1) amortized  |

### 🧑‍💻 Example (Python)

```python
arr = []

# Append
arr.append(10)
arr.append(20)
arr.append(30)

print(arr)  # Output: [10, 20, 30]

# Access
print(arr[1])  # Output: 20

# Insert at index
arr.insert(1, 15)
print(arr)  # Output: [10, 15, 20, 30]

# Delete
arr.remove(15)
print(arr)

---

### 📂 Strings/README.md

```markdown
# 📂 Strings

### ✨ Concept

- Sequence of characters.
- Typically immutable.
- Supports slicing, searching, concatenation, etc.
- Commonly used for text processing.

### 🕒 Time Complexity

| Operation          | Time Complexity |
|--------------------|-----------------|
| Access (indexing)  | O(1)            |
| Search (substring) | O(n)            |
| Concatenation      | O(n)            |
| Substring          | O(n)            |

### 🧑‍💻 Example (Python)

```python
s = "hello world"

# Access
print(s[1])  # Output: 'e'

# Search (substring)
if "world" in s:
    print("Found!")

# Concatenation
s2 = s + "!"
print(s2)  # Output: 'hello world!'

# Substring
sub = s[0:5]
print(sub)  # Output: 'hello'
