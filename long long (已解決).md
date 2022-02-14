# 等號右邊以範圍最大的當型態, 所以只要右邊有一個long long int即可
```cpp
#include <iostream>
#include <vector>
#include <string>
#include <algorithm>
using namespace std;
int main()
{
    int x = 1;
    vector<int> v = {-1073741824 , 1073741824};
        long long int ans = 0;
        int mul = 1;
        for ( int i = 0; i < v.size(); i++)
        {
            //ans += v[i] * i * pow(x, i - 1);
            ans += v[i] * (i + 1) * mul;
            mul *= x;
        }
        cout << ans << endl;

    return 0;
}


//
//
//#include <string>
//#include <iostream>
//using namespace std;
//#include <algorithm>
//#include <cmath>
//int main()
//{
//	string s;
//	while (getline(cin, s))
//	{
//		int flag = 0;
//		string temp = "0123456789"
//			"ABCDEFGHIJKLMNOPQRSTUVWXYZ"
//			"abcdefghijklmnopqrstuvwxyz";
//		string stemp = s;  // sort
//		sort(stemp.begin(), stemp.end());
//		char a = stemp[stemp.size() - 1];
//
//		int ans = 0;
//		reverse(s.begin(), s.end());
//		for (int i = (temp.find(a)) + 1; i != temp.size(); i++) {
//			// 123 -> n^0*3 +n^1*2....
//			long long int dividend = 0;
//			for (int j = 0; j < s.size(); j++) {
//				//arping
//				dividend += (pow(i, j)) * (temp.find(s[j]));
//			}
//			if (dividend % (i - 1) == 0) {
//				flag = 1;
//				ans = i;
//				break;
//			}
//		}
//		if (flag == 1) {
//			cout << ans << endl;
//		}
//
//		else {
//			cout << "such number is impossible" << endl;
//		}
//	}
//	return 0;
//}
```
