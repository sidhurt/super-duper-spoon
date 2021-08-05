# super-duper-spoon
Course coordinator wants to prepare the list of students for his class by inputting data such as Name, Roll Number, Division and Program. He only input Name and Roll Number through INPUT function; other data is common for all the students. So, INPUT function will accept default arguments for constant values that need to initialize to student’s attributes. Display the data for 3 students. Write a main function to implement function with default arguments.

#include<iostream>
#include<string.h>
using namespace std;
class student
{
    char name[50];
int roll_no;
char batch[50];
char division[];
public:
    void read_data()
    {
        cout<<"Enter Name:"<<endl;
        cin>>name;
        cout<<"Enter Roll Number:"<<endl;
        cin>>roll_no;
        cout<<"Enter Batch:"<<endl;
        cin>>batch;
    }
    void display_data(char division='E')
    {
        cout<<"Name:"<<name<<endl;
        cout<<"Roll Number:"<<roll_no<<endl;
        cout<<"Batch:"<<batch<<endl;
        cout<<"Division:"<<division<<endl;
    }
};
int main()
{
student s;
cout<<"------Student Data:------"<<endl;
for(int i=0;i<3;i++)
{
// Calling class function
s.read_data();
s.display_data();
}
}
