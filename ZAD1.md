#include <iostream>
#include<string.h>

using namespace std;

int main() {
    long a;
    int pol =0 ;
    char string2[250];
    char string[250];
    cin.getline(string, 250);
    a = strlen(string);

    for (int i = 0; i <a ; i++) {
        cout << string[i]<<'\n';

    }


    for (int i = 0; i < 250; i++) {
        
         if (string[i] == ' ')
         {
             string2[i]='%';
             string2[i+1]='2';
             string2[i+2]='0';
             pol=pol+2;
             
         }
        string2[i] = string[i];

    }
        for (int i = 0; i <250; i++) 
        {
            cout << string2[i];

        }



    return 0;
}
