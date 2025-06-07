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
