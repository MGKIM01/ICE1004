# 2020-2 ICE1004 ChoiHN Professor Final exam

<br/>

## 1번 문제

### Complete the program to produce the matrix multiplication and summation results as following

<img src = "https://user-images.githubusercontent.com/67851124/102856679-46cd1680-446a-11eb-8e8d-23ca3ffc32cf.JPG">

```

#include <iostream>
using namespace std;
#define AH ___________ //height of matrix A
#define AW ___________ //width of matrix A
#define BH ___________ //height of matrix B
#define BW ___________ //width of matrix B

void MatrixSum(int A[AH][BW], int B[AH][BW], int R[AH][BW])
{
	if (AH != BW)
	{
		cout << "Size error for matrix summation!" << endl;
	}
	else
	{
		//Matrix Summation







	}
}

void MatrixMulti(int A[AH][AW], int B[BH][BW], int R[AH][BW])
{
	if (_______ != ________)
	{
		cout << "Matrix Size error!" << endl;
	}
	else
	{
		//Matrix Multiplication








	}
}

void main()
{
	int A[AH][AW] = {___________________________};
	int B[BH][BW] = {___________________________};
	int C[__][__] = { ___________________________ };
	int R1[__][__] = { ___________________________ };
	int R2[__][__] = { ___________________________ };

	//print out the matrix A
	cout << "A = " << endl;
	for (int i = 0;i < AH;i++)
	{
		for (int j = 0; j < AW;j++)
		{
			cout << A[i][j] << "  ";
		}
		cout << endl;
	}
	cout << endl;

	//print out the matrix B
	cout << "B = " << endl;
	for (int i = 0; i < BH;i++)
	{
		for (int j = 0; j < BW;j++)
		{
			cout << B[i][j] << "  ";
		}
		cout << endl;
	}
	cout << endl;

	MatrixMulti(A, B, R1);
	//print out the matrix R1
	cout << "R1 = " << endl;
	for (int i = 0; i < AH;i++)
	{
		for (int j = 0; j < BW;j++)
		{
			cout << R1[i][j] << "  ";
		}
		cout << endl;
	}
	cout << endl;

	MatrixSum(R1, C, R2);
	//print out the matrix R2
	cout << "R2 = " << endl;
	for (int i = 0; i < AH;i++)
	{
		for (int j = 0; j < BW;j++)
		{
			cout << R2[i][j] << "  ";
		}
		cout << endl;
	}

}

```

## 2번 문제

### Load the "student_003.txt" file to compute average score of each subject (Korean, English, Math). Then store the result to the "evaulation.txt" file.

<div>
	<img src = "https://user-images.githubusercontent.com/67851124/102856891-c0fd9b00-446a-11eb-95f2-54dc67d797ee.png">
	</div>

