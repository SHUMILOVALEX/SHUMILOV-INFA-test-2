TASK 3.1(16.09 второе занятие)
#include <iostream>
int main() {
    double x, y;
    int a = 1;
    std::cout << "On the first day Ivan Ivanovich washed\n";
    std::cin >> x;
    std::cout << "The Federal Tax Service (FTS) plans to take an interest in Ivan Ivanovich on the day when the amount of money laundered exceeds\n";
    std::cin >> y;
     while (x <= y) {
        x += x * 0.1; 
        a++;
    }
    std::cout << "On the " << a << " st Ivan Ivanovich's sky will become checkered (the Federal Tax Service will take care of it)"<<std::endl;
    return 0;
}
TASK 4.1(16.09 второе занятие)
#include <cmath>
#include <iostream>
int main (){
    int a,b;
    char c;
    std::cin>>a>>c>>b;
    int result;
    switch(c){
        case '+':
            result = a + b;
            break;
        case '-':
            result = a - b;
            break;
        case '*':
            result = a * b;
            break;
        case '/':
        case ':':
            result = a / b;
            break;
        case '%':
            result = a % b;
            break;
        default:
            result = 0;
    }
    std::cout << result << '\n';
}
TASK 4.2(16.09 второе занятие)
#include <iostream>
#include <string>
int main (){
    int a, b, result;
    char operation;
    std::string name = "";
    std::cout << "enter two numbers\n";
    std::cin >> a >> b;
    while (result != b){
        std::cout << "enter the operation '-' or ':' or '/'\n";
        std::cin >> operation;
        if ((operation == ':' || operation == '/') && a%2 == 0){
            result = a / 2;
            a /= 2;
            name += "/"; 
            std::cout << result<<"\n";
        }
        else {
            result = a - 1;
            a = a - 1;
            name += "-";
            std::cout << result<<"\n";
        }
    }
std::cout << "U win"<<"\t"<< "Your subsequence"<<"\t"<<name;}
