# numbers-guess-game
#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;

int main() {
    srand(time(0)); // Seed the random number generator
    int randomNumber = rand() % 100 + 1; // Generates a number between 1 and 100
    int guess;
    bool guessedCorrectly = false;

    cout << "Welcome to the Number Guessing Game!" << endl;
    cout << "I have chosen a number between 1 and 100. Try to guess it!" << endl;

    while (!guessedCorrectly) {
        cout << "Enter your guess: ";
        cin >> guess;

        if (guess < randomNumber) {
            cout << "Too low! Try again." << endl;
        } else if (guess > randomNumber) {
            cout << "Too high! Try again." << endl;
        } else {
            cout << "Congratulations! You guessed the correct number." << endl;
            guessedCorrectly = true;
        }
    }
    return 0;
}
