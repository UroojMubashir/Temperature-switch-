


#include <iostream>


    using namespace std;
    void convertFahrenheitToCelsius(double f) {
        double c = (f - 32) / 1.8;
        cout << f << " Fahrenheit = " << c << " Celsius";
    }
    void convertCelsiusToFahrenheit(double c) {
        double f = (c * 1.8) + 32;
        cout << c << " Celsius = " << f << " Fahrenheit";
    }
    int main()
    {
        char choice;
        cout << "\ kindly Enter 'F' to convert from Fahrenheit to Celsius ,Kindly Enter 'C' to convert from Celsius to Fahrenheit:";
        cin >> choice;
        double temp_f;
        double temp_c;
        switch (choice) {
        case 'f':
            cout << "\nEnter temperature in Fahrenheit: ";
            cin >> temp_f;
            convertFahrenheitToCelsius(temp_f);

            break;
        case 'c':
            cout << "\nEnter temperature in Celsius: ";
            cin >> temp_c;
            convertCelsiusToFahrenheit(temp_c);
            break;
        default:
            cout << "\Opps Sorry Invalid input!";
        }


        return 0;
    }
