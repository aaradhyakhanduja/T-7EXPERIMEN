# Experiment 7
**Aim:** <br>
To study and implement C++ Arrays and Strings<br>
<br>
**Theory:** <br>
C++ arrays are collections of elements with mutually inclusive types which stay together in one contiguous memory space. They can be declared by presenting the type of these elements followed by square brackets that hold their numbers. In other words, arrays begin counting from zero; thus for instance character zero on array becomes the first one while second one becomes character one and so forth. C++ arrays have fixed sizes that must be determined at compile time.<br>

In C++, strings are managed through either C-style string or by utilizing the _string_ class which is included in the Standard Library. In this programming language, strings are made up of groups of characters terminated by a null character (‘\0’). Actions on C-styled strings are done by functions from C standard library like _strlen_, _strcpy_ and _strcat_.<br>
<br>
**Code:** <br>
a.<br> 
```
# include <iostream>  
using namespace std;
int main()
{
    int n = 0,i = 0;
    int a[n];
    cout<<"Enter size of array: ";
    cin>>n;
    for(i = 0; i < n;i++)
    {
        cout<<"Enter element no. "<< i <<" of  the array: ";
        cin>>a[i];

    }
    cout<<endl;
    cout<<"The array defined by the user: "<<endl;
    cout<<"{";
    for(i = 0; i < n;i++)
    {
        cout<<a[i]<<" ";

    }
    cout<<"}";
    cout<<endl;

    return 0;
}
```

<br>

b. <br>
```
# include <iostream>
using namespace std;
int main()
{
    int n = 0,i = 0;
    int a[n];
    cout<<"Enter size of array: ";
    cin>>n;
    for(i = 0; i < n;i++)
    {
        cout<<"Enter element no. "<< i+1 <<" of  the array: ";
        cin>>a[i];

    }
    cout<<endl;
    cout<<"The array defined by the user: "<<endl;
    for(i = 0; i < n;i++)
    {
        cout<<a[i]<<" ";

    }
    cout<<endl;

    cout<<"The array reversed: "<<endl;
    cout<<"{ ";
    for(i = n-1 ; i > -1 ;i--)
    {
        cout<<a[i]<<" ";

    }
    cout<<"}";
    cout<<endl;

    return 0;
}
```
<br>

c. <br>
```
# include <iostream>
using namespace std;
int main()
{
    int n = 0,i = 0;
    int num = 0, co = 0, flag = 0;
    int a[n];
    cout<<"Enter size of array: ";
    cin>>n;
    for(i = 0; i < n;i++)
    {
        cout<<"Enter element no. "<< i+1 <<" of  the array: ";
        cin>>a[i];
    }
    cout<<endl;
    cout<<"Enter the number you want to check: ";
    cin>>num;
    for(i = 0; i < n;i++)
    {
        if(a[i] == num)
        {
            co++;
            flag++;

        }
    }
    if (flag == 0)
    {
        cout<<"Element was not found.";
    }
    else
    {
        cout<<"The element was found "<<co<<" times.";
    }

}
```
<br>

d. <br>
```
# include <iostream>
using namespace std;
int main()
{
    int n = 0,i = 0;
    int a[n];
    int num = 0, maxi = 0, mini = a[0];
    
    cout<<"Enter size of array: ";
    cin>>n;
    for(i = 0; i < n;i++)
    {
        cout<<"Enter element no. "<< i+1 <<" of  the array: ";
        cin>>a[i];
    }
    cout<<endl;
    for(i = 0; i < n;i++)
    {
        if(a[i] > maxi)
        {
            maxi = a[i];
        }
        if(a[i] < mini)
        {
            mini = a[i];
        }
    }
    cout<<"Maximum value amongst the elements are: "<<maxi<<endl;
    cout<<"Minimum value amongst the elements are: "<<mini<<endl;


}
```
<br>

e. <br>
```
# include <iostream>
using namespace std;
int main()
{
    int n = 0,i = 0;
    int num = 0, sum = 0, avg = 0;
    int a[n];
    cout<<"Enter size of array: ";
    cin>>n;
    for(i = 0; i < n;i++)
    {
        cout<<"Enter element no. "<< i+1 <<" of  the array: ";
        cin>>a[i];
    }
    cout<<endl;
    for(i = 0; i < n;i++)
    {
        sum = sum + a[i];
    }
    avg = sum/n;
    cout<<"Sum of elements: "<<sum<<endl;
    cout<<"Average of elements: "<<avg<<endl;


}
```
<br>

f. <br>
```
#include <iostream>
#include <string>
using namespace std; 

int main()
{
    //printing a string
    string s;
    cout<<"Enter a word: ";
    cin>>s;
    cout<<"Word entered by user is: "<<s<<endl;
    cout<<endl;

    //concatenation
    string s1,s2;
    cout<<"Enter a word: ";
    cin>>s1;
    cout<<"Enter another word: ";
    cin>>s2;
    cout<<"Concatenated word is: "<<s1+s2<<endl;
    cout<<endl;

    //reverse
    string s3;
    int i = 0;
    cout<<"Enter a word: ";
    cin>>s3;
    cout<<"Reverse String: ";
    for (i = s3.length()-1; i>=0; i-- )
    {
        cout<<s3[i];
    }
    cout<<endl;
    cout<<endl;

    //palindrome.
    string s4,rs;
    int j = 0;
    cout<<"Enter a word: ";
    cin>>s4;
    for (j = s4.length()-1; j>=0; j-- )
    {
        rs = rs + s4[j];
    }
    if (rs == s4)
    {
        cout<<"It is a palindrome."<<endl;
    }
    else
    {
        cout<<"It is not a palindrome."<<endl;   
    }
    cout<<endl;
}
```
<br>

**Output**

a.<br>
![exp7a](https://github.com/user-attachments/assets/e7d97fa6-2e67-4395-bac9-38487e44e10a)

<br>
b.<br>
![exp7b](https://github.com/user-attachments/assets/4e114d50-4473-4579-80a5-f18bea84b158)

<br>
c.<br>
![exp7c](https://github.com/user-attachments/assets/b13f416d-fabd-4f1e-b9de-e506a8b3116a)

<br>
d.<br>
![exp7d cpp](https://github.com/user-attachments/assets/27ef208d-f28f-46ed-8512-5723f8820fc5)

<br>
e.<br>
![exp7e](https://github.com/user-attachments/assets/f37524f5-582f-473c-b27d-e1e194f8a4c5)

<br>
f.<br>
![exp7f cpp](https://github.com/user-attachments/assets/ceeb8b8c-58ae-4c5f-8b07-85d60e646e38)

<br>

**Conclusion:** <br>
&#8594; We learnt the use case of arrays in C++. <br>
&#8594; We learnt how to perform basic string manipulations in C++. <br>
<br>
