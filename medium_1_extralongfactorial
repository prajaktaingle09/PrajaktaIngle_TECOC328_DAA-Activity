#include <bits/stdc++.h>

using namespace std;

// Complete the extraLongFactorials function below.
void extraLongFactorials(int n) {
    int val[500],sz;
    val[0] = 1;
    sz = 1;
    for(int i = 2; i <= n; i++){

        int cary = 0;
        for(int j = 0; j < sz; j++){
            int pod = val[j]*i+cary;
            val[j] = pod%10;
            cary = pod/10;
        }
        while(cary){
            val[sz] = cary%10;
            cary/=10;
            sz++;
        }
    }
    for(int i = sz-1; i>= 0; i--)
    cout << val[i];
    cout << endl;
   
}

int main()
{
    int n;
    cin >> n;
    cin.ignore(numeric_limits<streamsize>::max(), '\n');

    extraLongFactorials(n);

    return 0;
}
