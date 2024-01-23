#include <iostream>
#include <cstdlib>
#include <ctime>

int rollDie() {
    return rand() % 6 + 1; // Generates a random number between 1 and 6
}

int main() {
    srand(static_cast<unsigned int>(time(0))); // Seed for random number generation

    int firstDie = rollDie();
    int secondDie = rollDie();

    std::cout << "First Die: " << firstDie << std::endl;
    std::cout << "Second Die: " << secondDie << std::endl;
    std::cout << "Total: " << firstDie + secondDie << std::endl;

    return 0;
}
