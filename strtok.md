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
