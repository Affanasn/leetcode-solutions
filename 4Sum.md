# 4Sum

Problem URL:
https://leetcode.com/problems/4sum/description/

## Solution

```cpp
                    if (sum < target) {
                while (p < q) {
                    long long sum = (long long)nums[i] + nums[j] + nums[p] + nums[q];
                int p = j + 1, q = n - 1;
            for (int j = i + 1; j < n; j++) {
                if (j > i + 1 && nums[j] == nums[j - 1]) continue;
            if (i > 0 && nums[i] == nums[i - 1]) continue;
        for (int i = 0; i < n; i++) {
        int n = nums.size();
        sort(nums.begin(), nums.end());
```
