#include <bits/stdc++.h>
using namespace std;

vector<vector<int>> a;
int n, m;
void BFS(int s){
    vector <bool> visited;
    visited.resize(n+1, false);
    queue <int> q;
    visited[s]=true;
    q.push(s);
    while(!q.empty()){
        s = q.front();
        cout<<s<<" ";
        q.pop();
        for (auto i: a[s])
            if (!visited[i]){
                visited[i]=true;
                q.push(i);
            }   
    }
}

int main(){
    cin >> n >> m;
    a.resize(m+1);
    for (int i = 1; i<=m; i++){
        int u, v;
        cin >> u >> v;
        a[u].push_back(v);
        a[v].push_back(u);
    }
    BFS(1);
}
