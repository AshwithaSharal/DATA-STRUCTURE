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
int stack[100], n=100, top=-1;
void push(int val) {
   if(top>=n-1)
   cout<<"Stack Overflow"<<endl;
   else {
      top++;
      stack[top]=val;
   }
}
void pop() {
   if(top<=-1)
   cout<<"Stack Underflow"<<endl;
   else {
      cout<<"The popped element is "<< stack[top] <<endl;
      top--;
   }
}
void display() {
   if(top>=0) {
      cout<<"Stack elements are:";
      for(int i=top; i>=0; i--)
      cout<<stack[i]<<" ";
      cout<<endl;
   } else
   cout<<"Stack is empty";
}
int main() {
   int ch, val;
   cout<<"1) Push in stack"<<endl;
   cout<<"2) Pop from stack"<<endl;
   cout<<"3) Display stack"<<endl;
   cout<<"4) Exit"<<endl;
   do {
      cout<<"Enter choice: "<<endl;
      cin>>ch;
      switch(ch) {
         case 1: {
            cout<<"Enter value to be pushed:"<<endl;
            cin>>val;
            push(val);
            break;
         }
         case 2: {
            pop();
            break;
         }
         case 3: {
            display();
            break;
         }
         case 4: {
            cout<<"Exit"<<endl;
            break;
         }
         default: {
            cout<<"Invalid Choice"<<endl;
         }
      }
   }while(ch!=4);
   return 0;
}
Output
1) Push in stack
2) Pop from stack
3) Display stack
4) Exit

Enter choice: 1
Enter value to be pushed: 2
Enter choice: 1
Enter value to be pushed: 6
Enter choice: 1
Enter value to be pushed: 8
Enter choice: 1
Enter value to be pushed: 7
Enter choice: 2
The popped element is 7
Enter choice: 3
Stack elements are:8 6 2
Enter choice: 5
Invalid Choice
Enter choice: 4
Exit
In the above program, the push() function takes argument val i.e. value to be pushed into the stack. If a top is greater than or equal to n, there is no space in a stack and overflow is printed. Otherwise, val is pushed into the stack. The code snippet for this is as follows.

void push(int val) {
   if(top>=n-1)
   cout<<"Stack Overflow"<<endl;
   else {
      top++;
      stack[top]=val;
   }
}
The pop() function pops the topmost value of the stack, if there is any value. If the stack is empty then underflow is printed. This is given as follows.

void pop() {
   if(top<=-1)
   cout<<"Stack Underflow"<<endl;
   else {
      cout<<"The popped element is "<< stack[top] <<endl;
      top--;
   }
}
The display() function displays all the elements in the stack. It uses a for loop to do so. If there are no elements in the stack, then Stack is empty is printed. This is given below.

void display() {
   if(top>=0) {
      cout<<"Stack elements are:";
      for(int i=top; i>=0; i--)
      cout<<stack[i]<<" ";
      cout<<endl;
   }else
   cout<<"Stack is empty";
}
The function main() provides a choice to the user if they want to push, pop or display the stack. According to the user response, the appropriate function is called using switch. If the user enters an invalid response, then that is printed. The code snippet for this is given below.

int main() {
   int ch, val;
   cout<<"1) Push in stack"<<endl;
   cout<<"2) Pop from stack"<<endl;
   cout<<"3) Display stack"<<endl;
   cout<<"4) Exit"<<endl;
   do {
      cout<<"Enter choice: "<<endl;
      cin>>ch;
      switch(ch) {
         case 1: {
            cout<<"Enter value to be pushed:"<<endl;
            cin>>val;
            push(val);
            break;
         }
         case 2: {
            pop();
            break;
         }
         case 3: {
            display();
            break;
         }
         case 4: {
            cout<<"Exit"<<endl;
            break;
         }
         default: {
            cout<<"Invalid Choice"<<endl;
         }
      }
   }while(ch!=4);
   return 0;
}<br>
	OUTPUT:<br>

