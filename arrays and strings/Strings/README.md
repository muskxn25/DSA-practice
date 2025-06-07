# 📂 Strings

### ✨ Concept

- Sequence of characters
- Typically immutable
- Supports slicing, searching, concatenation, etc.
- Commonly used for text processing

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
```

### 📝 Key Points

1. **String Properties**
   - Immutability
   - Character encoding
   - Memory representation

2. **Common Operations**
   - String manipulation
   - Pattern matching
   - Text processing

3. **Use Cases**
   - Text processing
   - Data validation
   - Pattern matching
   - String parsing 