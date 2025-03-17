#include <iostream>
using namespace std;


   double calculateAverage(int scores[], int numScores) {
    double total = 0;
    for (int i = 0; i < numScores; i++) {
        total += scores[i];
    }
    return total / numScores;
    }


   char determineGrade(double avgScore) {
    if (avgScore >= 90) return 'A';
    else if (avgScore >= 80) return 'B';
    else if (avgScore >= 70) return 'C';
    else if (avgScore >= 60) return 'D';
    else return 'F';
    }


   void displayResults(string names[], double averages[], char grades[], int numStudents) {
    cout << "\nResults:\n";
    cout << "------------------------------\n";
    cout << "Student    | Average | Grade\n";
    cout << "------------------------------\n";

    for (int i = 0; i < numStudents; i++) {
        cout << names[i] << " | " << averages[i] << " | " << grades[i] << endl;
    }
    cout << "------------------------------\n";
    }

    int main() {
    int numStudents;

    
    cout << "Enter the number of students: ";
    cin >> numStudents;

    
    string names[numStudents];
    double averages[numStudents];
    char grades[numStudents];


    for (int i = 0; i < numStudents; i++) {
     cout << "\nEnter name of student " << i + 1 << ": ";
     cin >> names[i];

     int numTests;
     cout << "Enter number of test scores: ";
     cin >> numTests;

     int scores[numTests]; 

        
    for (int j = 0; j < numTests; j++) {
     cout << "Enter score " << j + 1 << ": ";
     cin >> scores[j];
        }

      
    averages[i] = calculateAverage(scores, numTests);
    grades[i] = determineGrade(averages[i]);
    }

    
    displayResults(names, averages, grades, numStudents);

    return 0;
}
