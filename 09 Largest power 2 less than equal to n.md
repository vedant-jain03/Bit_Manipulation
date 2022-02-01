```
#include <bits/stdc++.h>
using namespace std;

int find(int n)
{
    int x = 0;
    while((1<<x) <= n)x++;
    return x-1;
}

int main()
{
    int n;
    cin>>n;
    cout<<find(n);
}
```
