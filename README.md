#include <iostream>
using namespace std;
int main() {
     double balance, withdraw, deposite;
     balance=0;
      int input;
      cout<<"1.to display the balance \n";
      cout<<"2.to deposite money into account\n";
      cout<<"3.to withdraw money from account\n";
      cout<<"4. exit\n";
      cout<<"enter choice:";
      cin>>input;
      
      while(input)
      {
        switch(input)
        {
            case 1:
            cout<<"the current balance in your account is:"<<balance<<endl;
            break;
            case 2:
            cout<<"enter money you wish to add to your bank:";
            cin>>deposite;
            balance=balance+deposite;
            cout<<"you have entered"<<deposite<<endl;
            break;
            case 3:
            cout<<"enter money you want to withdraw:";
            cin>>withdraw;
            balance= balance-withdraw;
            cout<<"you have withdrawn"<<withdraw<<" from your account"<<endl;
            break;
            default:
            cout<<"you have entered a wrong input"<<endl;
        }
        cout<<"enter choice:";
        cin>>input;
     }
}
      
