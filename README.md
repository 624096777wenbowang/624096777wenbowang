#include <iostream>
#include<string>
using namespace std;

int main()
{	// Declaration of eight variables
	int pennies;    
	int nickels;             
	int dimes;         
	int quarters;
	int cents;
	int dollars;
	int Twainesecents;
	int Twainesedollars;

	// Get the input of pennies, nickes, dimes, and quarters.
	cout << "Enter the pennies: " << endl;
		cin >> pennies;
	cout << "Enter the nickels: " << endl;
		cin >> nickels;
	cout << "Enter the dimes: " << endl;
		cin >> dimes;
	cout << "Enter the quarters: " << endl;
		cin >> quarters;

	cents = pennies * 1 + nickels * 5 + dimes * 10 + quarters * 25;
	dollars = cents / 100;
	Twainesecents = cents * 33;
	Twainesedollars = Twainesecents / 100;
	
	cout << "the total is " << cents;
	cout << " US cents " << endl;

	cout << "the total is " << dollars;
	cout << " US dollars " << cents%100 << " US cents" << endl;

	cout << "the total is " << Twainesecents;
	cout << " Twainese cents " << endl;

	cout << "the total is " << Twainesedollars;
	cout << " Twainese dollars " << Twainesecents%100 << " Twainese cents"<< endl;
	

		// Display a good-bye message
	cout << "It is a pleasure to do this currency conversion for you." << endl;
	cout << "Please enter any charcter and a return to quit the program." << endl;


	// Wait for the user input before ending the program
	char inputCharacter;    // Declare a variable for storing a character input from the keyboard
	cin >> inputCharacter; // Wait to read in a character input from the keyboard

	//Finish the program and return the control to the operating system.
	return 0;

}
