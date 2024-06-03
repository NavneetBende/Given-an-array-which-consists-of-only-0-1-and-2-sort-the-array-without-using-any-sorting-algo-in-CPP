Sort the array with elements 0, 1 and 2 in C++
Here, in this page we will discuss the program to sort the array with elements 0, 1 and 2 in C++ . We use the concept of counting the frequency of 0, 1 and 2 . We are giving with the size of the array along with array elements .We have to print sorted array.

sort the array with elements 0, 1 and 2 in C++
Algorithm :
Take the size of the array from the user and store it in variable say n.
Now, declare a vector of size n and take the n elements of the vector say arr from the user.
Declare three variables say count_0, count_1 and count_2 and initialize them with 0. (These variable will hold the count of the frequency of 0, 1 and 2).
Now, iterate over the array and increase the value of variable count_0 if arr[i] is 0 , count_1 if arr[i] is 1 and count_2 if arr[i] is 2 by value 1.
Now, clear the vector.
Declare variable say i and initialized it with 0.
Run a while loop till count_0 is not zero and inside while loop set arr[i++] =0.
Again Run a while loop till count_1 is not zero and inside while loop set arr[i++] =1.
At last again run while loop till count_2 is not zero and inside while loop set arr[i++] =2.
Finally the array get sorted without using any sorting technique and print the array.
Sort the array containing 0,1 and 2
Code in C++
#include<bits/stdc++.h>
using namespace std;
int main ()
{
 int n;
 cin >> n;
 int arr[n];
 for (int i = 0; i < n; i++) cin >> arr[i];
 int count_0 = 0, count_1 = 0, count_2 = 0;
 for (int i = 0; i < n; i++)
    {
        if (arr[i] == 0)
            count_0++;
        else if (arr[i] == 1)
            count_1++;
        else
            count_2++;
    }
    int i = 0;
    while(count_0--)
        arr[i++] = 0;
    while (count_1--)
        arr[i++] = 1;
    while (count_2--)
        arr[i++] = 2;
    for (int i = 0; i < n; i++)
        cout << arr[i] << " ";
    return 0;
}
Output :
6

1 0 0 1 0 0


0 0 0 0 1 1
