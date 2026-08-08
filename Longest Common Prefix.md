# Longest Common Prefix

Problem URL:
https://leetcode.com/problems/longest-common-prefix/description/?envType=problem-list-v2&envId=trie

## Solution

```cpp
            return strs[0];
        }
        string pre = strs[0];
        for(int i=1; i<strs.size(); i++){
            string result = "";
            string temp = strs[i];
            for(int j=0; j<strs[i].size(); j++){
                if(j < pre.size() && pre[j] == temp[j] ){
                    result = result + temp[j];
                }else{
                    break;
                }
            }
            pre = result;
            if(pre
        }
```
