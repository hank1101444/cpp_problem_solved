```cpp
// Fig. 9.1: fig09_01.cpp
// Time class.
#include <iostream>
#include <iomanip>
using namespace std;

// Time class definition

// 在上面為什麼可使用
void test() {
	Time t;
	t.hour = 1;

}

class Time
{
public:
	Time(); // constructor
	void setTime(int h, int m, int s); // set hour, minute and second
	void printUniversal(); // print time in universal-time format
	void printStandard(); // print time in standard-time format
//private:
	int hour; // 0 - 23 (24-hour clock format)
	int minute; // 0 - 59
	int second; // 0 - 59
}; // end class Time


// class 可使用 只是要放在 class function 裡
class test {
	Time t;
	t.hour = 1;
};

```
