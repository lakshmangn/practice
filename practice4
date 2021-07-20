#include <bits/stdc++.h>
using namespace std;
vector<int>ar[100001];
bool vis[100001];
int dfs(int n){
    vis[n]=true;
    for(int x:ar[n]){
        if(!vis[x]){
            return 1+dfs(x);
        }
    }
    return 1;
}
int main() {
    int t;
    cin>>t;
    while(t--){
        int n,m;
        cin>>n>>m;
        int a,b;
        for(int i=1;i<=n;i++){
            ar[i].clear();
            vis[i]=false;
        }
        for(int i=1;i<=m;i++){
            cin>>a>>b;
            ar[a].push_back(b);
            ar[b].push_back(a);
        }
        int c=0;
       long long  int x=1;
        for(int i=1;i<=n;i++){
            if(!vis[i]){
                c++;
                x=(x%1000000007*dfs(I)%100000007)%100000007;
            }
        }
        cout<<c<<" "<<x<<endl;
    }
	return 0;
}
