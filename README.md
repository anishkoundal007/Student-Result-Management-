#include <iostream>
using namespace std;

int main() {
    string name;
    int roll;
    float s1, s2, s3, total, percent;
    
    cout << "Enter Name: ";
    cin >> name;
    cout << "Enter Roll Number: ";
    cin >> roll;

    cout << "Enter marks of 3 subjects: ";
    cin >> s1 >> s2 >> s3;

    total = s1 + s2 + s3;
    percent = total / 3;

    cout << "\n--- RESULT ---\n";
    cout << "Name: " << name << endl;
    cout << "Roll: " << roll << endl;
    cout << "Total: " << total << endl;
    cout << "Percentage: " << percent << "%" << endl;

    if (percent >= 90) cout << "Grade: A+";
    else if (percent >= 80) cout << "Grade: A";
    else if (percent >= 70) cout << "Grade: B+";
    else if (percent >= 60) cout << "Grade: B";
    else if (percent >= 50) cout << "Grade: C";
    else cout << "Grade: Fail";

    return 0;
}
