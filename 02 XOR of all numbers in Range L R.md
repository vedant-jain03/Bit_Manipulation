```
#include <bits/stdc++.h>
using namespace std;


int xorans(int n)
{
    if(n%4 == 0) return n;
    if(n%4 == 1) return 1;
    if(n%4 == 2) return n+1;
    if(n%4 == 3) return 0;
}
int main()
{
    int l;
    int r;
    cin>>l>>r;
    cout<<(xorans(r)^xorans(l-1));
}
```
