#include <iostream>

using namespace std;

int main()
{
    double merchandiseCost, employeesSalary, rent, electricityCost, desiredProfit;

    // Prompting Linda to enter the necessary expenses
    cout << "Enter the total cost of merchandise: ";
    cin >> merchandiseCost;

    cout << "Enter the total salary of employees (including your own salary): ";
    cin >> employeesSalary;

    cout << "Enter the yearly rent: ";
    cin >> rent;

    cout << "Enter the estimated yearly electricity cost: ";
    cin >> electricityCost;

    cout << "Enter the desired net profit percentage (e.g., 10 for 10%): ";
    cin >> desiredProfit;

    // Calculating total expenses
    double totalExpenses = merchandiseCost + employeesSalary + rent + electricityCost;

    // Calculating the markup percentage needed for desired profit
    double markupPercentage = (desiredProfit / 100) * totalExpenses / merchandiseCost;

    // Considering the 15% sale discount
    markupPercentage = markupPercentage / 0.85;

    cout << "To achieve approximately " << desiredProfit << "% net profit, ";
    cout << "the merchandise should be marked up by approximately " << markupPercentage * 100 << "%." << endl;


    return 0;
}
