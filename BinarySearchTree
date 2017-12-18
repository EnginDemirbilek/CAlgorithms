#include <iostream>
using namespace std;

struct Tree{
int value;
Tree *left;
Tree *right;
Tree *parent;	
};


void insert(Tree* &ptr, int value)
{
	if(ptr==NULL){
		ptr = new Tree;
		ptr->value = value;
		ptr->left = NULL;
		ptr->right = NULL;	
	}
	
	else if(value < ptr->value){
			insert(ptr->left, value);	
	}
	
	else if(value > ptr->value){
		insert(ptr->right, value);
	}

}


void Display(Tree *ptr){
	if(ptr==NULL)
		return;
	Display(ptr->left);
	cout << ptr->value << endl;
	Display(ptr->right);
	
}


int main()
{
Tree *main_ptr = NULL;
int main_value;

while(1)
{
	cin >> main_value;
	if(main_value == -1)
		break;
	insert(main_ptr,main_value);	
	
}
Display(main_ptr);
	
}


