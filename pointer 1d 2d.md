```cpp
#include <iostream>
using namespace std;

int main() {
    // 2d
    int* tt = new int[5]();
    int** test = &tt;
    for (int i = 0; i < 5; ++i) {
        tt[i] += i + 1;
    }

    // 1d
    /*int tt2[10] = {};
    int* test = tt2;
    cout << test << endl << &tt2[0]<<endl << &tt2 <<endl;*/

    for (int i = 0; i < 5; ++i) {
        //cout << *(*(test + 0) + i) << ' ';
        cout << test[0][i] << ' ';
    }
    return 0;
}

```
