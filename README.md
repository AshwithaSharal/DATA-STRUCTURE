# DATA-STRUCTURE
ARRAY OF ADDING 10 NUMBERS USING FOR

#include <iostream> 
 
using namespace std; 
 
int main() 
{ 
    int i,arr[10],sum=0; 
 
    cout<<"Enter 10 elements:"; 
    for(i=0;i<10;++i) 
        cin>>arr[i]; 
 
    for(i=0;i<10;++i) 
        sum=sum+arr[i]; 
    cout<<"Sum of numbers is:"<<sum; 
 
    return 0; 
}
                                    
OUTPUT:
Enter 10 elements:1 6 7 8 6 9 5 6 5 7<br>
Sum of numbers is:60
