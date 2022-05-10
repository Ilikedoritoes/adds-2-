

//write a function that gets an array and adds to every number in it the num 2.

#include <stdlib.h>
#include <stdio.h>
#define SIZE 10

void two(int arr[], int size) // <--- adds 2 to each number
{
	int i;
	for (i = 0; i < SIZE; i++)
	{
		arr[i] = arr[i] + 2;
	}
}


void printarr(int arr[], int size) // <----prints the arrays
{
	int i=0;
	for (i = 0; i < SIZE; i++)
	{
		printf("%d ", arr[i]);
	}
}


void main()
{
	int i;
	int array[SIZE] = { 1,2,3,4,5,6,7,8,9,10 };

	printf("before adding 2.\n");
	printarr(array, SIZE); // <--- PRINTS INSTEAD OF THE WRITTING BELOW.

		/*for (i = 0; i < SIZE; i++)
		{
			printf("%d ", array[i]);
		}*/


	printf("\nafter adding 2.\n");
	two(array, SIZE); // <---- ADDS 2
	printarr(array, SIZE); // <--- PRINTS

		/*for (i = 0; i < SIZE; i++)
		{
			printf("%d ", array[i]);
		}*/

}
