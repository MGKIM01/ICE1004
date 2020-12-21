# Answer2

#### 교수님 왈 : 강의노트에 나와있는 코드는 버그가 있다. 이 버그를 해결한 코드를 제시하여라

```
#include <iostream>
using namespace std;

int main()
{
	cout << "Enter 10 numbers and output the maximumm and its location" << endl;
	cout << "Enter 10 numbers" << endl;
	int max; cin >> max; //제일 처음 입력한 값을 max값으로 설정(bug 해결)
	int location;
	int num = 1;
	while (1)
	{
		int a; cin >> a;
		if (max < a)
		{
			location = num;
			max = a;
		}
		num++;
		if (num == 10)
		{
			break;
		}
	}
	cout << "The max : " << max << endl;
	cout << "The location of max : " << location << endl;
}

```
#include <iostream>
using namespace std;

int main()
{
	cout << "Enter 10 numbers and output the maximumm and its location" << endl;
	cout << "Enter 10 numbers" << endl;
	int a;
	cin >> a;
	int max = a; //첫 입력값을 max값으로 설정해줌으로써 버그 제거
	int location = 0; //0으로 초기화시켜주지 않으면 (첫 입력값이 가장 큰 경우에) 버그 생김
	for (int i = 1;i < 9;i++)
	{
		cin >> a;
		if (max < a)
		{
			max = a;
			location = i;
		}
	}

	cout << "The max: " << max << endl;
	cout << "The location of max: " << location << endl;
}

```
