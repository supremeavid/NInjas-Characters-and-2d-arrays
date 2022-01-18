# NInjas-Characters-and-2d-arrays
#include <bits/stdc++.h>

using namespace std;
//Making function for char arrays, We don't need to input size like int array, because \0 is automatically used by machine
int length(char b[]){
    int count=0;
    int i=0;
    while(b[i]!='\0'){
        count++;
        i++;
    }
    return count;


}


int main()
{
/*    //Strings == 1D character arrays
    char b[10]; //This is a string
    //Here 10 bytes allocated in memory as char require only 1 byte each
    //Character arrays don't need a for loop to input our name
    //Cin and Cout behave specially for character arrays by inputting and outputting full names without even using for loop
    //(/0) is null character with ASCII value 0, this works as terminator in char arrays by the compilers
    char name[100];
    cin>>name;
    cout<<name<<endl;  //Name gets printed, moreover the value after space don't get printed due to properties of Cin
    int lenn= length(name);
    cout<<lenn<<endl;
    char Len[100];
    cin>>Len;
    Len[2]='\0'; //Placed null index (terminator) at the 2nd index of Len i.e. third place
    cout<<Len<<endl;    //Terminates the Len string at 2nd index for example Utkarsh is outputted as Ut     */


    //Write a cpp program to check whether a given string is palindrome or not
 /*   cout<<"Type in the word you want to check for Palindrome or not."<<endl;
    char Pal[100];
    cin>>Pal;
     int start=0;
    int n=length(Pal);
    int end=n-1;
    int count=0;
    for(int i=0;i<n/2;i++){
        if(Pal[start]==Pal[end]){
            count++;
        }
        start++;
        end--;
    }
    if(count>=(n-1)/2){
        cout<<"Palindrome"<<endl;
    }
    else{
        cout<<"Not a Palindrome"<<endl;
    }

    //More on character arrays:
    char b[4];
    cin>>b[4];
    cout<<b[4]; */

    //Write a program for reversing a string
 /*   cout<<"Enter the string to be reversed"<<endl;
    char Cswap[100];
    cin>>Cswap;
    int m=length(Cswap);
    int starts=0;
    int endd=m-1;
    while(starts<=endd){        //If the inner condition remain true then only the loop while run, otherwise it will be skipped
        swap(Cswap[starts],Cswap[endd]);
        starts++;
        endd--;
    }
    cout<<Cswap<<endl;
    //Copying a string from one to another:
    char a[10]="ABCDE";
    char b[10]="BAXNBX";
    strncpy(b,a,3);
    cout<<b<<endl;
    //Write a program to print All prefix of an string;
    //Example all prefix of ABCD are A,AB,ABC,ABCD
    char str[10]="CUCKOO";

    for(int i=1;i<=strlen(str);i++){
            char test[10]="\0";
        strncpy(test,str,i);
        cout<<test<<endl;
    }
    //2nd Approach
    for(int i=0;i<=strlen(str);i++){
        for(int j=0;j<=i;j++){
            cout<<str[j];
        }
        cout<<endl;
    }
        */

    //2D Arrays
/*    int m,n;
    cin>>m;
    cin>>n;
    int a[100][100]; //m rows and n columns
    //Input
    for(int i=0;i<m;i++){
        for(int j=0;j<n;j++){
            cin>>a[i][j];
        }
    }

    //Output /Printing array
    cout<<"Printing Row-wise"<<endl;
    for(int i=0;i<m;i++){
        for(int j=0;j<n;j++){
            cout<<a[i][j]<<" ";
        }
        cout<<endl;
    }
     cout<<"Printing Column-wise"<<endl;
      for(int j=0;j<n;j++){
        for(int i=0;i<m;i++){
            cout<<a[i][j]<<" ";
        }
        cout<<endl;
    }
    //Printing the sum of columns:
    for(int j=0;j<n;j++){
    cout<<"Sum of"<<(j+1) <<"th column is: "<<endl;
    int sum=0;
    for(int i=0;i<m;i++){
        sum=sum+a[i][j];
    }
    cout<<sum<<endl;
    }               */
    //Write a cpp program to print the wave pattern in an array
    int arr[100][100];
    int m,n;
    cout<<"Type the desired number of rows and columns separated by space."<<endl;
    cin>>m>>n;
    //Input
    for(int i=0;i<m;i++){
        for(int j=0;j<n;j++){
            cin>>arr[i][j];
        }
    }
    cout<<endl;
     //Output/Printing array

    for(int i=0;i<m;i++){
        for(int j=0;j<n;j++){
            cout<<arr[i][j]<<" ";
        }
        cout<<endl;
    }
    cout<<endl;
    cout<<"For zigzag pattern: "<<endl;
    for(int j=0;j<n;j++){
    for(int i=0;i<m;i++){
        cout<<arr[i][j]<<" ";
    }
    }
    cout<<endl;
    cout<<endl;
    cout<<endl;
    for(int j=0;j<n;j++){
        if(j%2==0){
            for(int i=0;i<m;i++){

        cout<<arr[i][j]<<" ";}
        }
        else{for(int i=(m-1);i>=0;i--){

        cout<<arr[i][j]<<" ";}
        }
    }




















    return 0;
}
