# Two Sum

Problem URL:
https://leetcode.com/problems/two-sum/description/

## Solution

```cpp
class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {
        unordered_map<int,int> m;
        vector<int> ans;
        int n=nums.size();
        for(int i=0; i<n;i++){
            int f=nums[i];
            int s=target-f;
            if(m.find(s) != m.end()){
                ans.push_back(i);
                ans.push_back(m[s]);
                break;
            }
            m[f] = i;
        }
    return ans;
    }
};
```
