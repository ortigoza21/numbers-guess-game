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
![yXDfAOkDnh](https://github.com/user-attachments/assets/9b9cb0b8-df87-4139-be20-c4505df1031f)
![Code_NA66PqTdsa](https://github.com/user-attachments/assets/81c4cea2-314d-4e12-92e9-82539c358d6d)
![ctPymy2uG7](https://github.com/user-attachments/assets/73ba8c04-086c-49b7-8383-63f91f19e574)
![Mlr3U8rjah](https://github.com/user-attachments/assets/98e7d2aa-aecc-4741-b1fe-324114f360fd)
![GQECLRhOQq](https://github.com/user-attachments/assets/262c6e30-d447-4fbf-8cfd-043b55919ec1)

