# Sum Game

Problem URL:
https://leetcode.com/problems/sum-game/description/

## Solution

```cpp
class Solution {
public:
    bool sumGame(string num) {
        int sum = 0;

        for(int i=0; i<num.size()/2; i++) {
            if(num[i] != '?') {
                sum += (num[i]m- '0');
            }
        }

        int count = 0;
        for(int i=0; i<num.size(); i++) {
            if(num[i] == '?' && count % 2 == 0) {
                num[i] = '9';
                count++;
            } else if(num[i] != '?' && count % 2 == 0) {
                num[i] = '9';
                count++;
            }
        }
    }
};
```
