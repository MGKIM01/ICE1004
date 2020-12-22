## Final exam Answer2

```c

#include <iostream>
using namespace std;
#define _CRT_SECURE_NO_WARNINGS
#pragma warning(disable:4996)


int main()
{
	FILE* fp = fopen("student003.txt", "r");

	if (fp == NULL)
	{
		cout << "ERROR!" << endl;
		exit(1);
	}

	int number;
	char name[20];
	float korean_total = 0, english_total = 0, math_total = 0;
	int korean, english, math;

	for (int i = 0; i < 4;i++)
	{
		fscanf(fp, "%d %s %d %d %d", &number, name, &korean, &english, &math);
		korean_total += korean;
		english_total += english;
		math_total += math;
	}
	float mean1 = korean_total / 4;
	float mean2 = english_total / 4;
	float mean3 = math_total / 4;

	cout << mean1 << endl;
	cout << mean2 << endl;
	cout << mean3 << endl;

	fclose(fp);

	
	FILE* fp2 = fopen("evaluation.txt", "w");
	fprintf(fp, "%.3f %.3f %.3f", mean1, mean2, mean3);

}

```
