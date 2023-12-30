#include <iostream>
#include <windows.h>
using namespace std;
int main() {
    SetConsoleCP(1251);
    SetConsoleOutputCP(1251);
    int height, number;
    cout << "Введите высоту треугольников: ";
    cin >> height;
    cout << "Введите число треугольников: ";
    cin >> number;

    for (int i = 0; i < height; i++) {

        for (int n = 0; n < number; n++) {
            for (int j = 0; j < 7 - i - 1; j++) {
                cout << " ";
            }
            for (int k = 0; k < 2 * i + 1; k++) {
                cout << "*";
            }

            for (int q = 0; q < 7 - i - 1; q++) {
                cout << " ";
            }
            cout << " ";

        }
        cout << endl;
    }

    return 0;
}
