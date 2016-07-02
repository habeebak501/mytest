
#include<iostream>
using namespace std;
class linkedlist
{
	struct node    //To create a node
	{
		string name;
		struct node *next;
	};
	struct node *start;
	public:
	void insert(string name);//Insert an element to the linkedlist
	void search();//Searching an element in the linkedlist
	void display();//Display the elements in the linkedlist
	int stringcmp(string,string);//Comparing the two strings
         string removespaces(string name);

	linkedlist()//Constructor
	{
		start=NULL;
	}
};
//Declare a function outside of a class 
void linkedlist::insert(string name)
{
        
	node *newnode;//To create a newnode
	newnode=new node;//Allocating memory for newnode using "new" keyword
	if(start==NULL)
	{
		newnode->name=name;
		newnode->next=NULL;
		start=newnode;
	}
	else//If aleready node is there then  adding a  newnode into existing node
	{
		newnode->name=name;
		newnode->next=start;
		start=newnode;
	}
            
}



void linkedlist::display()
{
	node *temp;
	temp=start;
	while(temp!=NULL)
	{
		cout<<temp->name<<endl;
		temp=temp->next;
	}
}
/*
int linkedlist::stringcmp(string str1,string str2)//Function defination
{
	int j=0,flag=0;
	while(str1[j]!='\0'&& str2[j]!='\0')
	{
		if(str1[j]!=str2[j])
		{
			flag=1;
			break;
		}
		j++;
	}
	if(flag==0&&str1[j]=='\0'&&str2[j]=='\0')
		return 1;
	else 
		return 0;
}*/
string linkedlist::removespaces(string name)
{

   int i,j;
for(i=0;name[i]!='\0';i++)
  {
    if(name[i]==' ')
     {
        for(j=i;name[j]!='\0';j++)
         {
            name[j]=name[j+1];
          }
      }
      name[j]='\0';
}
    return name;
}  
   





     //  insert(string name);

/*
void linkedlist::search()
{
	node *temp;
	temp=start;
	string str,str1;
	cout<<"Enter Search string:";//To take input from user searching a string
	getline(cin,str);
         str1=removespaces(str);
	int i;
	while(temp!=NULL)

	{


		i=stringcmp(temp->name,str1);//Function call
		if(i==1)
		{
			cout<<"---------String found---------"<<endl;//Searching string is found in the linkedlist to display message string is found
			return;

		}

		temp = temp->next;
	}

         cout<<"-----------string added---------";
	insert(str1);//If searching string is not found to add searching element into the linkedlist


}

*/
int main()
{
	linkedlist ll;
	//string str,str1;
	   
           /*   cout<<"enter the string:"<<endl;
               getline(cin,str);
           str1=ll. removespaces(str);
                 ll.insert(str1);
             // cout<<str1<<endl;
             ll.display();
    
	   //ll.search();
	   //ll.display();

 */


	int n;
	string str,str1;
	cout<<"how many strings u want to insert:";
	cin>>n;
        cout<<"enter the strings:"<<endl;
	for(int i=0;i<n;i++)
	{
          
                  getline(cin,str);
              // str1=ll.removespaces(str);
                 ll.insert(str1);
	}
             ll.display();
        

	return 0;
}

