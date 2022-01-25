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
 ![image](https://user-images.githubusercontent.com/98145023/150925825-27c1da30-d6cf-4bc6-a7c7-cd8d1cbfd677.png)<br><br>
	
	#include <iostream> 
 
using namespace std; 
 
int main() 
{ 
    int i,arr[10],sum1=0,sum2=0,sum3=0,n; 
     char ch;
    do{
 	 cout<<"ENTER CHOICE\n"<<"1.For\n"<<"2.While\n"<<"3.Do While\n";
    cout<<"Make a choice: ";
    cin>>n;
     
    switch(n)
    {
        case 1:  
        	cout<<"Enter 10 elements:\n"; 
    for(i=0;i<10;++i) 
      cin>>arr[i]; 
	  for(i=0;i<10;++i) 
        sum1=sum1+arr[i]; 
    
    cout<<"Sum of numbers is:"<<sum1; 
 
            
            break;
         
        case 2 : 
        	cout<<"Enter 10 elements:\n"; 
        i=0;
        while(i<10)
        {
        	cin>>arr[i];
        	i++;
		}
		i=0;
		while(i<10) 
		{
			sum2=sum2+arr[i];
			i++; 
		}
        cout<<"Sum of numbers is:"<<sum2; 
            
            break;
         
        case 3 : 
        cout<<"Enter 10 elements:\n"; 
        i=0;
        do{
        		cin>>arr[i];
        		i++;
		}while(i<10);
        
         i=0;
        do{
        		sum3=sum3+arr[i];
        		i++;
		}while(i<10);
		 cout<<"Sum of numbers is:"<<sum3; 
            break;
             
        default : 
            cout<<"Invalid Choice\n";
    }
     
    cout<<"\nDo you want to continue ? : ";
    cin>>ch;
 
    }while(ch=='Y'||ch=='y');
     
    return 0;
}<br><br>
	OUTPUT:<br>
	![image](https://user-images.githubusercontent.com/98145023/150928704-83a51495-6542-4ae2-a269-0645d7134f41.png)<br><br><br>
	
	
	ARRAY USING STACKS<br><br>
	#include <iostream>
using namespace std;
int stack[100], n=100, top=-1;<br>
void push(int val) <br>{<br>
   if(top>=n-1)<br>
   cout<<"Stack Overflow"<<endl;<br>
   else <br>{<br>
      top++;<br>
      stack[top]=val;<br>
   }<br>
}<br>
void pop()<br> {<br>
   if(top<=-1)<br>
   cout<<"Stack Underflow"<<endl;<br>
   else <br>{<br>
      cout<<"The popped element is "<< stack[top] <<endl;<br>
      top--;<br>
   }<br>
}<br>
void display() <br>{<br>
   if(top>=0) <br>{<br>
      cout<<"Stack elements are:";<br>
      for(int i=top; i>=0; i--)<br>
      cout<<stack[i]<<" ";<br>
      cout<<endl;<br>
   }<br> else<br>
   cout<<"Stack is empty";<br>
}<br>
int main()<br> {<br>
   int ch, val;<br>
   cout<<"1) Push in stack"<<endl;<br>
   cout<<"2) Pop from stack"<<endl;<br>
   cout<<"3) Display stack"<<endl;<br>
   cout<<"4) Exit"<<endl;<br>
   do<br> {<br>
      cout<<"Enter choice: "<<endl;<br>
      cin>>ch;<br>
      switch(ch) {<br>
         case 1: {<br>
            cout<<"Enter value to be pushed:"<<endl;<br>
            cin>>val;<br>
            push(val);<br>
            break;<br>
         }<br>
         case 2: {<br>
            pop();<br>
            break;<br>
         }<br>
         case 3: {<br>
            display();<br>
            break;<br>
         }<br>
         case 4: {<br>
            cout<<"Exit"<<endl;<br>
            break;<br>
         }<br>
         default: {<br>
            cout<<"Invalid Choice"<<endl;<br>
         }<br>
      }<br>
   }<br>while(ch!=4);<br>
   return 0;<br>
}<br>

	OUTPUT:
![image](https://user-images.githubusercontent.com/98145023/150932273-8406c171-c1c1-46e9-96bf-635bc43fd77b.png)
<br><br>
