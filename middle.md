# 2020-2 ICE1004 ChoiHN Professor Midterm exam

## 1번 

### Using the swtich statement to rewrite the following code instead of if statement.(should be produce same results with given code)
``` 
# include <iostream>
using namespace std;

int main()
{
	char x = 'C';
	if (x == 'a' && x == 'A')
	{
		cout << x << endl;
	}
	else if (x == 'b' || x == 'B')
	{
		cout << x << endl;
	}
	else if (x == 'c' || x == 'C')
	{
		cout << x << endl;
	}
	else if (x == 'd' || x == 'D')
	{
		cout << x << endl;
	}
	else
	{
		cout << "midterm exam" << endl;
	}
	return 0;
  ```
  click this to show answer :  [Ans.1](./middle_sol1.md)

  
  ## 2번
  
  ### Write a program to solve following problem
  ```
  Read  10 numbers and output the maximum and its location.
  
  Enter 10 numbers
  
  320 1440 80 12 33 21 88 10 11 20
  
  The max: 1440
  
  The location of max: 1 (starting index from 0)
  ```
click this to show answer : [Ans.2](./middle_sol2.md)
