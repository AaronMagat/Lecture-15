# Lecture-15





#include <iostream>
#include <string>
#include <array>
#include <algorithm>
using namespace std;

void welcome();
void bye();

int main()
{
    welcome();
    bye();
    return 0;
}


void welcome()
{
    cout << "Welcome\n";
}

void bye()
{
    cout << "Goodbye\n";
}
  
  
  
  
  
  
  
  #include <iostream>  
using namespace std;
/* return type set to string as this function will return a string value back  to main program */

string greetings(int time) {
	//evaluate int value passed in and set return message 
	if (time < 12) {
		return "Good Morning";
	}
	else if(time >=12 && time <=17)  {
		return "Good Afternoon";
	}
	else if (time >= 18 && time <= 21) {
		return "Good Evening";

	}
	else if (time >= 22 && time <= 24) {
		return "Good Night";
	}

}
int main() {
	cout << "What time is it? Enter the time in 24 format" << endl; //ask the user for time 
	int userInput; //variable to store user response
	cin >> userInput; //get user input

	//output string returned by function 
	cout << greetings(userInput) << endl;
	return 0;
}
