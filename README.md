# 🧠 NeetCode C++ Solutions  

This repository contains my C++ solutions to problems from [NeetCode.io](https://neetcode.io/), organized by topic.  
Each topic folder includes well-commented implementations and explanations inside the `.cpp` files.  

---

## 📂 Topic: Arrays & Hashing  

The **Arrays & Hashing** category includes some of the most essential problems that often appear in technical interviews.  
Mastering these helps build a solid foundation for data manipulation and problem-solving.

### 📘 Key Concepts

#### 🧱 Arrays (e.g., `std::vector`) 
A dynamic array in C++ implemented via `std::vector`.

- **Features:**
  * Random access in `O(1)` time
  * Automatically resizes as elements are added/removed
  * Efficient insertion/removal at the end: `O(1)` amortized
  * Insertion/deletion in the middle: `O(n)`
 
- **Common Operations:**
  ```cpp
  std::vector<int> nums = {1, 2, 3};
  nums.push_back(4);              // <-- Add element
  nums.pop_back();                // <-- Remove last element
  nums.size();                    // <-- Get size
  nums[i];                        // <-- Access element
  for (int x : nums) { ... }      // <-- Range-based loop
  ```

- **When to use:**
  * When frequent indexing or push_back is required.
 
- **Useful links:**
  * [cppreference - vector](https://en.cppreference.com/w/cpp/container/vector.html)

#### 🧩 Hash Maps (e.g., std::unordered_map)
A hash table that stores key-value pairs with fast average-case operations.

- **Features:**
  * Average `O(1)` time complexity for insertion, deletion, and lookup
  * Stores unique keys mapped to values
  * No guaranteed ordering of keys
  * Collision resolution via chaining

- **Common Operations:**
 ``` cpp
 std::unordered_map<char, int> freq;
 freq['a']++;                    // <-- Increment frequency
 if (freq.count('b')) { ... }   // <-- Check if key exists
 freq.erase('c');               // <-- Remove key
 for (auto& [key, val] : freq) {
     std::cout << key << ": " << val << "\n";
 }
```
  
---  

### 🔗 Problem List  

---  

📌 **Note:** This README includes only **theory** and links to solution files.  
Explanations and step-by-step logic are documented as comments within each `.cpp` file.


