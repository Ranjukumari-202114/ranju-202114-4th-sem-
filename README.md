# ranju-202114-4th-sem-


/*Write the program to read a matrix of size m x n from the keyboard and display 
 the same  using functions.*/ 


#include <iostream>
using namespace std;

int read_matrix(int a[2][20],int x,int y);
int display_matrix(int a[20][20],int x,int y);


int main()
{
    int m,n;
    cout<<"Enter the value of m = ";
    cin>>m;
    cout<<"Enter the value of n = ";
    cin>>n;
    cout<<endl;
    int a[20][20];
    read_matrix(a,m,n);
     cout<<endl;
    display_matrix(a,m,n);
}
int read_matrix(int a[20][20],int x,int y)
  {
    cout<<"enter the value of matrix"<<"\n";
    int i,j;
    for(i=0;i<x;i++)
    {
      for(j=0;j<y;j++) 
        { 
          cin>>a[i][j]; 
        } 

     }
     return 0;
 }

int display_matrix( int a[20][20] ,int x, int y) 
 { 
   int i,j; 
    for(i=0;i<x;i++) 
       { 
          for(j=0;j<y;j++)
            {
             cout<< a[i][j]<<"\t";
            }
            cout<< endl; 
        }
        return 0;
 } 
