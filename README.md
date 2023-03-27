#include <iostream>
using namespace std;

int main() {
    int year;
    int month;

    cout << "Enter the year: ";
    cin >> year;
    cout << "Enter the month as a number (1-12): ";
    cin >> month;

    int daysinmonth;
    string monthname;

    switch (month) {
        case 1:
            monthname = "January";
            daysinmonth = 31;
            break;
        case 2:
            monthname = "February";
            if ((year % 400 == 0 || year % 4 == 0))  {
                daysinmonth = 29;
            } else {
                daysinmonth = 28;
            }
            break;
        case 3:
            monthname = "March";
            daysinmonth = 31;
            break;
        case 4:
            monthname = "April";
            daysinmonth = 30;
            break;
        case 5:
            monthname = "May";
            daysinmonth = 31;
            break;
        case 6:
            monthname = "June";
            daysinmonth = 30;
            break;
        case 7:
            monthname = "July";
            daysinmonth = 31;
            break;
        case 8:
            monthname = "August";
            daysinmonth = 31;
            break;
        case 9:
            monthname = "September";
            daysinmonth = 30;
            break;
        case 10:
            monthname = "October";
            daysinmonth = 31;
            break;
        case 11:
            monthname = "November";
            daysinmonth = 30;
            break;
        case 12:
            monthname = "December";
            daysinmonth = 31;
            break;
        default:
            cout << "Invalid month number" << endl;
            return 0;
    }

    cout << "The " << month << " month is " << monthname << " and it has " << daysinmonth << " days." << endl;

    return 0;
}

