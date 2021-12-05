# Switch-Statements

# Lecture 8
Switch Statements 

## Fuel
        #include <iostream>
        using namespace std;
        int main()
        {

    char gas;
    int gasAmt;

    cout << "Welcome to the automatic gas service! Please enter your type of fuel to continue \n";
    cout << "[P] for Petrol or [D] for Diesel \n";
    cin >> gas;


    switch (gas)
    {
    case 'p':
    case 'P':
        cout << "You chose petrol, how many liters do you need? Rate: 2AED Per liter\n";
        cin >> gasAmt;
        cout << "You entered " << gasAmt << " liters. That would be " << gasAmt * 2 << " AED";

        break;
    
    case 'd':
    case 'D':
        cout << "You chose diesel, how many liters do you need? Rate: 3AED Per liter\n";
        cin >> gasAmt;
        cout << "You entered " << gasAmt << " liters. That would be " << gasAmt * 3 << " AED";

        break;
    default:
        cout << "Invalid input";

        return 0;

    }
    }


## Temperature
        #include <iostream>
        using namespace std;
        int main()
        {

    char temp;
    double tempInput;

    cout << "Converting temperatures! Would you like convert Celsius to Farenheit? or Farenheit to Celsius? \n";
    cout << "[C] for C to F or [F] for F to C \n";
    cin >> temp;


    switch (temp)
    {
    case 'C':
    case 'c':
        cout << "Insert temperature in Celsius to convert in Farenheit\n";
        cin >> tempInput;
        cout << "You entered " << tempInput << "C's. That would be " << (tempInput * 1.8) + 32 << " Degrees Farenheit";

        break;

    case 'F':
    case 'f':
        cout << "Insert temperature in Farenheit to convert in Celsius\n";
        cin >> tempInput;
        cout << "You entered " << tempInput << ". That would be " << 5 * (tempInput - 32) / 9 << " Degrees Celcius";

        break;
    default:
        cout << "Invalid input! Please enter a number.";

        return 0;

    }
    }

 ## Capital of France
        #include <iostream>
        using namespace std;
        int main()
        {
    cout << "What is the capital of France?\n";
    cout << "Press [P] for Paris\n";
    cout << "Press [D] for Dubai\n";
    cout << "Press [A] for Alabama\n";
    cout << "Press [W] for Washington \n";

    char capital;
    cin >> capital;

    switch (capital)
    {
    case 'P':
        cout << "Correct! \n";
        break;
    case 'p':
        cout << "Correct! \n";
        break;

    case 'D':
        cout << "Incorrect \n";
        break;
    case 'd':
        cout << "Incorrect \n";
        break;
    case 'A':
        cout << "Incorrect \n";
        break;
    case 'a':
        cout << "Incorrect \n";
        break;
    case 'W':
        cout << "Incorrect \n";
        break;
    case 'w':
        cout << "Incorrect \n";
        break;
    
         
    default:
        cout << "Invalid \n";
        break;
    } 
    }

## Shapes Switch 
        #include <iostream>
        using namespace std;
        int main()
        {
    int number;
    cout << "Give a number to determine its shape \n";
    cin >> number;

    switch (number)
    {
    case 3:
        cout << "Triangle";
        break;
    case 4:
        cout << "Square/Rectangle";
        break;
    case 5:
        cout << "Pentagon";
        break;
    case 6:
        cout << "Hexagon";
        break;
    case 7:
        cout << "Heptagon";
        break;
    case 8:
        cout << "Octagon";
        break;
    case 9:
        cout << "Nonagon";
        break;
    case 10:
        cout << "Decagon";
        break;
    default:
        cout << "Invalid \n";
        break;
    }

    }
    
    
## Grades
        #include <iostream>
        #include <string>
        using namespace std;
        int main()
        {
    string name;
    string lastname;
    int grade;

    cout << "Enter student's first name \n";
    cin >> name;
    cout << "Enter student's last name: \n";
    cin >> lastname;
    cout << "Enter the grade of " << name << " " << lastname << " to determine its mark. \n";
    cout << "Enter [1] If score is more than 70% \n";
    cout << "Enter [2] If score is 69-60% \n";
    cout << "Enter [3] If score is 59-50% \n";
    cout << "Enter [4] If score is 49-40% \n";
    cout << "Enter [5] If score is less than 39% \n";
    cin >> grade;
    
    switch (grade)
    {
    case 1:
        cout << name << " " << lastname << ", A";
        break;
    case 2:
        cout << name << " " << lastname << ", B";
        break;
    case 3:
        cout << name << " " << lastname << ", C";
        break;
    case 4:
        cout << name << " " << lastname << ", D";
        break;
    case 5:
        cout << name << " " << lastname << ", F";
        break;
    default:
        cout << "Invalid input. \n";
    }
        }

## Grades 2.0 (User can input full name)
        #include <iostream>
        #include <string>
        using namespace std;
        int main()
        {
    string name;
    int grade;

    cout << "Enter student's full name: \n";
    getline(cin, name);
    cout << "Enter the grade of " << name << " to determine its mark. \n";
    cout << "Enter [1] If score is more than 70% \n";
    cout << "Enter [2] If score is 69-60% \n";
    cout << "Enter [3] If score is 59-50% \n";
    cout << "Enter [4] If score is 49-40% \n";
    cout << "Enter [5] If score is less than 39% \n";
    cin >> grade;

    switch (grade)
    {
    case 1:
        cout << name << "- A";
        break;
    case 2:
        cout << name <<  "- B";
        break;
    case 3:
        cout << name <<  "- C";
        break;
    case 4:
        cout << name <<  "- D";
        break;
    case 5:
        cout << name << "- F";
        break;
    default:
        cout << "Invalid input. \n";
    }

        }
