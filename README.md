# DATA-STRUCTURE
ARRAY OF ADDING 10 NUMBERS USING FOR

#include <iostream.h>
 
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
                                    
OUTPUT:<br><br>
![image](https://user-images.githubusercontent.com/98145023/150921910-01833145-18b8-40e4-8643-aa2ab734e192.png)<br><br><br><br>

ARRAY TO ADD 10 ELEMENTS USING WHILE LOOP<br><br>
#include <iostream><br>
 
using namespace std; <br>
 
int main() <br>
{ <br>
    int i,arr[10],sum=0,number,n; <br>
     cout<<"Enter 10 elements:";<br>
     cin>>n;<br>
     while(n>0)<br>
	{<br>
		cin>>number;<br>
		sum+=number;<br>
		n--;<br>
	}<br>
	cout<<"\n sum is:"<<sum;<br>
	return 0;<br>
}<br>
 
 OUTPUT:<br><br>
 ![image](https://user-images.githubusercontent.com/98145023/150925825-27c1da30-d6cf-4bc6-a7c7-cd8d1cbfd677.png)
