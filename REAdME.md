# Reverse String (LeetCode 344)

## 📌 Problem Statement

Given an array of characters `s`, reverse the array **in-place**.

You must modify the input array directly without using extra space.

### Example

**Input**

```text
['h','e','l','l','o']
```

**Output**

```text
['o','l','l','e','h']
```

---

## 💡 Approach (Brute Force)

1. Create a new vector `ans`.
2. Traverse the original vector from the last index to the first.
3. Store each character in `ans`.
4. Copy `ans` back into the original vector `s`.

---

## 💻 Code

```cpp
class Solution {
public:
    void reverseString(vector<char>& s) {
        int n = s.size();
        vector<char> ans;

        for(int i = n - 1; i >= 0; i--) {
            ans.push_back(s[i]);
        }

        s = ans;
    }
};
```

---

## ⏱️ Complexity Analysis

* **Time Complexity:** `O(n)`
* **Space Complexity:** `O(n)`

---

## 🚀 Optimal Approach

Instead of creating another vector, use **two pointers**:

* One pointer starts from the beginning.
* Another pointer starts from the end.
* Swap both characters.
* Move the pointers toward each other until they meet.

### Complexity of Optimal Approach

* **Time Complexity:** `O(n)`
* **Space Complexity:** `O(1)`

---

## 🛠️ Concepts Used

* Arrays / Vectors
* Traversal
* Reversing an Array
* Two Pointers (Optimal Solution)

---

⭐ If you found this solution helpful, don't forget to star the repository!
