# coading-practice



// Online C++ compiler to run C++ program online
#include <iostream>
using namespace std;
unsigned int count = 0;
void display(int n, int digits){
    cout<<"Number of Digits in "<<n<<" : "<<digits;
}

int count_digits(int num){
    if(num == 0){
        return count;
    }
    else{
        count++;
        count_digits(num/10);
    }
}

int main() {
    cout<<"Enter a number : ";
    unsigned int Orig_number, number;
    
    cin>>number;
    Orig_number = number;
    int result = count_digits(number);
    display(number, result);
    

    return 0;
}
