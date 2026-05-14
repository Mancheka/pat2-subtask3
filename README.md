# pat2-subtask3

#include <iostream>
using namespace std;

int main() {

    const int experiments = 4;

    for (int i = 1; i <= experiments; i++) {
        cout << "\nExperiment " << i << endl;

        float total = 0, reading;

        for (int j = 1; j <= 3; j++) {
            cout << "Enter reading " << j << ": ";
            cin >> reading;
            total += reading;
        }

        float avg = total / 3;
        cout << "Experiment " << i << " average :"; cout<<avg;

        if (avg < 100)
            cout << "are: Below acceptable range" <<endl;
        else if (avg <= 300)
            cout << " are: Within acceptable range" <<endl;
        else
            cout << "are: Above acceptable range" <<endl;
    }  // <- this was missing

    return 0;
}
