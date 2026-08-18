# Climbing Stairs

Problem URL:
https://leetcode.com/problems/climbing-stairs/description/

## Solution

```cpp
class Solution {
public:
    int climbStairs(int n) {
        if(n == 1 || n == 2) return n;

        return climbStairs(n-1) + climbStairs(n-2);
    }
};
```
