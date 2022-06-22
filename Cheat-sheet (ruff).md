#this is The Cheat-sheet for Ruff idea about cpp
``` C++
//#include<bits/stdc++.h>   --use this for OOP and online compition of programing
#include<iostream>
#include<string.h>   //use only when you use string in program
using namespace std;

// ********** Function defining *****
//define function and call at line 88 to 93
int sum(int x,int y){
    int z;
    z=x+y;
    return z;
}

//#################    class
 class employee
{
    public:  // private: and protected:
    string name;
    int salary;

    //constructor  line 206
    employee(string name,int salary,int secp)  //employee(string N,int S)
     // the string name , int salary is individual so you can name it as you want  so the main and constructor variables are difreent
    {
        this->name =name;       // this->name =N
        this->salary =salary;  //this->salary =S
        this->SecretPassword =secp;
    }

    //***********method ********** in this table "this is method to call employee"
    void printDetails(){
        cout<<"The name of first employee is :"<<this->name<< "And the Salary was :"<<this->name<<"$"<<endl;
        // Don't Use "<<first.name<< ""<<first.salary<<"$"<<endl;  use "-> " insted of "."
    }
    // *****public method can access Private class data
    void getSecretPassword(){
        cout<<"the secret password is :"<<this->SecretPassword<<endl;
    }

   private:
   int SecretPassword;

};

//**************inharitans *****************
class programmer : public employee{

   public:
   int errors;

};

int main(){

    std::cout<<"this is cheetshit for Cpp"<<endl;
    //you can use std:: as a replacement of Using namespace std;
    int a, b ,c; //declare variables
    short astra;    //declate variables
    bool yes;  //declate variables
    char password;  //declate variables
    long A;
    long long B;

    if (a=0)
    {
        cout<<"this is not good input"<<endl;
    }

    else if(a=0)
    {
        cout<<"this is goood "<<endl;

    }
    else
    {
        cout<<"you are done"<<endl;
    }

    //******************************* switch case **********************************************

    int age;
    cout<<"input your age"<<endl;
    cin>>age;

    switch (age)
    {
    case 12:  //do not enter age=12 beacause this is case so it define in first line that thsi case is for age alimant
        cout<<"you are ready to run "<<endl;
        break;

    case 20:  //and dont forgate that this is :  not ;
        cout<<"this aligible to work "<<endl;
    break;

    default:
      cout<<"default case close"<<endl;
        break;
    }

//********************************** while loop **********************************************
int index=0;
while (index<35);
{
    cout<<"print number "<<index<<"as"<<index;
    index = index +1 ;
    //and use also
    // index ++ ;
}


//********************************** do while ***********************************************
/*do while loop is work as a while loop but the cache is that
    do while loop run atleast one time whether it condition is true or note*/
do
{
     cout<<"print number "<<index<<"as"<<index;
    index = index +1 ;

} while (index>35);

//********************************** for loop **************************************************
int count;
for (int i = 0; i < count; i++)
{
    cout<<count<<endl;
}

//********************************** Function define *****************************************
//in over top of  main section we have example of define function
int x,y;
cout<<"input number one"<<endl;
cin>>x;
cout<<"input number two"<<endl;
cin>>y;
cout<<"sum of two number is "<<sum(x,y);

//*********************************** array 1D ************************************************
int arr[3]={1,2,3};
//   index  0 1 2

for (int i = 0; i < 3; i++)
{
    cout<<arr[i]<<endl;

}

//************************************ array 2D ***********************************************
int arr2d[3][5]={{1,2,3},{4,5,6,7,8}};
//   index      0 1 2   0 1 2 3 4

for (int i = 0; i < 3; i++)
{
    for (int f = 0; f < 5; f++)
    {
         cout<<arr2d[i][f]<<endl;
    }
}

//*********************************** typecast **************************************************
int jaa=20;
int vaa=15;
int smp;

cout<<"value is"<<(float)jaa/vaa<<endl; /*now the two int values genraly output int value
            this is typecast                 but typcast can change the outpur as a float */



//********************************* string *****************************************************
// and also don't forgot to put #include <string.h> headder
string name="jay patel";
cout<<"my name is"<<name<<endl;
cout<<"lenght of name is "<<name.length()<<endl;
cout<<"substring of name is "<<name.substr(0,3)<<endl;
cout<<"substring of name is "<<name.substr(1,5)<<endl;


//****************************  pointer in c++  ************************************************
int j = 988;
int* ptra;
ptra = &j;
//also we input value from usr and store in programe
/*cout<<"input value :"<<endl;
cin>>j; */
cout<<ptra; //which shows the address of "j"
cout<<*ptra; /*which shows the value of "j"  * is D refrencing oprator which refrenc pointer
           ptra is just a refrence name if you want any name or A-Z in pointer you shoud */
cout<< "value of a is "<<a<<endl;      //show the value of a
cout<<"value of a is "<<*ptra<<endl;  //show the value of a
cout<<"address of a is "<<ptra<<endl; //show the address of a  like ex.ax0837309
cout<<"address of a is "<<&a<<endl;  //show the address of a




//*****************************************************************************************************************
// +++++++++++++++++++++++++++++++++++++++ Classis and Objects +++++++++++++++++++++++++++++++++++++++++++++++++++

//********************** classis **************************

// create class  you can use class on all program as object by put this on over(upper) in the main  method
/* class employee
{
    private: //public: and protected:
    string name;
    int salary;

}; */

//***this is without methods in class
employee first;
first.name = "stiven";
first.salary = 5000;
cout<<"The name of first employee is :"<<first.name<< "And the Salary was :"<<first.salary<<"$"<<endl;

//*** this is with method in class
employee second;
second.name = "stiven";
second.salary = 5000;
second.printDetails();
//cout<<"The name of first employee is :"<<first.name<< "And the Salary was :"<<first.salary<<"$"<<endl;


//*** Constructor
employee har("Stiven constructor",5000);
//har.name = "stiven";
//har.salary = 5000;
har.printDetails();
//cout<<"The name of first employee is :"<<first.name<< "And the Salary was :"<<first.salary<<"$"<<endl;

//****# private class Example (public class access private)
employee har("stiven strange",100000,987654321);
har.printDetails();
//cout<<har.SecretPassword;   -----> this is not able to get password because of private class
har.getSecretPassword();
return 0;


}


```
