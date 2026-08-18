# Kids With the Greatest Number of Candies

Problem URL:
https://leetcode.com/problems/kids-with-the-greatest-number-of-candies/description/

## Solution

```cpp
class Solution {
public:
    vector<bool> kidsWithCandies(vector<int>& candies, int extraCandies) {
        int n = candies.size();
        vector<bool> result(n, false);

        int maxi = INT_MIN;
        for(int i=0; i<n; i++) {
            maxi = max(maxi, candies[i]);
        }

        for(int i=0; i<n; i++) {
            if(candies[i] + extraCandies >= maxi) {
                result[i] = true;
            }
        }

        return result;
    }
};
```
