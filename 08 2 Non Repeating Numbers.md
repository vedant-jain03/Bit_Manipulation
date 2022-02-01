```
class Solution {
public:
    vector<int> singleNumber(vector<int>& nums) {
        vector<int> ans;
        int res = 0;
        for(auto x:nums) res=res^x;
        int mask = 1;
        while((mask & res) == 0) mask = mask << 1;
        int res1 = 0, res2=0;
        for(auto x:nums) {
            if((x&mask) == 0) res1=res1^x;
            else res2=res2^x;
        }
        ans.push_back(res1);
        ans.push_back(res2);
        return ans;
    }
};
```
