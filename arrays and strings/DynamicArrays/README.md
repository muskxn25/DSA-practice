# 📂 Dynamic Arrays

### ✨ Concept

- Resizable array — size can change at runtime
- Backed by a static array with dynamic reallocation
- Efficient for append-heavy use cases
- Automatically handles memory management

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
```

### 📝 Key Points

1. **Memory Management**
   - Automatic resizing
   - Amortized O(1) for append
   - Memory reallocation strategy

2. **Common Operations**
   - Dynamic resizing
   - Efficient appending
   - Flexible insertion/deletion

3. **Use Cases**
   - When size is unknown
   - When frequent appending is needed
   - When flexibility is required 