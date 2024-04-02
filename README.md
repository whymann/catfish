# catfish
#include<iostream>
using namespace std;

void MonsterGen();  //decleration

int main() {
	char input;
	while (1) {

		MonsterGen();
		cout << "press any key to continue..." << endl;
		cin >> input;
	}

}

void MonsterGen() { //definition
	int num = rand() % 100; //creates a number between 0-99
	if (num < 33) //15% chance of la llorona to appear
		cout << "you caught a Carp!" << endl;
	else if (num < 53) //30% chance of el chucky to appear
		cout << "YOU CAUGHT A WOODSKIP!" << endl;
	else //25% chance of el charro negro to appear
		cout << "you caught a catfish!" << endl;
}
