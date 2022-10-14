# My-small-game
This is my game "need to guess the number"
#include <iostream>
using namespace std;
static int valueX (2);

class Point {
private:
    int x = 5;
public:
    void Print() {
        cout << " Я загодал число от 1 до 10. Вам предстоит его угадать. " << endl;
        cout << "Я буду вам давать подсказки" << endl;
    }
    void gameGuess() {
        for (bool i = false; i < true;)
        {
            cout << " Введите целочисленое число в диапазоне от 1 до 10 - ";
            cin >> x;
            cout << endl;
            if (x==5)
            {
                cout << " ПОздравляю ";
                break;
            }
            if(x<5)
            {
                cout << " Вы ввели меньше чем загадано" << endl;
            }
            else {
                cout << "Вы ввели больше чем загадано";
            }
        }
    }
};


int main()
{ 
   
    setlocale(LC_ALL, "Rusian");
    Point a;
    a.Print();
    a.gameGuess();
}
