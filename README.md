#include <map>
#include <set>
#include <list>
#include <cmath>
#include <ctime>
#include <deque>
#include <queue>
#include <stack>
#include <string>
#include <bitset>
#include <cstdio>
#include <limits>
#include <vector>
#include <climits>
#include <cstring>
#include <cstdlib>
#include <fstream>
#include <numeric>
#include <sstream>
#include <iostream>
#include <algorithm>
#include <unordered_map>

using namespace std;
int main() {

    int n,i,s=0,max;
   cin>>n;
    int a[n];
    for(i=0;i<n;i++){
       cin>>a[i];
    }
    max=0;
     for(i=0;i<n;i++){
             s=s+a[i];
             if(s>max){
                 max=s;
         }
         if(s<0){
             s=0;
         }
     }
    cout<<max;
    return 0;
}

