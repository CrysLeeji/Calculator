# include <iostream>

using namespace std;

int main()
{
    cout<<"C A L C U L A T O R"<<endl;
    cout<<"by : Ligee Guillena"<<endl;
    cout<<"-------------------"<<endl;
    cout<<endl<<endl<<endl;
    
    char op,redo;
    float num1, num2;
    
    do
    {
        
        cout << "Enter operator either + or - or * or /: ";
        cin >> op;
        cout << "Enter first operand: ";
        cin>>num1;
        cout << "Enter second operand: ";
        cin>>num2;
    
    switch(op)
    {
        case '+':
            cout<<"Solution: "<<num1<<"+"<<num2<<" = ";
            cout<<num1+num2<<endl;
            break;
             
        case '-':
            cout<<"Solution: "<<num1<<"-"<<num2<<" = ";
            cout<<num1-num2<<endl;
            break;
            
        case '*':
            cout<<"Solution: "<<num1<<"*"<<num2<<" = ";
            cout<<num1*num2<<endl;
            break;
            
        case '/':
            cout<<"Solution: "<<num1<<"/"<<num2<<" = ";
            cout<<num1/num2<<endl;
            break;
            
        default:
            // If error occured message is shown
            cout << "unknown command";
            break;
            
        
    }
        //to continue
        cout<<"Enter C or c to continue:";
        cin>>redo;
        cout<<endl<<endl;
    }
    while(redo=='C'||redo=='c');
 
    return 0;
 
}
