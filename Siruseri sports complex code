C++

#include "bits/stdc++.h"
using namespace std;

typedef long long  ll;
const int N = 1e3 + 10;
const long long NN = 1e11;
const long long int INF = 1e18;

vector<pair<ll, ll> > vp;

bool cmp(pair<ll, ll> a, pair<ll, ll> b){
    return a.second < b.second;
}

int main(int argc, char const *argv[])
{
    ios_base::sync_with_stdio(0);cin.tie(NULL);cout.tie(NULL);
    ll n, x, y, res = 0, Time = 0;
    cin >> n;
    for (int i = 0; i < n; ++i){
        cin >> x >> y;
        vp.push_back(make_pair(x, x + y));
    }
    sort(vp.begin(), vp.end(), cmp);
    for(int i = 0 ;i < vp.size(); ++i){
        if(vp[i].first >= Time){
            Time = vp[i].second;
            ++res;
        }
    }
    cout << res <<"\n";
}
