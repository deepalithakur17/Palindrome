# Palindrome
...............
#include<bits/stdc++.h>
using namespace std;

int p(string str)
{
    int mid=str.length()/2;
    for(int i=0,j=str.length()-1;i<=mid,j>=mid;i++,j--)
    {
        if(str[i]!=str[j])
        {
            return 0;
        }
    }
    return 1;
}

int main()
{
    string str="23023";
    int g=p(str);
    if(g==1)
    {
        cout<<"yes! palindrome"<<endl;
    }
    else  
    {
        cout<<"oops! not palindrome"<<endl;
    }
}
