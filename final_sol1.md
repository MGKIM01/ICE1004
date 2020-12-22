##final exam Answer1

```

#include <iostream>
using namespace std;

#define AH 5
#define AW 1
#define BH 1
#define BW 5 

void MatrixSum(int A[AH][BW], int B[AH][BW], int R[AH][BW]);
void MatrixMulti(int A[AH][AW], int B[BH][BW], int R[AH][BW]);

void main()
{
	int A[5][1] = { {1},{1},{1},{1},{1} };
	int B[1][5] = { 1,2,3,4,5 };
	int C[5][5] = { {5,0,0,0,0},{0,4,0,0,0},{0,0,3,0,0},{0,0,0,2,0}, {0,0,0,0,1} };
	int R1[5][5] = { 0 };
	int R2[5][5] = { 0 };

	cout << "A = " << endl;
	for (int i = 0; i < AH;i++)
	{
		for (int j = 0; j < AW; j++)
		{
			cout << A[i][j] << endl;
		}
	}
	//Execution result와 동일하게 하기 위해 예제 코드를 변경하였습니다. 

	cout << endl;

	cout << "B = " << endl;
	for (int i = 0; i < BH;i++)
	{
		for (int j = 0; j < BW; j++)
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
		for (int j = 0; j < BW; j++)
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
		for (int j = 0; j < BW; j++)
		{
			cout << R2[i][j] << "  ";
		}
		cout << endl;
	}

}


void MatrixSum(int A[AH][BW], int B[AH][BW], int R[AH][BW])
{

	if (AH != BW)
	{
		cout << "Size error for matrix summation!" << endl;
	}
	else
	{
		for (int i = 0;i < 5;i++)
		{
			for (int j = 0; j < 5; j++)
			{
				R[i][j] = A[i][j] + B[i][j];
			}
		}
	}

}

void MatrixMulti(int A[AH][AW], int B[BH][BW], int R[AH][BW])
{

	if (AH != BW)
	{
		cout << "Size error for matrix summation!" << endl;
	}
	else
	{
		for (int i = 0;i < 5;i++)
		{
			for (int j = 0; j < 5; j++)
			{
				R[i][j] = A[i][0] * B[0][j];
			}
		}
	}

}

```
