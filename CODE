#include <iostream>
#include <string>

using namespace std;

class library {
    string user;
    string admin;
};
class user : public library {
public:
    void displayRole() {
        cout << "User role\n";
    }
    void processChoice() {
        int rentalDuration; 
        int yesorno;
        int option;
        int booktype;
        bool validChoice = false;
        string enteruser;

        cout << "Please enter your username: "; 
        cin >> enteruser; 

        while (!validChoice) {
            cout << "welcome to our library press 1 to continue" << endl;
            cin >> option;

            if (option >= 1 && option <= 2) {
                validChoice = true;
                switch (option) {
                case 1:
                    cout << "select book type" << endl;
                    break;
                }
            }
            else {
                cout << "Invalid choice, please try again." << endl;
            }
        }
        int bookchoice;
        validChoice = false;
        while (!validChoice) {
            cout << "1. Fantastic \n2. Drama \n3. Horror \n4. Comedy \n";
            cout << "select type: ";
            cin >> booktype;

            if (booktype >= 1 && booktype <= 4) {
                validChoice = true;
                switch (booktype) {
                case 1:
                    cout << "You have chosen the fantasy genre." << endl;
                    cout << "Fantasy books:" << endl;
                    cout << "1. Harry Potter" << endl;
                    cout << "2. Lord of the Rings" << endl;
                    cout << "3. Dragon Tattoo Girl" << endl;
                    cout << "4. Percy Jackson" << endl;
                    cout << "5. His Dark Materials" << endl;
                    break;
                case 2:
                    cout << "You have chosen the drama genre." << endl;
                    cout << "Drama books:" << endl;
                    cout << "1. Wuthering Heights" << endl;
                    cout << "2. Anna Karenina" << endl;
                    cout << "3. Red Monday" << endl;
                    cout << "4. Of Mice and Men" << endl;
                    cout << "5. Gonulcelen" << endl;
                    break;
                case 3:
                    cout << "You have chosen the horror genre." << endl;
                    cout << "Horror books:" << endl;
                    cout << "1. Dracula" << endl;
                    cout << "2. In Praise of Hell" << endl;
                    cout << "3. Haunting of Hill House" << endl;
                    cout << "4. Salem's Lot" << endl;
                    cout << "5. Shining" << endl;
                    break;
                case 4:
                    cout << "You have chosen the comedy genre." << endl;
                    cout << "Comedy books:" << endl;
                    cout << "1. Hitchhiker's Guide to the Galaxy" << endl;
                    cout << "2. Three Men in a Boat" << endl;
                    cout << "3. Diary of a Wimpy Kid" << endl;
                    cout << "4. Bridget Jones's Diary" << endl;
                    cout << "5. Catch-22" << endl;
                    break;
                }
            }
            else {
                cout << "Invalid selection, please try again." << endl;
            }
        }
        validChoice = false;
        while (!validChoice) {
            cout << "Please choose a book (1-5): ";
            cin >> bookchoice;

            if (bookchoice >= 1 && bookchoice <= 5) {
                validChoice = true;
            }
            else {
                cout << "Invalid choice, please select a book between 1 and 5." << endl;
            }
        }
        switch (option) {
        case 1: {
            while (true) {
                cout << "Enter the rental period (days): ";
                cin >> rentalDuration;

                if (rentalDuration > 30) {
       cout<< "If you do not return the product within" <<rentalDuration<<" days, a penalty of 5 dollars will be applied." << endl;
       cout << "Please return within 30 days.Please enter a new deadline." << endl;

                }
                else {
                    cout << "Product return within the time period we want (0-30)." << endl;
                    break;
                }
            }
            break;
        }
        case 2: {
            break;
        }
        default:
            cout << "Invalid election\n";
        }
        switch (option) {
        case 1: {
            while (true) {
                cout << " press 1 if you want to buy the product or press 2 if not" << endl;
                cin >> yesorno;

                bool validChoice = false;

                while (!validChoice) {
                   
                    if (yesorno == 1) {
                        cout << "Product received." << endl;
                        validChoice = true;
                    }
                    else if (yesorno == 2) {
                        cout << "Product not received." << endl;
                        validChoice = true;
                    }
                    else {
                        cout << "Invalid selection, please try again." << endl;
                    }
                }
                break;
            }
        case 2: {
            break;
        }
        default:
            cout << "Invalid election\n";
        }
        }
    }
};
class admin : public user {
public:
    void displayRole(bool isAdmin) {
        if (isAdmin) {
            cout << "Admin role\n";
        }
        else {
            cout << "User role\n";
        }
    }

    void processAdminChoice() {
        string bookinfo;
        string userinfo;
        int option;

        cout << "1.Add a book \n 2.Block user \n";
        cout << "Please make your choice: ";
        cin >> option;

        switch (option) {
        case 1:
            cout << "Selected book addition process." << endl;
          
            cout << "Enter book title and author: ";
            cin >> bookinfo;
            cout << "Book successfully added." << endl;
            break;
        case 2:
            cout << "User blocking process selected." << endl;
            cout << "Enter username: ";
            cin >> userinfo;
            cout << "User blocked." << endl;
            break;
        default:
            cout << "Invalid selection. Please enter 1 or 2." << endl;
        }
    }
};

int main() {
    admin nesne1;
    int choice;
    bool validChoice = false;

    bool isAdmin = false; 

    while (!validChoice) {
        cout << "Press 0 for User and 9 for Admin: ";
        cin >> choice;

        if (choice == 0) {
            nesne1.processChoice();
            validChoice = true;
        }
        else if (choice == 9) {
            isAdmin = true;
            nesne1.processAdminChoice();
            validChoice = true;
        }
        else {
            cout << "Invalid election\n";
        }
    }

    nesne1.displayRole(isAdmin);

    return 0;
}
