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
<br><br><br><br>
	
	
	
SINGLY LINKED LIST<br><br>
	#include<iostream><br>
#include<cstdlib> <br>
using namespace std; <br>
struct node <br>
{ <br>
 int info; <br>
 struct node *next; <br>
}*start; <br>
class single_llist <br>
{ <br>
 public: <br>
 node* create_node(int); <br>
 void insert_begin(); <br>
 void insert_last(); <br>
 void insert_pos(); <br>
 void delete_begin(); <br>
 void delete_last(); <br>
 void delete_pos(); <br>
 void update_begin(); <br>
 void update_last(); <br>
 void update_pos(); <br>
 void sort(); <br>
 void reverse(); <br>
 void search(); <br>
 void display(); <br>
 single_llist() <br>
 { <br>
 start = NULL; <br>
 } <br>
}; <br>
int main() <br>
{ <br>
 int choice; <br>
 single_llist sl,s2; <br>
 start = NULL; <br>
 do <br>
 { 
 cout<<"---------------------------------"<<endl; <br>
 cout<<"Operations on singly linked list"<<endl; <br>
 cout<<"---------------------------------"<<endl; <br>
 cout<<"1.Insert at first"<<endl; <br>
 cout<<"2.Insert at last"<<endl; <br>
 cout<<"3.Insert at position"<<endl; <br>
 cout<<"4.Delete at first"<<endl; <br>
 cout<<"5.Delete at Last"<<endl; <br>
 cout<<"6.Delete at position"<<endl; <br>
 cout<<"7.Update at first"<<endl; <br>
 cout<<"8.Update at last"<<endl; <br>
 cout<<"9.Update at position"<<endl; <br>
 cout<<"10.Ascending order"<<endl; <br>
 cout<<"11.Descending order"<<endl; <br>
 cout<<"12.Search"<<endl; <br>
 cout<<"13.Display"<<endl; <br>
 cout<<"14.Exit "<<endl; <br>
 cout<<"Enter your choice :"; <br>
 cin>>choice; <br>
 switch(choice) <br>
 { <br>
 case 1: sl.insert_begin(); <br>
 sl.display(); <br>
 break; <br>
 case 2: sl.insert_last(); <br>
 sl.display(); <br>
 break; <br>
 case 3: sl.insert_pos(); <br>
 sl.display(); <br>
 break; <br>
 case 4: s2.delete_begin(); <br>
 sl.display(); <br>
 break; <br>
 case 5: s2.delete_last(); <br>
 sl.display(); <br>
 break; <br>
 case 6: sl.delete_pos(); <br>
 sl.display(); <br>
 break; <br>
 case 7: sl.update_begin(); <br>
 sl.display(); <br>
 break; <br>
 case 8: sl.update_last(); <br>
 sl.display(); <br>
 break; <br>
 case 9: sl.update_pos(); <br>
 sl.display(); <br>
 break; <br>
 case 10:sl.sort(); <br>
 sl.display(); <br>
 break; <br>
 case 11:sl.reverse();<br> 
 sl.display(); <br>
 break; <br>
 case 12:sl.search(); <br>
 sl.display();<br> 
 break; <br>
 case 13:sl.display(); <br>
 break; <br>
 case 14:exit(0); <br>
 break; <br>
 default:cout<<"Wrong choice...???"<<endl; <br>
 break; <br>
 } <br>
 } <br>
 while(choice != 14); <br>
} <br>
node *single_llist::create_node(int value) <br>
{ <br>
 struct node *temp, *s; <br>
 temp = new(struct node); <br>
 if (temp == NULL) <br>
 { <br>
 cout<<"Memory not allocated"<<endl;<br> 
 return 0; <br>
 } <br>
 else <br>
 { <br>
 temp->info = value; <br>
 temp->next = NULL; <br>
 return temp; <br>
 } <br>
} <br>
void single_llist::insert_begin() <br>
{ <br>
 int value; <br>
 cout<<"Enter the value to be inserted : "; <br>
 cin>>value; <br>
 struct node *temp, *s; <br>
 temp = create_node(value); <br>
 if (start == NULL) <br>
 { <br>
 start = temp; <br>
 start->next = NULL;<br> 
 cout<<temp->info<<" is inserted at first in the empty list"<<endl; <br>
 } <br>
 else <br>
 { <br>
 s = start; <br>
 start = temp; <br>
 start->next = s; <br>
 cout<<temp->info<<" is inserted at first"<<endl; <br>
 } <br>
} <br>
void single_llist::insert_last() <br>
{ <br>
 int value; <br>
 cout<<"Enter the value to be inserted : "; <br>
 cin>>value; <br>
 struct node *temp, *s; <br>
 temp = create_node(value); <br>
 if (start == NULL) <br>
 { <br>
 start = temp; <br>
 start->next = NULL;<br> 
 cout<<temp->info<<" is inserted at last in the empty list"<<endl; <br>
 } <br>
 else <br>
 { <br>
 s = start; <br>
 while (s->next != NULL) <br>
 { <br>
 s = s->next; <br>
 } <br>
 temp->next = NULL; <br>
 s->next = temp; <br>
 cout<<temp->info<<" is inserted at last"<<endl; <br>
 } <br>
} <br>
void single_llist::insert_pos() <br>
{ <br>
 int value, pos, counter = 0, loc = 1; <br>
 struct node *temp, *s, *ptr; <br>
 s = start; <br>
 while (s != NULL) <br>
 { <br>
 s = s->next; <br>
 counter++; <br>
 } <br>
 if (counter == 0){} <br>
 else <br>
 { <br>
 cout<<"Enter the postion from "<<loc<<" to "<<counter+1<<" : "; <br>
 cin>>pos; <br>
 s = start; <br>
 if(pos == 1) <br>
 { <br>
 cout<<"Enter the value to be inserted : "; <br>
 cin>>value; <br>
 temp = create_node(value); <br>
 start = temp; <br>
 start->next = s; <br>
 cout<<temp->info<<" is inserted at first"<<endl;<br> 
 } <br>
 else if (pos > 1 && pos <= counter) <br>
 { <br>
 cout<<"Enter the value to be inserted : ";<br> 
 cin>>value; <br>
 temp = create_node(value); <br>
 for (int i = 1; i < pos; i++) <br>
 { <br>
 ptr = s; <br>
 s = s->next; <br>
 } <br>
 ptr->next = temp; <br>
 temp->next = s; <br>
 cout<<temp->info<<" is inserted at position "<<pos<<endl; <br>
 } <br>
 else if (pos == counter+1) <br>
 { <br>
 cout<<"Enter the value to be inserted : "; <br>
 cin>>value; <br>
 temp = create_node(value); <br>
 while (s->next != NULL) <br>
 { <br>
 s = s->next; <br>
 } <br>
 temp->next = NULL; <br>
 s->next = temp; <br>
 cout<<temp->info<<" is inserted at last"<<endl; <br>
 } <br>
 else <br>
 { <br>
 cout<<"Positon out of range...!!!"<<endl; <br>
 } <br>
 } <br>
} <br>
void single_llist::delete_begin() <br>
{ <br>
 if (start == NULL){} <br>
 else <br>
 { <br>
 struct node *s, *ptr; <br>
 s = start; <br>
 start = s->next;<br> 
 cout<<s->info<<" deleted from first"<<endl; <br>
 free(s); <br>
 } <br>
} <br>
void single_llist::delete_last()<br> 
{ <br>
 int i, counter = 0; <br>
 struct node *s, *ptr;<br> 
 if (start == NULL){} <br>
 else <br>
 { <br>
 s = start; <br>
 while (s != NULL) <br>
 { <br>
 s = s->next; <br>
 counter++; <br>
 } <br>
 s = start; <br>
 if (counter == 1) <br>
 { <br>
 start = s->next; <br>
 cout<<s->info<<" deleted from last"<<endl; <br>
 free(s); <br>
 } <br>
 else <br>
 { <br>
 for (i = 1;i < counter;i++) <br>
 { <br>
 ptr = s; <br>
 s = s->next; <br>
 } <br>
 ptr->next = s->next; <br>
 cout<<s->info<<" deleted from last"<<endl; <br>
 free(s); <br>
 } <br>
 } <br>
} <br>
void single_llist::delete_pos() <br>
{ <br>
 int pos, i, counter = 0, loc = 1; <br>
 struct node *s, *ptr; <br>
 s = start; <br>
 while (s != NULL) <br>
 { <br>
 s = s->next; <br>
 counter++; <br>
 } <br>
 if (counter == 0){} <br>
 else <br>
 { <br>
 if (counter == 1) <br>
 { <br>
 cout<<"Enter the postion [ SAY "<<loc<<" ] : "; <br>
 cin>>pos; <br>
 s = start; <br>
 if (pos == 1) <br>
 { <br>
 start = s->next; <br>
 cout<<s->info<<" deleted from first"<<endl; <br>
 free(s); <br>
 } <br>
 else <br>
 cout<<"Position out of range...!!!"<<endl; <br>
 } <br>
 else <br>
 { <br>
 cout<<"Enter the postion from "<<loc<<" to "<<counter<<" : "; <br>
 cin>>pos; <br>
 s = start; <br>
 if (pos == 1) <br>
 { <br>
 start = s->next; <br>
 cout<<s->info<<" deleted from first"<<endl; <br>
 free(s);<br>
 } <br>
 else if (pos > 1 && pos <= counter) <br>
 { <br>
 for (i = 1;i < pos;i++)<br> 
 { <br>
 ptr = s; <br>
 s = s->next; <br>
 } <br>
 ptr->next = s->next; <br>
 if(pos == counter) <br>
 {cout<<s->info<<" deleted from last"<<endl;<br> 
 free(s);} <br>
 else <br>
 {cout<<s->info<<" deleted from postion "<<pos<<endl; <br>
 free(s);} <br>
 } <br>
 else<br> 
 cout<<"Position out of range...!!!"<<endl; <br>
 } <br>
 } <br>
} <br>
void single_llist::update_begin() <br>
{ <br>
 int value, pos=1, i,counter = 0; <br>
 struct node *s, *ptr; <br>
 s = start; <br>
 while (s != NULL) <br>
 { <br>
 s = s->next; <br>
 counter++; <br>
 } <br>
 if (counter == 0){} <br>
 else if (pos == 1) <br>
 { <br>
 cout<<"Enter the new node : "; <br>
 cin>>value; <br>
 start->info = value; <br>
 cout<<"Node updated at first position : "<<pos<<" = "<<start->info<<endl; <br>
 } <br>
} <br>
void single_llist::update_last() <br>
{ <br>
 int value, pos, i,counter = 0; <br>
 struct node *s, *ptr; <br>
 s = start; <br>
 while (s != NULL) <br>
 { <br>
 s = s->next; <br>
 counter++; <br>
 } <br>
 s=start; <br>
 if (counter == 0){} <br>
 else <br>
 { <br>
 cout<<"Enter the new node : "; <br>
 cin>>value; <br>
 for (i = 1; i < counter ; i++) <br>
 { <br>
 s = s->next; <br>
 } <br>
 s->info = value; <br>
 cout<<"Node updated at last position : "<<counter<<" = "<<s->info<<endl; <br>
 } <br>
} <br>
void single_llist::update_pos() <br>
{ <br>
 int value, pos, i,counter = 0, loc = 1; <br>
 struct node *s, *ptr; <br>
 s = start; <br>
 while (s != NULL) <br>
 { <br>
 s = s->next; <br>
 counter++; <br>
 } <br>
 if (counter == 0){} <br>
 else <br>
 { <br>
 if (counter == 1) <br>
 { <br>
 cout<<"Enter the postion [ SAY "<<loc<<" ] : "; <br>
 cin>>pos; <br>
 s = start; <br>
 if (pos == 1) <br>
 { <br>
 cout<<"Enter the new node : "; <br>
 cin>>value; <br>
 start->info = value; <br>
 cout<<"Node updated at position : "<<pos<<" = "<<start->info<<endl; <br>
 } <br>
 else <br>
 cout<<"Position out of range...!!!"<<endl; <br>
 } <br>
 else <br>
 { <br>
 cout<<"Enter the postion from "<<loc<<" to "<<counter<<" : "; <br>
 cin>>pos; <br>
 s = start; <br>
 if (pos == 1) <br>
 { <br>
 cout<<"Enter the new node : "; <br>
 cin>>value; <br>
 start->info = value; <br>
 cout<<"Node updated at position : "<<pos<<" = "<<start->info<<endl; <br>
 } <br>
 else if (pos > 1 && pos <= counter) <br>
 { <br>
 cout<<"Enter the new node : "; <br>
 cin>>value; <br>
 for (i = 1; i < pos ; i++) <br>
 { <br>
 s = s->next; <br>
 } <br>
 s->info = value; <br>
 cout<<"Node updated at position : "<<pos<<" = "<<s->info<<endl; <br>
 } <br>
 else <br>
 cout<<"Position out of range...!!!"<<endl; <br>
 } <br>
 } <br>
} <br>
void single_llist::sort() <br>
{ <br>
 struct node *ptr, *s; <br>
 int value;<br> 
 if (start == NULL){} <br>
 else <br>
 { <br>
 ptr = start; <br>
 while (ptr != NULL) <br>
 { <br>
 for (s = ptr->next;s !=NULL;s = s->next) <br>
 { <br>
 if (ptr->info > s->info) <br>
 { <br>
 value = ptr->info; <br>
 ptr->info = s->info; <br>
 s->info = value; <br>
 } <br>
 } <br>
 ptr = ptr->next; <br>
 } <br>
 } <br>
} <br>
void single_llist::reverse() <br>
{ <br>
 struct node *ptr, *s; <br>
 int value; <br>
 if (start == NULL){} <br>
 else <br>
 { <br>
 ptr = start; <br>
 while (ptr != NULL) <br>
 { <br>
 for (s = ptr->next;s !=NULL;s = s->next) <br>
 { <br>
 if (ptr->info < s->info) <br>
 { <br>
 value = ptr->info; <br>
 ptr->info = s->info; <br>
 s->info = value; <br>
 } <br>
 } <br>
 ptr = ptr->next; <br>
 } <br>
 } <br>
} <br>
void single_llist::search() <br>
{ <br>
 int value, loc = 0, pos = 0, counter = 0; <br>
 struct node *s; <br>
 s = start; <br>
 while (s != NULL) <br>
 { <br>
 s = s->next; <br>
 counter++; <br>
 } <br>
 if (start == NULL){} <br>
 else <br>
 { <br>
 cout<<"Enter the value to be searched : "; <br>
 cin>>value; <br>
 struct node *s; <br>
 s = start; <br>
 while (s != NULL) <br>
 { <br>
 pos++; <br>
 if (s->info == value) <br>
 { <br>
 loc++; <br>
 if(loc == 1) <br>
 cout<<"Element "<<value<<" is found at position "<<pos; <br>
 else if(loc <= counter) <br>
 cout<<" , "<<pos; <br>
 } <br>
 s = s->next; <br>
 } <br>
 cout<<endl; <br>
 if (loc == 0) <br>
 cout<<"Element "<<value<<" not found in the list"<<endl; <br>
 } <br>
} <br>
void single_llist::display() <br>
{ <br>
 struct node *temp; <br>
 if (start == NULL) <br>
 cout<<"Linked list is empty...!!!"<<endl; <br>
 else <br>
 { <br>
 cout<<"Linked list contains : "; <br>
 temp = start; <br>
 while (temp != NULL) <br>
 { <br>
 cout<<temp->info<<" "; <br>
 temp = temp->next; <br>
 } <br>
 cout<<endl; <br>
 } <br>
}<br>
OUTPUT:<br>
	![image](https://user-images.githubusercontent.com/98145023/152730730-90821375-b1c0-4e3d-ace8-32c872230415.png)<br>
	![image](https://user-images.githubusercontent.com/98145023/152730852-cdca1412-6792-406f-840d-4abcdafa1981.png)<br>
	![image](https://user-images.githubusercontent.com/98145023/152731107-2f3728b2-fe7b-445e-88f9-4d7a173bd488.png)<br>
	![image](https://user-images.githubusercontent.com/98145023/152731257-92bdc871-2889-48cb-862d-3a32fd6837d9.png)<br>
	![image](https://user-images.githubusercontent.com/98145023/152731411-8549d63b-3633-4708-9ee2-8cebe50a6a75.png)<br><br><br>
	
	
	
Write a C++ program to split the given linked list in such a way that the given element's position should be the first node of second list<br>
#include<iostream><br>
using namespace std;<br>
struct Node <br>
{<br>
	int value;<br>
	struct Node *next;<br>
};<br>
struct Node* head=NULL;<br>
struct Node* sHead=NULL;<br>
struct Node* temp=NULL;<br>
void insert(int new_data)<br>
{<br>
	struct Node* new_node = new Node();<br>
	new_node->value = new_data;<br>
	new_node->next = head;<br>
	head = new_node;<br>
}<br>
int n;<br>
int ele;<br>
int splitlndex;<br>
int main()<br>
{<br>
	int i;<br>
	cout<<"Enter number of elements you want in the list\t";<br>
	cin>>n;<br>
	cout<<"Enter elements:"<<endl;<br>
	for(i=0;i<n;i++)<br>
	{<br>
	     cin>>ele;<br>
	     insert(ele);<br>
	}<br>
	cout<<"\nList of elements:"<<endl;<br>
	Node *t;<br>
	t=head;<br>
	while(t!=NULL)<br>
	{<br>
	 cout<<t->value<<"\t";<br>
		t=t->next;<br>
	}<br>
	cout<<"\n\nEnter the element you want the list to split";<br>
	cin>>splitlndex;<br>
	while(splitlndex<0||splitlndex>n-1)<br>
	{<br>
		cout<<"Invalid position.Try again."<<endl;<br>
		cin>>splitlndex;<br>
	}<br>
	temp=head;<br>
	for(i=0;i<splitlndex;i++)<br>
	{<br>
		if(i==splitlndex-1)<br>
		{<br>
	                Node *tN;<br>
			tN=temp->next;<br>
			sHead=tN;<br>
			temp->next=NULL;<br>
			break;<br>
		}<br>
		temp=temp->next;<br>
	}<br>
	temp=head;<br>
	if(temp==NULL)<br>
	{<br>
		cout<<"\n First list is empty"<<endl;<br>
	}<br>
	else<br>
	{<br>
		cout<<"\n\nFirst list element"<<endl;<br>
		while(temp!=NULL)<br>
		{<br>
			cout<<temp->value<<"\t";<br>
			temp=temp->next;<br>
		}<br>
	}<br>
	temp=sHead;<br>
	if(temp==NULL)<br>
	{<br>
		cout<<"\nSecond list is empty"<<endl;<br>
	}<br>
	else<br>
	{<br>
		cout<<"\n\nSecond list elements"<<endl;<br>
		while(temp!=NULL)<br>
		{<br>
			cout<<temp->value<<"\t";<br>
			temp=temp->next;<br>
		}<br>
	}<br>
	return 0;<br>
}<br><br>
![image](https://user-images.githubusercontent.com/98145023/155084172-a54e22ea-eef5-4671-8706-6b78008d5517.png)<br><br><br>
	
	
	#include<iostream><br>
	using namespace std;<br>
	struct node<br>
	{<br>
   int data;<br>
   struct node *left;<br>
   struct node *right;<br>
};<br>
struct node *createNode(int val)
 {<br>
   struct node *temp = (struct node *)malloc(sizeof(struct node));<br>
   temp->data = val;<br>
   temp->left = temp->right = NULL;<br>
   return temp;<br>
}<br>
void inorder(struct node *root)<br>
 {<br>
   if (root != NULL) <br>
   {<br>
      inorder(root->left);<br>
      cout<<root->data<<" ";<br>
      inorder(root->right);<br>
   }<br>
}<br>
struct node* insertNode(struct node* node, int val)<br>
 {<br>
   if (node == NULL) return createNode(val);<br>
   if (val < node->data)<br>
   node->left = insertNode(node->left, val);<br>
   else if (val > node->data)<br>
   node->right = insertNode(node->right, val);<br>
   return node;<br>
}<br>
int main() <br>
{<br>
   struct node *root = NULL;<br>
   root = insertNode(root, 7);<br>
   insertNode(root, 90);<br>
   insertNode(root, 100);<br>
   insertNode(root, 10);<br>
   insertNode(root, 20);<br>
   insertNode(root, 18);<br>
   insertNode(root, 200);<br>
   insertNode(root, 150);<br>
   cout<<"In-Order traversal of the Binary Search Tree is: ";<br>
   inorder(root);<br>
   return 0;<br>
}<br>
![image](https://user-images.githubusercontent.com/98145023/155083678-8ad9d5ea-e6fd-4af3-9efc-8e84b3bc4f01.png)<br><br><br>


8.Write a program to store k keys into an array of size n at the location compute using a hash function, loc=key%n, where k<=n and key takes values from [1 to m], m>n.
Handle the collision using Linear Probing technique.<br>

#include<iostream> <br>
#include<limits.h> <br>
using namespace std; <br>
void Insert(int ary[],int hFn, int Size) <br>
{ <br>
int element,pos,n=0; <br>
cout<<"Enter key element to insert\n"; <br>
cin>>element; <br>
pos = element%hFn; <br>
while(ary[pos]!= INT_MIN) <br>
{ <br>
if(ary[pos]== INT_MAX) <br>
break; <br>
pos = (pos+1)%hFn; <br>
n++; <br>
if(n==Size) <br>
break; <br>
} <br>
if(n==Size) <br>
cout<<"Hash table was full of elements\nNo Place to insert this element\n\n"; <br>
else <br>
ary[pos] = element; <br>
} <br>
void display(int ary[],int Size)<br>
{ <br>
int i; <br>
cout<<"Index\tValue\n"; <br>
for(i=0;i<Size;i++) <br>
cout<<i<<"\t"<<ary[i]<<"\n"; <br>
} <br>
int main() <br>
{ <br>
int Size,hFn,i,choice; <br>
cout<<"Enter size of hash table\n"; <br>
cin>>Size; <br>
hFn=Size; <br>
int ary[Size]; <br>
for(i=0;i<Size;i++) <br>
ary[i]=INT_MIN; <br>
do <br>
{ <br>
cout<<"Enter your choice\n";<br> 
cout<<" 1-> Insert\n 2-> Display\n 0-> Exit\n"; <br>
cin>>choice; <br>
switch(choice)<br> 
{ <br>
case 1: Insert(ary,hFn,Size); <br>
break; <br>
case 2: display(ary,Size); <br>
break;<br> 
default: cout<<"Enter correct choice\n"; <br>
break;<br>
}<br>
}<br>
while(choice);<br>
return 0;<br>
}<br>
OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98145023/155932060-7dbcc60c-be65-4259-a926-285a9df82d1a.png)
![image](https://user-images.githubusercontent.com/98145023/155932226-50289bde-e42c-45fe-9b60-d83f45f2ac0e.png)<br><br><br>


C++ proagrm to implement doubly linked list.<br>
#include <iostream><br>
using namespace std;<br>
struct Node <br>
{<br>
   int data;<br>
   struct Node *prev;<br>
   struct Node *next;<br>
};<br>
struct Node* head = NULL;<br>
void insert(int newdata)<br> 
{<br>
   struct Node* newnode = (struct Node*) malloc(sizeof(struct Node));<br>
   newnode->data = newdata;<br>
   newnode->prev = NULL;<br>
   newnode->next = head;<br>
   if(head != NULL)<br>
   head->prev = newnode ;<br>
   head = newnode;<br>
}<br>
void display() <br>
{<br>
   struct Node* ptr;<br>
   ptr = head;<br>
   while(ptr != NULL) <br>
   {<br>
      cout<< ptr->data <<" ";<br>
      ptr = ptr->next;<br>
   }<br>
}<br>
int main() <br>
{<br>
   insert(3);<br>
   insert(1);<br>
   insert(7);<br>
   insert(2);<br>
   insert(9);<br>
   cout<<"The doubly linked list is: ";<br>
   display();<br>
   return 0;<br>
}<br>
OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98145023/155934148-fc606d97-e4c9-4e18-920e-a1ce6adfb590.png)<br><br><br>

 Write C++ program for implementing the Heap Sort technique.<br>
#include <iostream><br>
using namespace std;<br>
void MaxHeapify (int a[], int i, int n)<br>
{<br>
int j, temp;<br>
temp = a[i];<br>
j = 2*i;<br>
while (j <= n)<br>
{<br>
if (j < n && a[j+1] > a[j])<br>
j = j+1;<br>
if (temp > a[j])<br>
break;<br>
else if (temp <= a[j])<br>
{<br>
a[j/2] = a[j];<br>
j = 2*j;<br>
}<br>
}<br>
a[j/2] = temp;<br>
return;<br>
}<br>
void HeapSort(int a[], int n)<br>
{<br>
int i, temp;<br>
for (i = n; i >= 2; i--)<br>
{<br>
temp = a[i];<br>
a[i] = a[1];<br>
a[1] = temp;<br>
MaxHeapify(a, 1, i - 1);<br>
}<br>
}<br>
void Build_MaxHeap(int a[], int n)<br>
{<br>
int i;<br>
for(i = n/2; i >= 1; i--)<br>
MaxHeapify(a, i, n);<br>
}<br>
int main()<br>
{<br>
int n, i,arr[100];<br>
cout<<"\nEnter the number of data element to be sorted: ";<br>
cin>>n;<br>
n++;<br>
for(i=1;i<n;i++)<br>
{<br>
cout<<"Enter element"<<i<<":";<br>
cin>>arr[i];<br>
}<br>
Build_MaxHeap(arr, n-1);<br>
HeapSort(arr, n-1);<br>
cout<<"\nSorted Data ";<br>
for (i = 1; i < n; i++)<br>
cout<<" "<<arr[i];<br>
return 0;<br>
}<br>
OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98145023/155941514-8fec0d75-8d3a-420d-b1af-178ed59a1cc3.png)<br><br><br>


Write  C++ program to implement sum of subsets using backtracking.<br>
#include<iostream><br>
using namespace std;<br>
int s[10],d,n,set[10],count=0;<br>
void display(int);<br>
int flag = 0;<br>
int main()<br>
{<br>
 int subset(int,int);<br>
 int i;<br>
 cout<<"ENTER THE NUMBER OF THE ELEMENTS IN THE SET : ";<br>
 cin>>n;<br>
 cout<<"ENTER THE SET OF VALUES : ";<br>
 	for(i=0;i<n;i++)<br>
   		cin>>s[i];<br>
 cout<<"ENTER THE VALUE : ";<br>
 	cin>>d;<br>
 cout<<"THE PROGRAM OUTPUT IS: ";<br>
 	subset(0 , 0);<br>
 if(flag == 0)<br>
 cout<<"There is no solution";<br>
 }<br>
 int subset(int sum,int i)<br>
{<br>
if(sum == d)<br>
 {<br>
 flag = 1;<br>
 display(count);<br>
 return 0;<br>
 }<br>
if(sum>d || i>=n)<br>
return 1;<br>
else<br>
  {<br>
 set[count]=s[i];<br>
 count++;<br>
 subset(sum+s[i],i+1);<br>
 count--;<br>
 subset(sum,i+1);<br>
  }<br>
}<br>
void display(int count)<br>
{<br>
 int i;<br>
 cout<<"\t{";<br>
 for(i=0;i<count;i++)<br>
 cout<<set[i];<br>
 cout<<"}";<br>
}<br>
OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98145023/157187457-4bab5320-9f61-483c-a54a-ffa5f36cf167.png)<br><br><br>

	
	
#include<iostream><br>
#include<cstdio><br>
#include<sstream><br>
#include<algorithm><br>
#define pow2(n) (1 << (n))<br>
using namespace std;<br>
struct avl<br>
 {<br>

  int d;<br>

  struct avl *l;<br>

  struct avl *r;<br>
}*r;<br>
class avl_tree {<br>
public:<br>
int height(avl *);<br>
int difference(avl *);<br>
avl *rr_rotat(avl *);<br>
      avl *ll_rotat(avl *);<br>
      avl *lr_rotat(avl*);<br>
      avl *rl_rotat(avl *);<br>
      avl * balance(avl *);<br>
      avl * insert(avl*, int);<br>
      void show(avl*, int);<br>
      void inorder(avl *);<br>
      void preorder(avl *);<br>
      void postorder(avl*);<br>
      avl_tree()<br> {<br>
         r = NULL;<br>
      }<br>
};<br>
int avl_tree::height(avl *t) {<br>
   int h = 0;<br>
   if (t != NULL)<br> {<br>
      int l_height = height(t->l);<br>
      int r_height = height(t->r);<br>
      int max_height = max(l_height, r_height);<br>
      h = max_height + 1;<br>
   }<br>
   return h;<br>
}<br>
int avl_tree::difference(avl *t)<br> {<br>
   int l_height = height(t->l);<br>
   int r_height = height(t->r);<br>
   int b_factor = l_height - r_height;<br>
   return b_factor;<br>
}<br>
avl *avl_tree::rr_rotat(avl *parent)<br> {<br>
   avl *t;<br>
   t = parent->r;<br>
   parent->r = t->l;<br>
   t->l = parent;<br>
   cout<<"Right-Right Rotation";<br>
   return t;<br>
}<br>
avl *avl_tree::ll_rotat(avl *parent)<br> {<br>
   avl *t;<br>
   t = parent->l;<br>
   parent->l = t->r;<br>
   t->r = parent;<br>
   cout<<"Left-Left Rotation";<br>
   return t;<br>
}<br>
avl *avl_tree::lr_rotat(avl *parent)<br> {<br>
   avl *t;<br>
   t = parent->l;<br>
   parent->l = rr_rotat(t);<br>
   cout<<"Left-Right Rotation";<br>
   return ll_rotat(parent);<br>
}<br>
avl *avl_tree::rl_rotat(avl *parent)<br> {<br>
   avl *t;<br>
   t = parent->r;
   parent->r = ll_rotat(t);<br>
   cout<<"Right-Left Rotation";<br>
   return rr_rotat(parent);<br>
}<br>
avl *avl_tree::balance(avl *t)<br> {<br>
   int bal_factor = difference(t);<br>
   if (bal_factor > 1)<br> {<br>
      if (difference(t->l) > 0)<br>
         t = ll_rotat(t);<br>
      else<br>
         t = lr_rotat(t);<br>
   } else if (bal_factor < -1)<br> {<br>
      if (difference(t->r) > 0)<br>
         t = rl_rotat(t);<br>
      else<br>
         t = rr_rotat(t);<br>
   }<br>
   return t;<br>
}<br>
avl *avl_tree::insert(avl *r, int v)<br> {<br>
   if (r == NULL)<br> {<br>
      r = new avl;<br>
      r->d = v;<br>
      r->l = NULL;<br>
      r->r = NULL;<br>
      return r;<br>
   } <br>else if (v< r->d)<br> {<br>
      r->l = insert(r->l, v);<br>
      r = balance(r);<br>
   } else if (v >= r->d)<br> {<br>
      r->r = insert(r->r, v);<br>
      r = balance(r);<br>
   }<br> return r;<br>
}<br>
void avl_tree::show(avl *p, int l)<br> {<br>
   int i;<br>
   if (p != NULL)<br> {<br>
      show(p->r, l+ 1);<br>
      cout<<" ";<br>
      if (p == r)<br>
         cout << "Root -> ";<br>
      for (i = 0; i < l&& p != r; i++)<br>
         cout << " ";<br>
         cout << p->d;<br>
         show(p->l, l + 1);<br>
   }<br>
}<br>
void avl_tree::inorder(avl *t)<br> {<br>
   if (t == NULL)<br>
      return;<br>
      inorder(t->l);<br>
      cout << t->d << " ";<br>
      inorder(t->r);<br>
}<br>
void avl_tree::preorder(avl *t)<br> {<br>
   if (t == NULL)<br>
      return;<br>
      cout << t->d << " ";<br>
      preorder(t->l);<br>
      preorder(t->r);<br>
}<br>
void avl_tree::postorder(avl *t)<br> {<br>
   if (t == NULL)<br>
      return;<br>
      postorder(t ->l);<br>
      postorder(t ->r);<br>
      cout << t->d << " ";<br>
}<br>
int main()<br> {<br>
   int c, i;<br>
   avl_tree avl;<br>
   while (1) {<br>
      cout << "1.Insert Element into the tree" << endl;<br>
      cout << "2.show Balanced AVL Tree" << endl;<br>
      cout << "3.InOrder traversal" << endl;<br>
      cout << "4.PreOrder traversal" << endl;<br>
      cout << "5.PostOrder traversal" << endl;<br>
      cout << "6.Exit" << endl;<br>
      cout << "Enter you<br>r Choice: ";<br>
      cin >> c;<br>
      switch (c) {<br>
         case 1:<br>
            cout << "Enter value to be inserted: ";<br>
            cin >> i;<br>
            r = avl.insert(r, i);<br>
         break;<br>
         case 2:<br>
            if (r == NULL) {<br>
               cout << "Tree is Empty" << endl;<br>
               continue;<br>
            }<br>
            cout << "Balanced AVL Tree:" << endl;<br>
            avl.show(r, 1);<br>
            cout<<endl;<br>
         break;<br>
         case 3:<br>
            cout << "Inorder Traversal:" << endl;<br>
            avl.inorder(r);<br>
            cout << endl;<br>
         break;<br>
         case 4:<br>
            cout << "Preorder Traversal:" << endl;<br>
            avl.preorder(r);<br>
            cout << endl;<br>
         break;<br>
         case 5:<br>
            cout << "Postorder Traversal:" << endl;<br>
            avl.postorder(r);<br>
            cout << endl;<br>
         break;<br>
         case 6:<br>
            exit(1);<br>
         break;<br>
         default:<br>
            cout << "Wrong Choice" << endl;<br>
      }<br>
   }<br>
   return 0;<br>
}<br><br>
OUTPUT:<br>
	![image](https://user-images.githubusercontent.com/98145023/163158944-798b2707-95bc-434a-b483-dec707dd14ea.png)<br>
        ![image](https://user-images.githubusercontent.com/98145023/163158844-e346f20b-a472-4359-aad3-dcaa035ab785.png)<br>
![image](https://user-images.githubusercontent.com/98145023/163159106-8a59050a-0632-46d5-8724-2b32cca25854.png)<br><br><br>


	
	
#include <bits/stdc++.h><br>
using namespace std;<br>
void mergeofarrays(int a[], int low, int mid, int high) {<br>
  int i = low, j = mid + 1, index = low, temp[100], k;<br>
  while ((i <= mid) && (j <= high)) {<br>
    if (a[i] < a[j]) {<br>
      temp[index] = a[i];<br>
      i++;<br>
    } else {<br>
      temp[index] = a[j];<br>
      j++;<br>
    }<br>
    index++;<br>
  }<br>
  //copy the remaining elements of right array<br>
  if (i > mid) {<br>
    while (j <= high) {<br>
      temp[index] = a[j];<br>
      j++;<br>
      index++;<br>
    }<br>
  } else //remaining elements of left array<br>
  {<br>
    while (i <= mid) {<br>
      temp[index] = a[i];<br>
      i++;<br>
      index++;<br>
    }<br>
  }<br>
  for (k = low; k < index; k++) //copying into original array<br>
  {<br>
    a[k] = temp[k];<br>
  }<br>
}<br>
void mergesort(int a[], int low, int high) {<br>
  if (low < high) {<br>
    int middle = (low + high) / 2; //calculating middle index of array to divide it in two halves<br>
    mergesort(a, low, middle); //sorting first half<br>
    mergesort(a, middle + 1, high); //sorting second half<br>
    mergeofarrays(a, low, middle, high); //merging 2 sorted halves<br>
  }<br>
}<br>
int main() {<br>
  int n = 7;<br>
  int a[100] = {54,34,23,10,98,2,3};<br>
  mergesort(a, 0, 6);<br>
  for (int i = 0; i < n; i++) {<br>
    cout << a[i] << " ";<br>
  }<br>
}<br>
OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98145023/163165229-5cd1e7fd-ed45-4f1d-96b2-cfd673255d15.png)<br><br><br>
		    

	

HASHING<br>
#include<iostream><br>
#include<limits.h> <br>
using namespace std;<br>
void Insert(int ary[],int hFn, int Size)<br>
	{ <br>
 int element,pos,n=0; <br>
cout<<"Enter key element to insert\n";<br>
cin>>element;<br>
pos = element%hFn; <br>
while(ary[pos]!= INT_MIN)<br>
	{ <br>
if(ary[pos]== INT_MAX)<br>
 break; <br>
pos = (pos+1)%hFn; <br>
n++;<br>
if(n==Size)<br>
 break; <br>
} <br>
if(n==Size)<br>
 cout<<"Hash table was full of elements\nNo Place to insert this element\n\n";<br> 
else<br>
 ary[pos] = element; <br>
} <br>
void display(int ary[],int Size)<br>
	{ <br>
int i;<br>
 <br>cout<<"Index\tValue\n";<br>
for(i=0;i<Size;i++)<br>
 cout<<i<<"\t"<<ary[i]<<"\n"; <br>
} <br>
int main(){<br>
int Size,hFn,i,choice; <br>
cout<<"Enter size of hash table\n";<br>
cin>>Size;<br>
hFn=Size;<br>
int ary[Size];<br>
for(i=0;i<Size;i++)<br>
 ary[i]=INT_MIN; <br>
do{ <br>
cout<<"Enter your choice\n"; <br>
cout<<" 1-> Insert\n 2-> Display\n 0-> Exit\n";<br>
cin>>choice;<br>
switch(choice){<br>
case 1:<br>
Insert(ary,hFn,Size);<br>
break; <br>
case 2:<br>
display(ary,Size);<br>
break; <br>
default:<br><br>
cout<<"Enter correct choice\n";<br>
break;<br> 
} <br>
}while(choice);<br>
return 0;<br>
}<br>
OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98145023/163770441-45230300-4d83-4a8c-ba79-50d7d42b8aa6.png)<br>
![image](https://user-images.githubusercontent.com/98145023/163770339-c97624e6-bc5e-4f1f-8b39-8393a7d6e54d.png)<br><br><br>
	

	
Nqueen<br>	
//program to solve the n queen problem <br><br>
//grid[][] is represent the 2-d array with value(0 and 1) for grid[i][j]=1 means queen i are placed at j column.<br>
//we can take any number of queen , for this time we take the atmost 10 queen (grid[10][10]).<br>
#include<iostream><br>
using namespace std;<br>
int grid[100][100];<br>
//print the solution<br>
void print(int n) <br>
{<br>
    for (int i = 0;i <= n-1; i++) <br>
	{<br>
        for (int j = 0;j <= n-1; j++) <br>
		{<br>
            cout <<grid[i][j]<< " ";<br>
             }<br>
        cout<<endl;<br>
    }<br>
    cout<<endl;<br>
    cout<<endl;<br>
}<br>
//function for check the position is safe or not<br>
//row is indicates the queen no. and col represents the possible positions<br>
bool isSafe(int col, int row, int n) <br>
{<br>
  //check for same column<br>
	 for (int i = 0; i < row; i++) <br>
	{<br>
        if (grid[i][col]) <br>
		{<br>
            return false;<br>
        }<br>
    }<br>
    //check for upper left diagonal<br>
    for (int i = row,j = col;i >= 0 && j >= 0; i--,j--) <br>
	{<br>
        if (grid[i][j]) <br>
		{<br>
            return false;<br>
        }<br>
    }<br>
    //check for upper right diagonal<br>
    for (int i = row, j = col; i >= 0 && j < n; j++, i--) <br>
	{<br>
        if (grid[i][j]) <br>
		{<br>
            return false;<br>
        }<br>
    }<br>
    return true;<br>
}<br>
//function to find the position for each queen<br>
//row is indicates the queen no. and col represents the possible positions<br>
bool solve (int n, int row)<br> 
{<br>
    if (n == row) <br>
	{<br>
        print(n);<br>
        return true;<br>
    }<br>
    //variable res is use for possible backtracking <br>
    bool res = false;<br>
    for (int i = 0;i <=n-1;i++) <br>
	{<br>
        if (isSafe(i, row, n)) <br>
		{<br>
            grid[row][i] = 1;<br>
            //recursive call solve(n, row+1) for next queen (row+1)<br>
            res = solve(n, row+1) || res;//if res ==false then backtracking will occur <br>
            //by assigning the grid[row][i] = 0<br>
            grid[row][i] = 0;<br>
        }<br>
    }<br>
    return res;<br>
}<br>
int main()<br>
{<br>
  int n;<br>
        cout<<"Enter the number of queen"<<endl;<br>
        cin >> n;<br>
        for (int i = 0;i < n;i++)<br> {<br>
            for (int j = 0;j < n;j++) <br>{<br>
                grid[i][j] = 0;<br>
            }<br>
        }<br>
        bool res = solve(n, 0);<br>
        if(res == false)<br> {<br>
            cout << "No solution"<< endl; //if there is no possible solution<br>
        }<br> else<br> {<br>
            cout << endl;<br>
        }<br>
  return 0;<br>
}<br>
OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98145023/163946845-85e2b035-de15-456b-84f1-b8d9866ff94c.png)<br>
![image](https://user-images.githubusercontent.com/98145023/163946993-b2eedb4b-5303-4830-be9b-6ca6da2d2102.png)<br><br><br>
	
	
	
DOUBLY LINKED LIST<br>
	/*<br>
 * C++ Program to Implement Doubly Linked List <br>
 */<br>
#include<iostream><br>
#include<cstdio><br>
#include<cstdlib><br>
/*<br>
 * Node Declaration<br>
 */<br>
using namespace std;<br>
struct node<br>
{<br>
    int info;<br>
    struct node *next;<br>
    struct node *prev;<br>
}*start;<br>
 
/*<br>
 Class Declaration <br>
 */<br>
class double_llist<br>
{<br>
    public:<br>
        void create_list(int value);<br>
        void add_begin(int value);<br>
        void add_after(int value, int position);<br>
        void delete_element(int value);<br>
        void search_element(int value);<br>
        void display_dlist();<br>
        void count();<br>
        void reverse();<br>
        double_llist()<br>
        {<br>
            start = NULL;  <br>
        }<br>
};<br>
 
/*<br>
 * Main: Conatins Menu<br>
 */<br>
int main()<br>
{<br>
    int choice, element, position;<br>
    double_llist dl;<br>
    while (1)<br>
    {<br>
        cout<<endl<<"----------------------------"<<endl;<br>
        cout<<endl<<"Operations on Doubly linked list"<<endl;<br>
        cout<<endl<<"----------------------------"<<endl; <br>        
        cout<<"1.Create Node"<<endl;<br>
        cout<<"2.Add at begining"<<endl;<br>
        cout<<"3.Add after position"<<endl;<br>
        cout<<"4.Delete"<<endl;<br>
        cout<<"5.Display"<<endl;<br>
        cout<<"6.Count"<<endl;<br>
        cout<<"7.Reverse"<<endl;<br>
        cout<<"8.Quit"<<endl;<br>
        cout<<"Enter your choice : ";<br>
        cin>>choice;<br>
        switch ( choice )<br>
        {<br>
        case 1:<br>
            cout<<"Enter the element: ";<br>
            cin>>element;<br>
            dl.create_list(element);<br>
            cout<<endl;<br>
            break;<br>
        case 2:<br>
            cout<<"Enter the element: ";<br>
            cin>>element;<br>
            dl.add_begin(element);<br>
            cout<<endl;<br>
            break;<br>
        case 3:<br>
            cout<<"Enter the element: ";<br>
            cin>>element;<br>
            cout<<"Insert Element after postion: ";<br>
            cin>>position;<br>
            dl.add_after(element, position);<br>
            cout<<endl;<br>
            break;<br>
        case 4:<br>
            if (start == NULL)<br>
            {               <br>       
                cout<<"List empty,nothing to delete"<<endl; <br>  
                break;<br>
            }<br>
            cout<<"Enter the element for deletion: ";<br>
            cin>>element;<br>
            dl.delete_element(element);<br>
            cout<<endl;<br>
            break;<br>
        case 5:<br>
            dl.display_dlist();<br>
            cout<<endl;<br>
            break;<br>
        case 6:<br>
            dl.count();<br>
            break;    <br>
        case 7:<br>
            if (start == NULL)<br>
            {<br>
                cout<<"List empty,nothing to reverse"<<endl;<br>
                break;<br>
            }<br>
            dl.reverse();<br>
            cout<<endl;<br>
            break;<br>
        case 8:<br>
            exit(1);<br>
        default:<br><br>
            cout<<"Wrong choice"<<endl;<br>
        }<br>
    }<br>
    return 0;<br>
}<br>
 
/*<br>
 * Create Double Link List<br>
 */<br>
void double_llist::create_list(int value)<br>
{<br>
    struct node *s, *temp;<br>
    temp = new(struct node); <br>
    temp->info = value;<br>
    temp->next = NULL;<br>
    if (start == NULL)<br>
    {
        temp->prev = NULL;<br>
        start = temp;<br>
    }<br>
    else<br>
    {<br>
        s = start;<br>
        while (s->next != NULL)<br>
            s = s->next;<br>
        s->next = temp;<br>
        temp->prev = s;<br>
    }<br>
}<br>
 
/*<br>
 * Insertion at the beginning<br>
 */<br>
void double_llist::add_begin(int value)<br>
{<br>
    if (start == NULL)<br>
    {<br>
        cout<<"First Create the list."<<endl;<br>
        return;<br>
    }<br>
    struct node *temp;<br>
    temp = new(struct node);<br>
    temp->prev = NULL;<br>
    temp->info = value;<br>
    temp->next = start;<br>
    start->prev = temp;<br>
    start = temp;<br>
    cout<<"Element Inserted"<<endl;<br>
}<br>
 
/*<br>
 * Insertion of element at a particular position<br>
 */<br>
void double_llist::add_after(int value, int pos)<br>
{<br>
    if (start == NULL)<br>
    {<br>
        cout<<"First Create the list."<<endl;<br>
        return;<br>
    }<br>
    struct node *tmp, *q;<br>
    int i;<br>
    q = start;<br>
    for (i = 0;i < pos - 1;i++)<br>
    {<br>
        q = q->next;<br>
        if (q == NULL)<br>
        {<br>
            cout<<"There are less than ";<br>
            cout<<pos<<" elements."<<endl;<br>
            return;<br>
        }<br>
    }<br>
    tmp = new(struct node);<br>
    tmp->info = value;<br>
    if (q->next == NULL)<br>
    {<br>
        q->next = tmp;<br>
        tmp->next = NULL;<br>
        tmp->prev = q;      <br>
    }<br>
    else<br>
    {<br>
        tmp->next = q->next;<br>
        tmp->next->prev = tmp;<br>
        q->next = tmp;<br>
        tmp->prev = q;<br>
    }<br>
    cout<<"Element Inserted"<<endl;<br>
}<br>
 
/*<br>
 * Deletion of element from the list<br>
 */<br>
void double_llist::delete_element(int value)<br>
{<br>
    struct node *tmp, *q;<br>
     /*first element deletion*/<br>
    if (start->info == value)<br>
    {<br>
        tmp = start;<br>
        start = start->next;  <br>
        start->prev = NULL;<br>
        cout<<"Element Deleted"<<endl;<br>
        free(tmp);<br>
        return;<br>
    }<br>
    q = start;<br>
    while (q->next->next != NULL)<br>
    {   <br>
        /*Element deleted in between*/<br>
        if (q->next->info == value)  <br>
        {<br>
            tmp = q->next;<br>
            q->next = tmp->next;<br>
            tmp->next->prev = q;<br>
            cout<<"Element Deleted"<<endl;<br>
            free(tmp);<br>
            return;<br>
        }<br>
        q = q->next;<br>
    }<br>
     /*last element deleted*/<br>
    if (q->next->info == value)  <br>  
    { 	<br>
        tmp = q->next;<br>
        free(tmp);<br>
        cout<<"Element Deleted"<<endl;<br>
        return;<br>
    }<br>
    cout<<"Element "<<value<<" not found"<<endl;<br>
}<br>
 
/*<br>
 * Display elements of Doubly Link List<br>
 */<br>
void double_llist::display_dlist()<br>
{<br>
    struct node *q;<br>
    if (start == NULL)<br>
    {<br>
        cout<<"List empty,nothing to display"<<endl;<br>
        return;<br>
    }<br>
    q = start;<br>
    cout<<"The Doubly Link List is :"<<endl;<br>
    while (q != NULL)<br>
    {<br>
        cout<<q->info<<" <-> ";<br>
        q = q->next;<br>
    }<br>
    cout<<"NULL"<<endl;<br>
}<br><br><br>
output:<br>
 
Choose one option from the following list ...

1.Insert in begining
2.Insert at last
3.Insert at any random location
4.Delete from Beginning
5.Delete from last
6.Delete the node after the given data
7.Search
8.Show
9.Exit

Enter your choice?
1

Enter Item value2

Node inserted

Choose one option from the following list ...

1.Insert in begining
2.Insert at last
3.Insert at any random location
4.Delete from Beginning
5.Delete from last
6.Delete the node after the given data
7.Search
8.Show
9.Exit

Enter your choice?
1

Enter Item value3

Node inserted

Choose one option from the following list ...

1.Insert in begining
2.Insert at last
3.Insert at any random location
4.Delete from Beginning
5.Delete from last
6.Delete the node after the given data
7.Search
8.Show
9.Exit

Enter your choice?
1

Enter Item value4

Node inserted

Choose one option from the following list ...

1.Insert in begining
2.Insert at last
3.Insert at any random location
4.Delete from Beginning
5.Delete from last
6.Delete the node after the given data
7.Search
8.Show
9.Exit

Enter your choice?
2

Enter value7

node inserted

Choose one option from the following list ...

1.Insert in begining
2.Insert at last
3.Insert at any random location
4.Delete from Beginning
5.Delete from last
6.Delete the node after the given data
7.Search
8.Show
9.Exit

Enter your choice?
8

 printing values...
4
3
2
7

Choose one option from the following list ...

1.Insert in begining
2.Insert at last
3.Insert at any random location
4.Delete from Beginning
5.Delete from last
6.Delete the node after the given data
7.Search
8.Show
9.Exit

Enter your choice?
2

Enter value9

node inserted

Choose one option from the following list ...

1.Insert in begining
2.Insert at last
3.Insert at any random location
4.Delete from Beginning
5.Delete from last
6.Delete the node after the given data
7.Search
8.Show
9.Exit

Enter your choice?
5

node deleted

Choose one option from the following list ...

1.Insert in begining
2.Insert at last
3.Insert at any random location
4.Delete from Beginning
5.Delete from last
6.Delete the node after the given data
7.Search
8.Show
9.Exit

Enter your choice?
8

 printing values...
4

Choose one option from the following list ...

1.Insert in begining
2.Insert at last
3.Insert at any random location
4.Delete from Beginning
5.Delete from last
6.Delete the node after the given data
7.Search
8.Show
9.Exit

Enter your choice?<br><br><br>
	


MERGESORT<br>
#include <iostream><br>
using namespace std;<br>
// A function to merge the two half into a sorted data.<br>
void Merge(int *a, int low, int high, int mid)<br>
{<br>
// We have low to mid and mid+1 to high already sorted.<br>
int i, j, k, temp[high-low+1];<br>
i = low;<br>
k = 0;<br>
j = mid + 1;<br>
// Merge the two parts into temp[].<br>
while (i <= mid && j <= high)<br>
{<br>
if (a[i] < a[j])<br>
{<br>
temp[k] = a[i];<br>
k++;<br>
i++;<br>
}<br>
else<br>
{<br>
temp[k] = a[j];<br>
k++;<br>
j++;<br>
}<br>
}<br>
// Insert all the remaining values from i to mid into temp[].<br>
while (i <= mid)<br>
{<br>
temp[k] = a[i];<br>
k++;<br>
i++;<br>
}<br>
// Insert all the remaining values from j to high into temp[].<br>
while (j <= high)<br>
{<br>
temp[k] = a[j];<br>
k++;<br>
j++;<br>
}<br>
// Assign sorted data stored in temp[] to a[].<br>
for (i = low; i <= high; i++)<br>
{<br>
a[i] = temp[i-low];<br>
}<br>
}<br>
// A function to split array into two parts.<br>
void MergeSort(int *a, int low, int high)<br>
{<br>
int mid;<br>
if (low < high)<br>
{<br>
mid=(low+high)/2;<br>
// Split the data into two half.<br>
MergeSort(a, low, mid);<br>
MergeSort(a, mid+1, high);<br>
// Merge them to get sorted output.<br>
Merge(a, low, high, mid);<br>
}<br>
}<br>
int main()<br>
{<br>
int n, i;<br>
cout<<"\nEnter the number of data element to be sorted: ";<br>
cin>>n;<br>
int arr[n];<br>
for(i = 0; i < n; i++)<br>
{<br>
cout<<"Enter element : ";<br>
cin>>arr[i];<br>
}<br>
MergeSort(arr, 0, n-1);<br>
// Printing the sorted data.<br>
cout<<"\nSorted Data ";<br>
for (i = 0; i < n; i++)<br>
cout<<"->"<<arr[i];<br>
return 0;<br>
}<br>
OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98145023/165239624-717f5b4c-69fa-40ef-a1cc-acd2c52a21ca.png)<br><br><br>
		   


MINHEAP<br>
#include <iostream><br>
#include <conio.h><br>
using namespace std;<br>
void min_heap(int *a, int m, int n){<br>
int j, t;<br>
t= a[m];<br>
j = 2 * m;<br>
while (j <= n) {<br>
if (j < n && a[j+1] < a[j])<br>
j = j + 1;<br>
if (t < a[j])<br>
break;<br>
else if (t >= a[j]) {<br>
a[j/2] = a[j];<br>
j = 2 * j;<br>
}<br>
}<br>
a[j/2] = t;<br>
return;<br>
}<br>
void build_minheap(int *a, int n) {<br>
int k;<br>
for(k = n/2; k >= 1; k--) {<br>
min_heap(a,k,n);<br>
}<br>
}<br>
int main() {<br>
int n, i;<br>
cout<<"enter no of elements of array\n";<br>
cin>>n;<br>
int a[30];<br>
for (i = 1; i <= n; i++) {<br>
cout<<"enter element"<<" "<<(i)<<endl;<br>
cin>>a[i];<br>
}<br>
build_minheap(a, n);<br>
cout<<"Min Heap\n";<br>
for (i = 1; i <= n; i++) {<br>
cout<<a[i]<<endl;<br>
}<br>
getch();<br>
}<br>
OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98145023/165242597-2518cdd6-12b4-4a07-a700-b34d46a23cc7.png)<br><be><br>
	
	
	
BFS DFS<br>
#include<iostream><br>
#include<vector><br>
#include<queue><br>
#include<stack><br>
using namespace std;<br>
void edge(vector<int>adj[],int u,int v){<br>
  adj[u].push_back(v);<br>
}<br>
void bfs(int s,vector<int>adj[],bool visit[]){<br>
  queue<int>q;<br>
  q.push(s);<br>
  visit[s]=true;<br>
  while(!q.empty()){<br>
    int u=q.front();<br>
    cout<<u<<" ";<br>
    q.pop();<br>
    for(int i=0;i<adj[u].size();i++){<br>
      if(!visit[adj[u][i]]){<br>
        q.push(adj[u][i]);<br>
        visit[adj[u][i]]=true;<br>
      }<br>
    }<br>
  }<br>
}<br>
void dfs(int s,vector<int>adj[],bool visit[]){<br>
  stack<int>stk;<br>
  stk.push(s);<br>
  visit[s]=true;<br>
  while(!stk.empty()){<br>
    int u=stk.top();<br>
    cout<<u<<" ";<br>
    stk.pop();<br><br>

    for(int i=0;i<adj[u].size();i++){<br>
      if(!visit[adj[u][i]]){<br>
        stk.push(adj[u][i]);<br>
        visit[adj[u][i]]=true;<br>
      }<br>
    }<br>
  }<br>
}<br>
int main(){<br>
  vector<int>adj[5];<br>
  bool visit[5];<br>
  for(int i=0;i<5;i++){<br>
    visit[i]=false;<br>
  }<br>
  edge(adj,0,2);<br>
  edge(adj,0,1);<br>
  edge(adj,1,3);<br>
  edge(adj,2,0);<br>
  edge(adj,2,3);<br>
  edge(adj,2,4);<br>
  cout<<"BFS traversal is"<<"  ";<br>
  bfs(0,adj,visit);<br>
  cout<<endl;<br>
  for(int i=0;i<5;i++){<br>
    visit[i]=false;<br>
  }<br>
  cout<<"DFS traversal is"<<"  ";<br>
  dfs(0,adj,visit);<br>
}<br>
OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98145023/165246628-04765081-e790-4d6f-9eef-3f665e23871c.png)<br><br><br>

