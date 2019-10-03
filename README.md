# include <iostream>
using namespace std;
int main()
{
    cout<<"C A L C U L A T O R"<<endl;
    cout<<"by : Ligee Guillena"<<endl;
    cout<<"-------------------"<<endl;
    cout<<endl<<endl<<endl;
    
    char op;
    float num1, num2;
    cout << "Enter operator either + or - or * or /: ";
    cin >> op;
    cout << "Enter first operand: ";
    cin>>num1;
    cout << "Enter second operand: ";
    cin>>num2;
    
    switch(op)
    {
        case '+':
            cout<<""<<num1<<"+"<<num2<<": ";
            cout << num1+num2;
            break;
             
        case '-':
            cout<<""<<num1<<"-"<<num2<<": ";
            cout << num1-num2;
            break;
            
        case '*':
            cout<<""<<num1<<"*"<<num2<<": ";
            cout << num1*num2;
            break;
            
        case '/':
            cout<<""<<num1<<"/"<<num2<<": ";
            cout << num1/num2;
            break;
            
        default:
            // If the operator is other than +, -, * or /, error message is shown
            cout << "unknown error";
            break;
    }
    return 0;
}
