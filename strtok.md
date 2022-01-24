```cpp
#include <iostream>
using namespace std;
#include <cstring>

int main() {

	//string a = "12345 234,34 4";
	char a[] = "12345 234,34 4";
	char p[] = " ,";
	char* z = NULL;
	// 
	char* token = strtok_s(a, p, &z);
	while (token) {
		cout << token << endl;
		token = strtok_s(0, p, &z);
	}


	return 0;
}
```
&nbsp;
## vector string 解
```cpp
#include <iostream>
using namespace std;
#include<string>
#include<vector>
int main() {
	vector <int> z;
	string a = "123 456 4";
	int temp = 0;
	for (int i = 0; i < a.size(); i++) {
		if (a[i] != ' ') {
			temp *= 10;
			temp += a[i] - '0';
		}
		else {
			z.push_back(temp);
			temp = 0;
		}
	}
	// 讀最後一個數字 如果最後是空白會讀到0
	z.push_back(temp);
	int n;

	return 0;
}
```
