#include <iostream>
#include <limits>

using namespace std;

int main() {
  char scaleFrom, scaleTo;
  double temperature;

  cout << "Enter the temperature: ";
  cin >> temperature;

  cout << "Enter the scale of the input temperature (C, F, or K): ";
  cin >> scaleFrom;

  cout << "Enter the scale you want to convert to (C, F, or K): ";
  cin >> scaleTo;

  // Input validation
  if (scaleFrom != 'C' && scaleFrom != 'F' && scaleFrom != 'K') {
    cout << "Invalid input scale. Please enter C, F, or K." << endl;
    return 1;
  }
  if (scaleTo != 'C' && scaleTo != 'F' && scaleTo != 'K') {
    cout << "Invalid output scale. Please enter C, F, or K." << endl;
    return 1;
  }

  // Conversion logic
  double convertedTemp;
  if (scaleFrom == 'C' && scaleTo == 'F') {
    convertedTemp = (temperature * 9.0 / 5.0) + 32.0;
  } else if (scaleFrom == 'C' && scaleTo == 'K') {
    convertedTemp = temperature + 273.15;
  } else if (scaleFrom == 'F' && scaleTo == 'C') {
    convertedTemp = (temperature - 32.0) * 5.0 / 9.0;
  } else if (scaleFrom == 'F' && scaleTo == 'K') {
    convertedTemp = (temperature - 32.0) * 5.0 / 9.0 + 273.15;
  } else if (scaleFrom == 'K' && scaleTo == 'C') {
    convertedTemp = temperature - 273.15;
  } else if (scaleFrom == 'K' && scaleTo == 'F') {
    convertedTemp = (temperature - 273.15) * 9.0 / 5.0 + 32.0;
  } else {
    cout << "You chose the same scale for input and output." << endl;
    return 1;
  }

  cout << "Converted temperature: " << convertedTemp << " " << scaleTo << endl;

  return 0;
}
