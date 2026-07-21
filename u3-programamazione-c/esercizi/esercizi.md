C Programming Exercises
============================

Source: [https://www.w3resource.com/c-programming-exercises/]([https://www.w3resource.com/c-programming-exercises/)


# 1. Variables and Expressions

## Exercise 1.1

Write a C program to print your name, date of birth and mobile number. 
**Expected Output:**
```
Name   : Mario Rossi
DOB    : 05 December, 1984  
Mobile : 99-9999999999
```
**Solution:**
```c
#include <stdio.h>
int main(){
		char nome[20] = "Mario Rossi";
		char dob[20] = "05 December, 1984";
		char mobile[20] = "99-9999999999";

		printf("Name  : %s\n", nome);
		printf("DOB   :%s\n", dob);
		printf("Mobile:%s\n", mobile);
}
```

## Exercise 1.2

Write a C program to print a block F using hash (#), where the F has a height of six characters and width of five and four characters. And also to print a big 'C'. 

**Solution:**
```c
#include <stdio.h>
int main(){
	printf("######\n");
	printf("#\n");
	printf("#\n");
	printf("#####\n");
	printf("#\n");
	printf("#\n");
	printf("#\n");
	

	printf("  #######\n");
	printf(" ##    	##\n");
	printf("#\n");
	printf("#\n");
	printf("#\n");
	printf("#\n");
	printf("#\n");
	printf(" ##    	##\n");
	printf("  #######\n");
	return 0;
}
```

## Exercise 1.3

Write a C program to print the following characters in a reverse way. 
Test Characters: 'X', 'M', 'L'

**Expected Output:**
The reverse of XML is LMX

**Solution:**
```c
#include <stdio.h>

int main(int argc, char const *argv[])
{
	char test[4] = {'X','M','L','\0'};

	printf("%c %c %c \n", test[2], test[1], test[0]);

	return 0;
}
```

## Exercise 1.4

Write a C program to compute the perimeter and area of a rectangle with a height of 7 inches and width of 5 inches. 

**Expected Output:**
```
Perimeter of the rectangle = 24 inches
Area of the rectangle = 35 square inches
```
**Solution:**
```c
#include <stdio.h>

int main(int argc, char const *argv[])
{
	float perimeter;
	float area;

	int height = 7;
	int width = 5;

	printf("Perimeter = %d\n", (2*height)+(2*width));
	printf("Area = %d\n", (height * width));


	return 0;
}
```


## Exercise 1.5

Write a C program to compute the perimeter and area of a circle with a given radius. 

**Expected Output:**
```
Perimeter of the Circle = 37.680000 inches
Area of the Circle = 113.040001 square inches
```
**Solution:**
```c
#include <stdio.h>
#include <stdlib.h>

int main(int argc, char const *argv[])
{

	const float PI = 3.14159; 

	int radius = 0;
	float perimeter = 0;
	float area = 0;

	radius = atoi(argv[1]); //alphabetical to int
	perimeter = 2*PI*radius;
	area = 2*PI*radius*radius;
	
	printf("Perimeter of the Circle: %f\n", (float)perimeter);
	printf("Area of the Circle: %f\n", (float)area);

	return 0;
}
```



## Exercise 1.6

Write a C program to convert a given integer (in seconds) to hours, minutes and seconds.

**Expected Output:**
```
Input seconds: 25300                                                   
H:M:S - 7:1:40
```
**Solution:**
```c
#include <stdio.h>
int main() {
	int sec, h, m, s;
	printf("Input seconds: ");
	scanf("%d", &sec);
	
	h = (sec/3600); 
	m = (sec -(3600*h))/60;
	s = (sec -(3600*h)-(m*60));
	printf("H:M:S - %d:%d:%d\n",h,m,s);
	
	return 0;
}
```

## Exercise 1.7

Write a C program that reads two integers and checks whether they are multiplied or not.

**Expected Output:**
```
Input the first number: 5                                              
Input the second number: 15
Multiplied!
```
**Solution:**
```c
#include <stdio.h>

int main() {
	int  x, y;
    printf("\nInput the first number: "); 
    scanf("%d", &x);
    printf("\nInput the second number: ");
    scanf("%d", &y);
  
    if(x > y) 
	{
		int temp;
		temp = x;
		x = y;
		y = temp;
	}
	
	if((y % x)== 0) 
	{
		printf("\nMultiplied!\n");
	} 
	else 
	{
		printf("\nNot Multiplied!\n");
	}
	
	return 0;
}
```

# 2. Flow control

# 3. Console Operations

# 4. Strings

# 5. Files


