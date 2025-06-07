# 📂 Static Arrays

### ✨ Concept

- Fixed-size collection of elements of the same type
- Memory allocated once at creation (static)
- Elements stored in contiguous memory
- Indexed access

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
```

### 📝 Key Points

1. **Memory Allocation**
   - Fixed size at creation
   - Cannot be resized
   - Contiguous memory blocks

2. **Common Operations**
   - Random access
   - Sequential search
   - Insert/Delete with shifting

3. **Use Cases**
   - When size is known in advance
   - When random access is needed
   - When memory efficiency is important 