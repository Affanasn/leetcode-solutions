# Word Break

Problem URL:
https://leetcode.com/problems/word-break/description/

## Solution

```cpp
class Solution {
public:
    class Node {
    public:
        unordered_map<char, Node*> children;
        bool endOfWord;
        Node() {
            endOfWord = false;
        }
```
