# character-counter
Count the number of times a character appears in a string 


#include <iostream>
using namespace std;

int charcounter (string a , char b){
    int counter , length = a.length();
    for(int i=0; i<length; i++){
        if(a[i]==b){
            counter++;
        }
    }
    return counter;

}



int main(){
    string s;
    char c;
    cout << "Enter your string: ";
    getline(cin,s);
    cout << "Enter the letter you want to count: ";
    cin >> c;

    cout << "Number of " << c << " in the string: " << charcounter(s , c);
}
