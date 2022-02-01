```
vector<string> AllPossibleStrings(string s){
		    // Code here
		    vector<string> ans;
		    int n=s.size();
		    for(int i=0;i<(1<<n);i++)
		    {
		        string res="";
		        for(int j=0;j<n;j++)
		        {
		            if(i&(1<<j)) {
		                res+=s[j];
		            }
		        }
		        if(res!="")ans.push_back(res);
		    }
		    return ans;
		}
```
