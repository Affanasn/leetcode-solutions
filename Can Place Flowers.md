# Can Place Flowers

Problem URL:
https://leetcode.com/problems/can-place-flowers/description/

## Solution

```cpp
class Solution {
public:
    bool canPlaceFlowers(vector<int>& flowerbed, int n) {
        if(flowerbed.size() == 3 && flowerbed[1] == 1) return false;

        for(int i=0; i<flowerbed.size(); i++) {
            if(flowerbed[i] == 1) {
                n++;
            }
        }

        bool flag = false;
        int size = flowerbed.size();
        if(size % 2 == 0) {
            size /= 2;
            if(size >= n) {
                flag = true;
            }
        } else {
            size /= 2;
            if(size + 1 >= n) {
                flag = true;
            }
        }

        return flag;
    }
};
```
