#include <iostream>
using namespace std;

struct Stack
{
int value;
Stack* next;	
};

void push(Stack* &ptr, int input)
{
	
if(ptr != NULL)	
	push(ptr->next, input);
else{

ptr = new Stack;	
ptr->value = input;
ptr->next = NULL;
return;
}
}

void pop(Stack* &ptr)
{
if(ptr->next != NULL)	
	pop(ptr->next);
	
else{
ptr->value = 0;
ptr = NULL;
	}
};

void display(Stack* ptr)
{
if(ptr != NULL)
{
cout << ptr->value << endl;
display(ptr->next);
}	
	
}



int main()
{
int main_input;
Stack *main_ptr = NULL;

while(1)
{
cin >> main_input;	
if(main_input == -1)
break;	
push(main_ptr, main_input);	
}

display(main_ptr);

}
