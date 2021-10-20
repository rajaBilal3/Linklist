# Linklist
#include <iostream>

using namespace std;
class Node{
    public:
    int data;
    Node*next;
};
void print_List(Node*n)
{
    cout << "Print List of Node"<< endl;
   
    while(n!=NULL ){
        cout <<n->data<<endl;
        n=n->next;
    }
}
int main()
{
    cout<<"Link list"<<endl;
   Node * head;
   Node * second;
   
   head = new Node();
  second= new Node();
   
   
   head->data = 12;
   head->next = second;
   
   second->data = 13;
   second->next = NULL;
   
  /* cout << "head data "<<head->data<< endl;
   cout << "second data "<<second->data<< endl;
    */
    print_List(head);
   
   
   
    return 0;
}
