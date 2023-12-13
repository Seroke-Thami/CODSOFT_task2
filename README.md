#include <iostream>
using namespace std;

int main() {
    char operation;
    double num1, num2, result;
    //input
    cout << "Enter first number: ";
    cin >> num1;
    cout << "Enter second number: ";
    cin >> num2;

    //operation_sysmbols
    cout << "Choose operation (+, -, *, /): ";
    cin >> operation;

    // Proccessing
    switch (operation) {
        case '+':
            result = num1 + num2;
            cout << "Result: " << result << endl;
            break;
        case '-':
            result = num1 - num2;
            cout << "Result: " << result << endl;
            break;
        case '*':
            result = num1 * num2;
            cout << "Result: " << result << endl;
            break;
        case '/':
            if (num2 != 0) {
                result = num1 / num2;
                cout << "Result: " << result << endl;
            } else {
                cout << "Error! Division by zero is not allowed." << endl;
            }
            break;
        default:
            cout << "Invalid operation. Please choose +, -, *, or /." << endl;
            break;
    }

    return 0;
}
