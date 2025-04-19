#include <iostream>
#include <string.h>
#include <unistd.h>
#include <windows.h>
#include <mysql.h>
#include <mysqld_error.h>
#include <conio.h>
#include <fstream>
#include <vector>

using namespace std;
struct User {
    string username;
    string password;
};

string HOST[] = "localhost";
string PASSWORD[] = "gerbolingo";


void userpage();
void subscore();
void createUser();
void updateUser();
void deleteUser();
void selectUser();
//user account
string username = "marky";
string userpass = "s240112354";


//admin
string name;
string adminname = "mark";
string pass, adminpass = "alcayde";

bool closeprog = false;
void adminpage(){
	int choice;
   system("cls");
   cout << "Hello admin, " << adminname << endl;


      while(!closeprog){
	  
        cout << "\n\t\t1. View Student";
        cout << "\n\t\t2. Create User";
        cout << "\n\t\t3. Update Password";
        cout << "\n\t\t4. Delete User";
        cout << "\n\t\t5. Logout" << endl;
        cout << "Choice: ";

        cin >> choice;

        switch (choice) {
            case 1: 
                  closeprog = true;
			      selectUser(); break;
            case 2: 
            closeprog = true;
			createUser(); break;
            case 3: 
			closeprog = true;
			updateUser(); break;
            case 4:
			closeprog = true;
			deleteUser(); break;
            case 5: break; 
            default: cout << "\n\t\tInvalid choice.\n"; system("pause");
        }
    }

   
}

void selectUser(){
	
}


void createUser(){
	
}

void updateUser(){
	
}

void deleteUser(){
	
}

	
//subject menu and subject taken
bool exitprog = false, comprog_taken = false, purcomm_taken = false, pathfit_taken = false, nstp_taken = false, fildis_taken = false, artapp_taken = false, sts_taken = false, ethics_taken = false, discrete_taken = false;
//global name

// student number

char ch;
// subject scores
	int comprog_score = 0, purcomm_score = 0, pathfit_score = 0, nstp_score = 0, fildis_score = 0, artapp_score = 0, sts_score = 0, ethics_score = 0, discrete_score = 0;

void loadingScreen() {
	HANDLE h = GetStdHandle(STD_OUTPUT_HANDLE);
SetConsoleTextAttribute(h,14);
  cout << "\n\n\n";
  cout << "\t\t\t                 *                      *                                *                      *                     *                 *                           " << endl;
  cout << "\t\t\t                               *                          *                      *                            *            *                   *             " << endl; 
  cout << "\t\t\t                                               *                    *                        *                                     *                      " << endl;
  cout << "\t\t\t                         *                                   *                                       *                   *                   *               " << endl;
  cout << "\t\t\t             *                      *               *                        *            *                     *                 *                  *         \n" << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t                                              ccee88oo                                                     ccee88oo" << endl;
  cout << "\t\t\t                                           C8O8O8Q8PoOb o8o                                             C8O8O8Q8PoOb o8o" << endl;
  cout << "\t\t\t                                        dOB69QO8PdUOpugoO9bD                                         dOB69QO8PdUOpugoO9bD" << endl;
  cout << "\t\t\t                                      CgggbU8OU qOp qOdoUOdcboo                                    CgggbU8OU qOp qOdoUOdcboo" << endl;
  cout << "\t\t\t                                          6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t                                              \\//  ////                                                   \\//  /////" << endl;
  cout << "\t\t\t                                               \\//////                                                      \\//////" << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t               ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo   " << endl;
  cout << "\t\t\t            C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o" << endl;
  cout << "\t\t\t         dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD" << endl;
  cout << "\t\t\t       CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....           ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....          ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo" << endl;
  cout << "\t\t\t           6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t               \\//  ////                                                    \\//  ////                                                    \\//  ////" << endl;
  cout << "\t\t\t                \\//////                                                      \\//////                                                      \\//////" << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t           .....//||||....                                              .....//||||....                                              .....//||||...." << endl;
  SetConsoleTextAttribute(h,3);
  cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n\n";
  SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t   --      --      --      --      --      --      --      --      --      --      --      --      --      --      --      --      --      --   \n\n\n\n" << endl;
  SetConsoleTextAttribute(h,3);
  cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n";  
  SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t\t\t\t\t\t\t\t      PRESS ENTER TO START! ";
  cin.get();
  SetConsoleTextAttribute(h,15);
  system("cls");
SetConsoleTextAttribute(h,14);
  cout << "\n\n\n";
  cout << "\t\t\t                 *                      *                                *                      *                     *                 *                           " << endl;
  cout << "\t\t\t                               *                          *                      *                            *            *                   *             " << endl; 
  cout << "\t\t\t                                               *                    *                        *                                     *                      " << endl;
  cout << "\t\t\t                         *                                   *                                       *                   *                   *               " << endl;
  cout << "\t\t\t             *                      *               *                        *            *                     *                 *                  *         \n" << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t                                              ccee88oo                                                     ccee88oo" << endl;
  cout << "\t\t\t                                           C8O8O8Q8PoOb o8o                                             C8O8O8Q8PoOb o8o" << endl;
  cout << "\t\t\t                                        dOB69QO8PdUOpugoO9bD                                         dOB69QO8PdUOpugoO9bD" << endl;
  cout << "\t\t\t                                      CgggbU8OU qOp qOdoUOdcboo                                    CgggbU8OU qOp qOdoUOdcboo" << endl;
  cout << "\t\t\t                                          6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t                                              \\//  ////                                                   \\//  /////" << endl;
  cout << "\t\t\t                                               \\//////                                                      \\//////" << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t               ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo   " << endl;
  cout << "\t\t\t            C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o" << endl;
  cout << "\t\t\t         dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD" << endl;
  cout << "\t\t\t       CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....           ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....          ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo" << endl;
  cout << "\t\t\t           6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t               \\//  ////                                                    \\//  ////                                                    \\//  ////" << endl;
  cout << "\t\t\t                \\//////                                                      \\//////                                                      \\//////" << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t           .....//||||....                                              .....//||||....                                              .....//||||...." << endl;
  SetConsoleTextAttribute(h,3);
  cout << "\t\t\t\t=================================================================================================================================================\n\n\n";
  SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t                                                     ________" << endl;
  cout << "\t\t\t\t                                                ____/__|___|_\\_____" << endl;
  SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t   --      --      --      --      --      --  ";
  SetConsoleTextAttribute(h,15);
  cout << "|  _          _    o|" << endl;
  cout << "\t\t\t\t                                               ='(_)--------(_)'===\n\n\n" << endl;
  SetConsoleTextAttribute(h,3);
  cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n";
  SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t\t\t\t\t\t\t\t      LOADING PLEASE WAIT.";
  sleep(1);
  system("cls");
  SetConsoleTextAttribute(h,14);
  cout << "\n\n\n";
  cout << "\t\t\t                           *                                *                      *                     *                 *                    *                       " << endl;
  cout << "\t\t\t                  *                          *                           *                       *               *                   *                                  " << endl; 
  cout << "\t\t\t                                      *                       *                *                                          *                  *                          " << endl;
  cout << "\t\t\t             *                                        *                                    *                 *                   *                *                     " << endl;
  cout << "\t\t\t                          *               *                        *            *               *                 *                      *               *           \n" << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t               ccee88oo                                                     ccee88oo                                                     ccee88oo" << endl;
  cout << "\t\t\t            C8O8O8Q8PoOb o8o                                             C8O8O8Q8PoOb o8o                                             C8O8O8Q8PoOb o8o" << endl;
  cout << "\t\t\t         dOB69QO8PdUOpugoO9bD                                         dOB69QO8PdUOpugoO9bD                                         dOB69QO8PdUOpugoO9bD" << endl;
  cout << "\t\t\t       CgggbU8OU qOp qOdoUOdcboo                                    CgggbU8OU qOp qOdoUOdcboo                                    CgggbU8OU qOp qOdoUOdcboo" << endl;
  cout << "\t\t\t           6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t               \\//  ////                                                   \\//   ////                                                   \\//   ////" << endl;
  cout << "\t\t\t                \\//////                                                      \\//////                                                      \\//////" << endl;
  cout << "\t\t\t                 |||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       " << endl;
  cout << "\t\t\t                 |||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    " << endl;
  cout << "\t\t\t                 |||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 " << endl;
  cout << "\t\t\t           .....//||||....           ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....           ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....          " << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t                                         6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t                                             \\//  ////                                                    \\//  ////" << endl;
  cout << "\t\t\t                                               \\//////                                                      \\//////" << endl;
  cout << "\t\t\t                                                |||||                                                        ||||| " << endl;
  cout << "\t\t\t                                                |||||                                                        ||||| " << endl;
  cout << "\t\t\t                                                |||||                                                        ||||| " << endl;
  cout << "\t\t\t                                          .....//||||....                                              .....//||||...." << endl;
  SetConsoleTextAttribute(h,3);
  cout << "\t\t\t\t=================================================================================================================================================\n\n\n";
  SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t                                                             ________" << endl;
  cout << "\t\t\t\t                                                        ____/__|___|_\\_____" << endl;
  SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t   --      --      --      --      --      --      --  ";
  SetConsoleTextAttribute(h,15);
  cout << "|  _          _    o|" << endl;
  cout << "\t\t\t\t                                                       ='(_)--------(_)'===\n\n\n" << endl;
  SetConsoleTextAttribute(h,3);
cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n";  
SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t\t\t\t\t\t\t\t      LOADING PLEASE WAIT..";
sleep(1);
  system("cls");
SetConsoleTextAttribute(h,14);
  cout << "\n\n\n";
  cout << "\t\t\t                 *                      *                                *                      *                     *                 *                           " << endl;
  cout << "\t\t\t                               *                          *                      *                            *            *                   *             " << endl; 
  cout << "\t\t\t                                               *                    *                        *                                     *                      " << endl;
  cout << "\t\t\t                         *                                   *                                       *                   *                   *               " << endl;
  cout << "\t\t\t             *                      *               *                        *            *                     *                 *                  *         \n" << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t                                              ccee88oo                                                     ccee88oo" << endl;
  cout << "\t\t\t                                           C8O8O8Q8PoOb o8o                                             C8O8O8Q8PoOb o8o" << endl;
  cout << "\t\t\t                                        dOB69QO8PdUOpugoO9bD                                         dOB69QO8PdUOpugoO9bD" << endl;
  cout << "\t\t\t                                      CgggbU8OU qOp qOdoUOdcboo                                    CgggbU8OU qOp qOdoUOdcboo" << endl;
  cout << "\t\t\t                                          6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t                                              \\//  ////                                                   \\//  /////" << endl;
  cout << "\t\t\t                                               \\//////                                                      \\//////" << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t               ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo   " << endl;
  cout << "\t\t\t            C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o" << endl;
  cout << "\t\t\t         dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD" << endl;
  cout << "\t\t\t       CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....           ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....          ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo" << endl;
  cout << "\t\t\t           6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t               \\//  ////                                                    \\//  ////                                                    \\//  ////" << endl;
  cout << "\t\t\t                \\//////                                                      \\//////                                                      \\//////" << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t           .....//||||....                                              .....//||||....                                              .....//||||...." << endl;
  SetConsoleTextAttribute(h,3);
  cout << "\t\t\t\t=================================================================================================================================================\n\n\n";
  SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t                                                                    ________" << endl;
  cout << "\t\t\t\t                                                               ____/__|___|_\\_____" << endl;
  SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t   --      --      --      --      --      --      --     EVAL";
  SetConsoleTextAttribute(h,15);
  cout << "|  _          _    o|" << endl;
  cout << "\t\t\t\t                                                              ='(_)--------(_)'===\n\n\n" << endl;
  SetConsoleTextAttribute(h,3);
cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n";  
SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t\t\t\t\t\t\t\t      LOADING PLEASE WAIT...";
sleep(1);
  system("cls");
  SetConsoleTextAttribute(h,14);
  cout << "\n\n\n";
  cout << "\t\t\t                           *                                *                      *                     *                 *                    *                       " << endl;
  cout << "\t\t\t                  *                          *                           *                       *               *                   *                                  " << endl; 
  cout << "\t\t\t                                      *                       *                *                                          *                  *                          " << endl;
  cout << "\t\t\t             *                                        *                                    *                 *                   *                *                     " << endl;
  cout << "\t\t\t                          *               *                        *            *               *                 *                      *               *           \n" << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t               ccee88oo                                                     ccee88oo                                                     ccee88oo" << endl;
  cout << "\t\t\t            C8O8O8Q8PoOb o8o                                             C8O8O8Q8PoOb o8o                                             C8O8O8Q8PoOb o8o" << endl;
  cout << "\t\t\t         dOB69QO8PdUOpugoO9bD                                         dOB69QO8PdUOpugoO9bD                                         dOB69QO8PdUOpugoO9bD" << endl;
  cout << "\t\t\t       CgggbU8OU qOp qOdoUOdcboo                                    CgggbU8OU qOp qOdoUOdcboo                                    CgggbU8OU qOp qOdoUOdcboo" << endl;
  cout << "\t\t\t           6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t               \\//  ////                                                   \\//   ////                                                   \\//   ////" << endl;
  cout << "\t\t\t                \\//////                                                      \\//////                                                      \\//////" << endl;
  cout << "\t\t\t                 |||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       " << endl;
  cout << "\t\t\t                 |||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    " << endl;
  cout << "\t\t\t                 |||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 " << endl;
  cout << "\t\t\t           .....//||||....           ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....           ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....          " << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t                                         6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t                                             \\//  ////                                                    \\//  ////" << endl;
  cout << "\t\t\t                                               \\//////                                                      \\//////" << endl;
  cout << "\t\t\t                                                |||||                                                        ||||| " << endl;
  cout << "\t\t\t                                                |||||                                                        ||||| " << endl;
  cout << "\t\t\t                                                |||||                                                        ||||| " << endl;
  cout << "\t\t\t                                          .....//||||....                                              .....//||||...." << endl;
  SetConsoleTextAttribute(h,3);
  cout << "\t\t\t\t=================================================================================================================================================\n\n\n";
  SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t                                                                           ________" << endl;
  cout << "\t\t\t\t                                                                      ____/__|___|_\\_____" << endl;
  SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t   --      --      --      --      --      --      --     EVALUATION ";
  SetConsoleTextAttribute(h,15);
  cout <<"|  _          _    o|" << endl;
  cout << "\t\t\t\t                                                                     ='(_)--------(_)'===\n\n\n" << endl;
  SetConsoleTextAttribute(h,3);
cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n";  
SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t\t\t\t\t\t\t\t      LOADING PLEASE WAIT.";
sleep(1);
  system("cls");
SetConsoleTextAttribute(h,14);
  cout << "\n\n\n";
  cout << "\t\t\t                 *                      *                                *                      *                     *                 *                           " << endl;
  cout << "\t\t\t                               *                          *                      *                            *            *                   *             " << endl; 
  cout << "\t\t\t                                               *                    *                        *                                     *                      " << endl;
  cout << "\t\t\t                         *                                   *                                       *                   *                   *               " << endl;
  cout << "\t\t\t             *                      *               *                        *            *                     *                 *                  *         \n" << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t                                              ccee88oo                                                     ccee88oo" << endl;
  cout << "\t\t\t                                           C8O8O8Q8PoOb o8o                                             C8O8O8Q8PoOb o8o" << endl;
  cout << "\t\t\t                                        dOB69QO8PdUOpugoO9bD                                         dOB69QO8PdUOpugoO9bD" << endl;
  cout << "\t\t\t                                      CgggbU8OU qOp qOdoUOdcboo                                    CgggbU8OU qOp qOdoUOdcboo" << endl;
  cout << "\t\t\t                                          6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t                                              \\//  ////                                                   \\//  /////" << endl;
  cout << "\t\t\t                                               \\//////                                                      \\//////" << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t               ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo   " << endl;
  cout << "\t\t\t            C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o" << endl;
  cout << "\t\t\t         dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD" << endl;
  cout << "\t\t\t       CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....           ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....          ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo" << endl;
  cout << "\t\t\t           6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t               \\//  ////                                                    \\//  ////                                                    \\//  ////" << endl;
  cout << "\t\t\t                \\//////                                                      \\//////                                                      \\//////" << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t           .....//||||....                                              .....//||||....                                              .....//||||...." << endl;
  SetConsoleTextAttribute(h,3);
  cout << "\t\t\t\t=================================================================================================================================================\n\n\n";
  SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t                                                                                 ________" << endl;
  cout << "\t\t\t\t                                                                            ____/__|___|_\\_____" << endl;
   SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t   --      --      --      --      --      --      --     EVALUATION FOR TH";
   SetConsoleTextAttribute(h,15);
  cout << "|  _          _    o|" << endl;
  cout << "\t\t\t\t                                                                           ='(_)--------(_)'===\n\n\n" << endl;
  SetConsoleTextAttribute(h,3);
cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n";  
SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t\t\t\t\t\t\t\t      LOADING PLEASE WAIT..";
sleep(1);
  system("cls");
  SetConsoleTextAttribute(h,14);
  cout << "\n\n\n";
  cout << "\t\t\t                           *                                *                      *                     *                 *                    *                       " << endl;
  cout << "\t\t\t                  *                          *                           *                       *               *                   *                                  " << endl; 
  cout << "\t\t\t                                      *                       *                *                                          *                  *                          " << endl;
  cout << "\t\t\t             *                                        *                                    *                 *                   *                *                     " << endl;
  cout << "\t\t\t                          *               *                        *            *               *                 *                      *               *           \n" << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t               ccee88oo                                                     ccee88oo                                                     ccee88oo" << endl;
  cout << "\t\t\t            C8O8O8Q8PoOb o8o                                             C8O8O8Q8PoOb o8o                                             C8O8O8Q8PoOb o8o" << endl;
  cout << "\t\t\t         dOB69QO8PdUOpugoO9bD                                         dOB69QO8PdUOpugoO9bD                                         dOB69QO8PdUOpugoO9bD" << endl;
  cout << "\t\t\t       CgggbU8OU qOp qOdoUOdcboo                                    CgggbU8OU qOp qOdoUOdcboo                                    CgggbU8OU qOp qOdoUOdcboo" << endl;
  cout << "\t\t\t           6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t               \\//  ////                                                   \\//   ////                                                   \\//   ////" << endl;
  cout << "\t\t\t                \\//////                                                      \\//////                                                      \\//////" << endl;
  cout << "\t\t\t                 |||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       " << endl;
  cout << "\t\t\t                 |||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    " << endl;
  cout << "\t\t\t                 |||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 " << endl;
  cout << "\t\t\t           .....//||||....           ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....           ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....          " << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t                                         6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t                                             \\//  ////                                                    \\//  ////" << endl;
  cout << "\t\t\t                                               \\//////                                                      \\//////" << endl;
  cout << "\t\t\t                                                |||||                                                        ||||| " << endl;
  cout << "\t\t\t                                                |||||                                                        ||||| " << endl;
  cout << "\t\t\t                                                |||||                                                        ||||| " << endl;
  cout << "\t\t\t                                          .....//||||....                                              .....//||||...." << endl;
  SetConsoleTextAttribute(h,3);
  cout << "\t\t\t\t=================================================================================================================================================\n\n\n";
  SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t                                                                                       ________" << endl;
  cout << "\t\t\t\t                                                                                  ____/__|___|_\\_____" << endl;
   SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t   --      --      --      --      --      --      --     EVALUATION FOR THE HIGH";
   SetConsoleTextAttribute(h,15);
  cout <<"|  _          _    o|" << endl;
  cout << "\t\t\t\t                                                                                 ='(_)--------(_)'===\n\n\n" << endl;
  SetConsoleTextAttribute(h,3);
cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n";  
SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t\t\t\t\t\t\t\t      LOADING PLEASE WAIT...";
sleep(1);
  system("cls");
SetConsoleTextAttribute(h,14);
  cout << "\n\n\n";
  cout << "\t\t\t                 *                      *                                *                      *                     *                 *                           " << endl;
  cout << "\t\t\t                               *                          *                      *                            *            *                   *             " << endl; 
  cout << "\t\t\t                                               *                    *                        *                                     *                      " << endl;
  cout << "\t\t\t                         *                                   *                                       *                   *                   *               " << endl;
  cout << "\t\t\t             *                      *               *                        *            *                     *                 *                  *         \n" << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t                                              ccee88oo                                                     ccee88oo" << endl;
  cout << "\t\t\t                                           C8O8O8Q8PoOb o8o                                             C8O8O8Q8PoOb o8o" << endl;
  cout << "\t\t\t                                        dOB69QO8PdUOpugoO9bD                                         dOB69QO8PdUOpugoO9bD" << endl;
  cout << "\t\t\t                                      CgggbU8OU qOp qOdoUOdcboo                                    CgggbU8OU qOp qOdoUOdcboo" << endl;
  cout << "\t\t\t                                          6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t                                              \\//  ////                                                   \\//  /////" << endl;
  cout << "\t\t\t                                               \\//////                                                      \\//////" << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t               ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo   " << endl;
  cout << "\t\t\t            C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o" << endl;
  cout << "\t\t\t         dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD" << endl;
  cout << "\t\t\t       CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....           ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....          ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo" << endl;
  cout << "\t\t\t           6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t               \\//  ////                                                    \\//  ////                                                    \\//  ////" << endl;
  cout << "\t\t\t                \\//////                                                      \\//////                                                      \\//////" << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t           .....//||||....                                              .....//||||....                                              .....//||||...." << endl;
  SetConsoleTextAttribute(h,3);
  cout << "\t\t\t\t=================================================================================================================================================\n\n\n";
  SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t                                                                                             ________" << endl;
  cout << "\t\t\t\t                                                                                        ____/__|___|_\\_____" << endl;
   SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t   --      --      --      --      --      --      --     EVALUATION FOR THE HIGHER UPS";
   SetConsoleTextAttribute(h,15);
  cout <<"|  _          _    o|" << endl;
  cout << "\t\t\t\t                                                                                       ='(_)--------(_)'===\n\n\n" << endl;
  SetConsoleTextAttribute(h,3);
cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n";  
SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t\t\t\t\t\t\t\t      LOADING PLEASE WAIT.";
sleep(1);
  system("cls");
  SetConsoleTextAttribute(h,14);
  cout << "\n\n\n";
  cout << "\t\t\t                           *                                *                      *                     *                 *                    *                       " << endl;
  cout << "\t\t\t                  *                          *                           *                       *               *                   *                                  " << endl; 
  cout << "\t\t\t                                      *                       *                *                                          *                  *                          " << endl;
  cout << "\t\t\t             *                                        *                                    *                 *                   *                *                     " << endl;
  cout << "\t\t\t                          *               *                        *            *               *                 *                      *               *           \n" << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t               ccee88oo                                                     ccee88oo                                                     ccee88oo" << endl;
  cout << "\t\t\t            C8O8O8Q8PoOb o8o                                             C8O8O8Q8PoOb o8o                                             C8O8O8Q8PoOb o8o" << endl;
  cout << "\t\t\t         dOB69QO8PdUOpugoO9bD                                         dOB69QO8PdUOpugoO9bD                                         dOB69QO8PdUOpugoO9bD" << endl;
  cout << "\t\t\t       CgggbU8OU qOp qOdoUOdcboo                                    CgggbU8OU qOp qOdoUOdcboo                                    CgggbU8OU qOp qOdoUOdcboo" << endl;
  cout << "\t\t\t           6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t               \\//  ////                                                   \\//   ////                                                   \\//   ////" << endl;
  cout << "\t\t\t                \\//////                                                      \\//////                                                      \\//////" << endl;
  cout << "\t\t\t                 |||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       " << endl;
  cout << "\t\t\t                 |||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    " << endl;
  cout << "\t\t\t                 |||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 " << endl;
  cout << "\t\t\t           .....//||||....           ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....           ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....          " << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t                                         6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t                                             \\//  ////                                                    \\//  ////" << endl;
  cout << "\t\t\t                                               \\//////                                                      \\//////" << endl;
  cout << "\t\t\t                                                |||||                                                        ||||| " << endl;
  cout << "\t\t\t                                                |||||                                                        ||||| " << endl;
  cout << "\t\t\t                                                |||||                                                        ||||| " << endl;
  cout << "\t\t\t                                          .....//||||....                                              .....//||||...." << endl;
  SetConsoleTextAttribute(h,3);
  cout << "\t\t\t\t=================================================================================================================================================\n\n\n";
  SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t                                                                                                      ________" << endl;
  cout << "\t\t\t\t                                                                                                 ____/__|___|_\\____" << endl;
   SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t   --      --      --      --      --      --      --     EVALUATION FOR THE HIGHER UPS    --  ";
   SetConsoleTextAttribute(h,15);
  cout << " |  _          _    o|" << endl;
  cout << "\t\t\t\t                                                                                                ='(_)--------(_)'===\n\n\n" << endl;
  SetConsoleTextAttribute(h,3);
cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n";  
SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t\t\t\t\t\t\t\t      LOADING PLEASE WAIT..";
sleep(1);
  system("cls");
SetConsoleTextAttribute(h,14);
  cout << "\n\n\n";
  cout << "\t\t\t                 *                      *                                *                      *                     *                 *                           " << endl;
  cout << "\t\t\t                               *                          *                      *                            *            *                   *             " << endl; 
  cout << "\t\t\t                                               *                    *                        *                                     *                      " << endl;
  cout << "\t\t\t                         *                                   *                                       *                   *                   *               " << endl;
  cout << "\t\t\t             *                      *               *                        *            *                     *                 *                  *         \n" << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t                                              ccee88oo                                                     ccee88oo" << endl;
  cout << "\t\t\t                                           C8O8O8Q8PoOb o8o                                             C8O8O8Q8PoOb o8o" << endl;
  cout << "\t\t\t                                        dOB69QO8PdUOpugoO9bD                                         dOB69QO8PdUOpugoO9bD" << endl;
  cout << "\t\t\t                                      CgggbU8OU qOp qOdoUOdcboo                                    CgggbU8OU qOp qOdoUOdcboo" << endl;
  cout << "\t\t\t                                          6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t                                              \\//  ////                                                   \\//  /////" << endl;
  cout << "\t\t\t                                               \\//////                                                      \\//////" << endl;
  SetConsoleTextAttribute(h,2);
  cout << "\t\t\t               ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo                         ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                       ";
  SetConsoleTextAttribute(h,2);
  cout << "ccee88oo   " << endl;
  cout << "\t\t\t            C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o                    ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                    ";
  SetConsoleTextAttribute(h,2);
  cout << "C8O8O8Q8PoOb o8o" << endl;
  cout << "\t\t\t         dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD                   ";
  SetConsoleTextAttribute(h,6);
  cout << "|||||                 ";
  SetConsoleTextAttribute(h,2);
  cout << "dOB69QO8PdUOpugoO9bD" << endl;
  cout << "\t\t\t       CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....           ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo          ";
  SetConsoleTextAttribute(h,6);
  cout << ".....//||||....          ";
  SetConsoleTextAttribute(h,2);
  cout << "CgggbU8OU qOp qOdoUOdcboo" << endl;
  cout << "\t\t\t           6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP                                          6OuU   p u gcoUodpP" << endl;
  SetConsoleTextAttribute(h,6);
  cout << "\t\t\t               \\//  ////                                                    \\//  ////                                                    \\//  ////" << endl;
  cout << "\t\t\t                \\//////                                                      \\//////                                                      \\//////" << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t                 |||||                                                        |||||                                                        ||||| " << endl;
  cout << "\t\t\t           .....//||||....                                              .....//||||....                                              .....//||||...." << endl;
  SetConsoleTextAttribute(h,3);
  cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n\n";
  SetConsoleTextAttribute(h,15);
  cout << "\t\t\t\t   --      --      --      --      --      --      --     EVALUATION FOR THE HIGHER UPS    --      --      --      --      --      --      --   \n\n\n\n" << endl;
SetConsoleTextAttribute(h,3);
cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n";  
SetConsoleTextAttribute(h,15);
cout << "\t\t\t\t\t\t\t\t\t\t\t     PRESS ENTER TO CONTINUE";
cin.get();
SetConsoleTextAttribute(h,15);
system("cls");
}
void sub_grade() {
    char select;
    int comprog_grade = ((float)comprog_score / 5) * 50 + 50;
    int purcomm_grade = ((float)purcomm_score / 5) * 50 + 50;
    int pathfit_grade = ((float)pathfit_score / 5) * 50 + 50;
    int nstp_grade = ((float)nstp_score / 5) * 50 + 50;
    int fildis_grade = ((float)fildis_score / 5) * 50 + 50;
    int artapp_grade = ((float)pathfit_score / 5) * 50 + 50;
    int sts_grade = ((float)sts_score / 5) * 50 + 50;
    int ethics_grade = ((float)ethics_score / 5) * 50 + 50;
    int discrete_grade = ((float)discrete_score / 5) * 50 + 50;
    cout << "\tHere's your Grades of every subject:" << endl;
    cout << " Subject:\t\t\t\t\t";
    cout << "Grades:\n";
    cout << " Purposive Communication\t\t"<< purcomm_grade << "%" << endl;
    cout << " Art Appreciation\t" << artapp_grade << "%" << endl;
    cout << " Science, Technology and Society\t\t\t" << sts_grade << "%" << endl;
    cout << " Applied Ethics\t\t\t" << ethics_grade << "%" << endl;
    cout << " Discrete Mathematics\t\t\t" << discrete_grade << "%" << endl;
    cout << " Computer Programming 2\t\t\t" << comprog_grade << "%" << endl;
    cout << " Filipino sa iba't ibang Disiplina\t\t\t" << fildis_grade << "%" << endl;
    cout << " National Service Training Program\t\t\t" << nstp_grade << "%" << endl;
    cout << " PATHFIT2 \t\t\t" << pathfit_grade << "%" << endl;
    cout << "(1 = back to subject selection, 2 = back to scores)" << endl;
    cout << "Choose: ";
    cin >> select;

    if(select == '1') {
        cout << "Returning to subject selection..." << endl;
        sleep(1.5);
        system("cls");
        exitprog = false;
        return;
    } else if(select == '2') {
        cout << "Returning to scores..." << endl;
        sleep(1.5);
        system("cls");
        subscore();
    } else {
        cout << "\nInvalid Operator!!" << endl;
    }
}

void fildis(){
	HANDLE h = GetStdHandle(STD_OUTPUT_HANDLE);
	char choose;
    system("cls");

    cout << "This is Filipino sa Iba't ibang Disiplina subject" << endl;
    cout << "1. Take an exam" << endl;
    cout << "2. Back" << endl;
    cout << "Choose: ";
    cin >> choose;

    if (choose == '1') {
        cout << "Exam's Starting, Goodluck..." << endl;
        sleep(1.5);
        system("cls");

        // Questions & Answers
        SetConsoleTextAttribute(h,5);
        cout << "\n                             ==================================================================================================================================================\n";
        cout << "\n\t\t\t\tDIRECTIONS: PLEASE READ EACH QUESTION CAREFULLY AND THINK BEFORE YOU ANSWER. MAKE SURE TO FOLLOW ALL INSTRUCTIONS GIVEN. ALL ANSWERS MUST BE \n\t\t\t\t    WRITTEN IN CAPITAL LETTERS ONLY. FAILURE TO DO SO MAY RESULT IN YOUR ANSWER BEING MARKED INCORRECT. TAKE YOUR TIME AND DO YOUR BEST!\n" << endl;
        cout << "                             ==================================================================================================================================================\n\n";
        SetConsoleTextAttribute(h,15);
        const int NUM_QUESTIONS = 25;
        string questions[NUM_QUESTIONS] = {
		"\t\t\t\t\t\t1. Ayon kay Patrick M. Malabo, 'Isang midyum at isang instrumento ang wika na nakatutulong sa komunikasyon, \n\t\t\t\t\t\t    pagpapalitan ng kaisipan, at pag-uunawaan ng tao.'\n\n\t\t\t\t\t\t\tA. TAMA\n\t\t\t\t\t\t\tB. MALI",
		"\t\t\t\t\t\t2. Wala nang pangangailangan para sa mga terminolohiyang medikal sa Wikang Filipino dahil ang Ingles ang \n\t\t\t\t\t\t    ginagamit na wika sa lahat ng medikal na larangan.\n\n\t\t\t\t\t\t\tA. TAMA\n\t\t\t\t\t\t\tB. MALI",
		"\t\t\t\t\t\t3. Binibigyang-diin ni Malabo na ang lahat ng terminolohiya sa accounting ay madaling maisasalin sa Wikang Filipino.\n\n\t\t\t\t\t\t\tA. TAMA\n\t\t\t\t\t\t\tB. MALI",
		"\t\t\t\t\t\t4. Ayon kay Perla S. Carpio (1939), 'The wisdom of the past is of value, when it is merge with the present. \n\t\t\t\t\t\t    Adherence to the past can cause death to progress and misery to the living.'\n\n\t\t\t\t\t\t\tA. TAMA\n\t\t\t\t\t\t\tB. MALI",
		"\t\t\t\t\t\t5. Ayon sa ilang eksperto, ang paggamit ng Wikang Filipino sa mga dokumento ng medisina ay naglalagay sa \n\t\t\t\t\t\t    panganib sa kalidad ng Impormasyon.\n\n\t\t\t\t\t\t\tA. TAMA\n\t\t\t\t\t\t\tB. MALI",
		"\t\t\t\t\t\t6. Ayon kay Patrick M. Malabo, makakatulong ang paggamit ng librong nakasulat sa Wikang Filipino sa mas madaling \n\t\t\t\t\t\t    pag-unawa ng mga konsepto sa accounting.\n\n\t\t\t\t\t\t\tA. TAMA\n\t\t\t\t\t\t\tB. MALI",
		"\t\t\t\t\t\t7. Ayon kay Carpio, ang kulturang popular ay hindi nakakaapekto sa mga kultural na identidad ng mga tao.\n\n\t\t\t\t\t\t\tA. TAMA\n\t\t\t\t\t\t\tB. MALI",
		"\t\t\t\t\t\t8. Ayon kay Sarah Boydon (2014), 'Ang pagkakaroon ng sariling wika ay masasabing katumbas ng pagkakaroon ng sariling \n\t\t\t\t\t\t    mga paa dahil ito ang tumatayong instrumento upang tayo'y magkaunawaan at magkaisa, kung saan ito ang unang \n\t\t\t\t\t\t     hakbang tungo sa kaunlaran.'\n\n\t\t\t\t\t\t\tA. TAMA\n\t\t\t\t\t\t\tB. MALI",
		"\t\t\t\t\t\t9. Sinasalamin ni Malabo ang potensyal ng lokal na wika sa pagpapayaman ng edukasyon sa accounting.\n\n\t\t\t\t\t\t\tA. TAMA\n\t\t\t\t\t\t\tB. MALI",
		"\t\t\t\t\t\t10. Isinasaad ni Perla S. Carpio na ang kulturang popular ay isang repleksyon ng mga karanasan at pananaw ng masa.\n\n\t\t\t\t\t\t\tA. TAMA\n\t\t\t\t\t\t\tB. MALI",
		"\t\t\t\t\t\t11. Ano ang pangunahing layunin ng alternatibong sistema ng pagkatuto sa edukasyon?\n\n\t\t\t\t\t\t\tA. Magturo ng mga tradisyonal na asignatura tulad ng matematika at agham\n\t\t\t\t\t\t\tB. Magtutok lamang sa mga  kabataang may mataas na marka\n\t\t\t\t\t\t\tC. Magbigay ng mga alternatibong paraan ng pagkatuto upang matugunan ang pangangailangan ng mga mag-aaral",
		"\t\t\t\t\t\t12. Siya ang nag aral hingil sa kaabisaan ng Wikang Filipino bilng panturo sa (ALS)\n\n\t\t\t\t\t\t\tA. Harty Aguilar\n\t\t\t\t\t\t\tB. Hermeline Aguilar\n\t\t\t\t\t\t\tC. Harline Aguilara",
		"\t\t\t\t\t\t13. Ano ang khulugan ng (EFA)\n\n\t\t\t\t\t\t\tA. Education For Age\n\t\t\t\t\t\t\tB. Education For All\n\t\t\t\t\t\t\tC. Education For Alternative",
		"\t\t\t\t\t\t14. Ito ng tinaguriang Millennium Development Goal ng Pilipinas\n\n\t\t\t\t\t\t\tA. ALS\n\t\t\t\t\t\t\tB. EFA\n\t\t\t\t\t\t\tC. ERA",
		"\t\t\t\t\t\t15. Taong ano isinaktuparan ang (ALS) sa kagawarad ng Edukasyon.\n\n\t\t\t\t\t\t\tA. 2004\n\t\t\t\t\t\t\tB. 2002\n\t\t\t\t\t\t\tC. 2003",
		"\t\t\t\t\t\t16. Taon nasakatuparan ang (EFA)\n\n\t\t\t\t\t\t\tA. 2014\n\t\t\t\t\t\t\tB. 2013\n\t\t\t\t\t\t\tC. 2015",
		"\t\t\t\t\t\t17. Ano ang kahulugan ng (ALS)\n\n\t\t\t\t\t\t\tA. Alternatibong Sistema ng Pagturo\n\t\t\t\t\t\t\tB. Alternatibong Sistema ng Pagkatuto\n\t\t\t\t\t\t\tC. Alternatibong Sistema ng Pag-unlad",
		"\t\t\t\t\t\t18. Siya ng gumawa ng pag-aaral hinggil sa pagsalin ng mga alintuntunin, panuto at direksyon.\n\n\t\t\t\t\t\t\tA. Angle Garatol\n\t\t\t\t\t\t\tB. Ranee Rose Garatol\n\t\t\t\t\t\t\tC. Rasty Garatol",
		"\t\t\t\t\t\t19. Ito ang Departamentong nag patupat ng ALS\n\n\t\t\t\t\t\t\tA. EFA\n\t\t\t\t\t\t\tB. CHED\n\t\t\t\t\t\t\tC. DepEd",
		"\t\t\t\t\t\t20. Departamento ng edukasyon\n\n\t\t\t\t\t\t\tA. DepEd\n\t\t\t\t\t\t\tB. ALS\n\t\t\t\t\t\t\tC. EFA",
		"\t\t\t\t\t\t21. Tuwing kailan nagaganap ang buwan ng wika?\n\n\t\t\t\t\t\t\tA. Agosto\n\t\t\t\t\t\t\tB. Hulyo\n\t\t\t\t\t\t\tC. Hunyo",
		"\t\t\t\t\t\t22. Anong wika ang sinasabing mabisang panturo sa ALS?\n\n\t\t\t\t\t\t\tA. Ingles\n\t\t\t\t\t\t\tB. Filipino\n\t\t\t\t\t\t\tC. Pilipino",
		"\t\t\t\t\t\t23. Ang sumulat ang awitin na “Anak”\n\n\t\t\t\t\t\t\tA. Freddie Aguilar\n\t\t\t\t\t\t\tB. Gary Granada\n\t\t\t\t\t\t\tC. Gary Valenciano",
		"\t\t\t\t\t\t24. Ang awiting “Pablong Politaryo” ay sinulat ni?\n\n\t\t\t\t\t\t\tA. Tom Agulto\n\t\t\t\t\t\t\tB. Atom Agulto\n\t\t\t\t\t\t\tC. Pablo",
		"\t\t\t\t\t\t25. Anong aspeto ng buhay ang madalas pagtuunan ng pansin ni Gary Granada sa kanyang mga liriko?\n\n\t\t\t\t\t\t\tA.  Politika\n\t\t\t\t\t\t\tB. Pag-ibig\n\t\t\t\t\t\t\tC. Pamilya"
		};
        char correctAnswers[NUM_QUESTIONS] = {'B', 'B', 'B', 'B', 'B', 'A', 'B', 'A', 'A', 'A', 'C', 'B', 'B', 'B', 'C', 'C', 'B', 'B', 'C', 'A', 'A', 'B', 'A', 'A', 'A'};
        char userAnswers[NUM_QUESTIONS];

        
        for (int i = 0; i < NUM_QUESTIONS; i++) {
            cout << questions[i] << "\n\n\t\t\t\t\t\tAnswer: ";
            cin >> userAnswers[i];
            cout << "\n";
        }
        
        //  ==== Edit Answers =======!!
        
        
        char reviewChoice;
        int qNum;
        while (true) {

            cout << "\t\t\t\tWould you like to change an answer? (Y = Yes || N = No): ";
            cin >> reviewChoice;
            if (reviewChoice == 'N' || reviewChoice == 'n') {
                break;
            } else if(reviewChoice == 'Y' || reviewChoice == 'y'){
            cout << "\t\t\t\tEnter the question number to edit (1-" << NUM_QUESTIONS << "): ";
            cin >> qNum;
            
            if (qNum >= 1 && qNum <= NUM_QUESTIONS) {
                cout << "\n" << questions[qNum - 1] << "\n\n\t\t\t\t\t\tNew Answer: ";
                cin >> userAnswers[qNum - 1];
            } else {
                cout << "\t\t\t\tInvalid question number! Try again.\n";
            }
        }
        else{
        	cout << "\t\t\t\tInvalid choices!! Y = Yes || N = No" << endl;
		}
        }

        // Calculate Score
        for (int i = 0; i < NUM_QUESTIONS; i++) {
            if (toupper(userAnswers[i]) == correctAnswers[i]) {
                fildis_score++;
            }
        }

        system("cls");
        cout << "You completed the Filipino sa Iba't ibang Disiplina' exam!\n";
        cout << "Final Score: " << fildis_score << "/" << NUM_QUESTIONS << endl;
        cout << "Please wait...";
        sleep(3);
        fildis_taken = true;
        system("cls");
        exitprog = false;
        userpage();
        
    } else if (choose == '2') {
        cout << "Returning to Menu..." << endl;
        system("cls");
        sleep(1.5);
        exitprog = false;
        return;
    } else {
        cout << "INVALID, PLEASE CHOOSE 1 or 2" << endl;
    }
	
}

void nstp(){
	HANDLE h = GetStdHandle(STD_OUTPUT_HANDLE);
	cout << "NSTP TO!!";
}


void artapp(){
	HANDLE h = GetStdHandle(STD_OUTPUT_HANDLE);
	cout << "this is art app!!!";
}

void sts(){
	HANDLE h = GetStdHandle(STD_OUTPUT_HANDLE);
	char choose;
    system("cls");

    cout << "This is Science, Technology and Society subject" << endl;
    cout << "1. Take an exam" << endl;
    cout << "2. Back" << endl;
    cout << "Choose: ";
    cin >> choose;

    if (choose == '1') {
        cout << "Exam's Starting, Goodluck..." << endl;
        sleep(1.5);
        system("cls");

        // Questions & Answers
        SetConsoleTextAttribute(h,7);
        cout << "\n                             ==================================================================================================================================================\n";
        cout << "\n\t\t\t\tDIRECTIONS: PLEASE READ EACH QUESTION CAREFULLY AND THINK BEFORE YOU ANSWER. MAKE SURE TO FOLLOW ALL INSTRUCTIONS GIVEN. ALL ANSWERS MUST BE \n\t\t\t\t    WRITTEN IN CAPITAL LETTERS ONLY. FAILURE TO DO SO MAY RESULT IN YOUR ANSWER BEING MARKED INCORRECT. TAKE YOUR TIME AND DO YOUR BEST!\n" << endl;
        cout << "                             ==================================================================================================================================================\n\n";
        SetConsoleTextAttribute(h,15);
        const int NUM_QUESTIONS = 25;
        string questions[NUM_QUESTIONS] = {
		"\t\t\t\t\t\t1. Artificial Intelligence (Al) is capable of simulating human learning, problem-solving, and decision-making.\n\n\t\t\t\t\t\t\tA.TRUE\n\t\t\t\t\t\t\tB.FALSE",
		"\t\t\t\t\t\t2. Deep learning allows Al to make decisions independently and learn new tasks without human intervention.\n\n\t\t\t\t\t\t\tA.TRUE\n\t\t\t\t\t\t\tB.FALSE",
		"\t\t\t\t\t\t3. Artificial General Intelligence (AGI) is the only type of Al that currently exists and can perform tasks better than humans.\n\n\t\t\t\t\t\t\tA.TRUE\n\t\t\t\t\t\t\tB.FALSE",
		"\t\t\t\t\t\t4. Reactive Machine AI is capable of remembering past outcomes and using that data for future decisions.\n\n\t\t\t\t\t\t\tA.TRUE\n\t\t\t\t\t\t\tB.FALSE",
		"\t\t\t\t\t\t5. Super Al, once realized, would be capable of understanding human emotions and developing its own beliefs.\n\n\t\t\t\t\t\t\tA.TRUE\n\t\t\t\t\t\t\tB.FALSE",
		"\t\t\t\t\t\t6. Limited Memory Al can retain long-term memories and apply them over many years.\n\n\t\t\t\t\t\t\tA.TRUE\n\t\t\t\t\t\t\tB.FALSE",
		"\t\t\t\t\t\t7. The development of Artificial Neural Networks in 2012 allowed Al to simulate human brain functions more accurately.\n\n\t\t\t\t\t\t\tA.TRUE\n\t\t\t\t\t\t\tB.FALSE",
		"\t\t\t\t\t\t8. Question: According to Bill Joy, one of the potential risks of Al is that humans may become obsolete or extinct.\n\n\t\t\t\t\t\t\tA.TRUE\n\t\t\t\t\t\t\tB.FALSE",
		"\t\t\t\t\t\t9. Generative Al tools like ChatGPT and Bard are examples of Reactive Machine Al.\n\n\t\t\t\t\t\t\tA.TRUE\n\t\t\t\t\t\t\tB.FALSE",
		"\t\t\t\t\t\t10. Marx believed that if machines took over laborious tasks, humans would lose the ability to pursue meaningful activities.\n\n\t\t\t\t\t\t\tA.TRUE\n\t\t\t\t\t\t\tB.FALSE",
		"\t\t\t\t\t\t11. Which of the following is an example of Narrow Al? \n\n\t\t\t\t\t\t\tA. None of the choices\n\t\t\t\t\t\t\tB. IBM Watson\n\t\t\t\t\t\t\tC. A robot that can feel emotions\n\t\t\t\t\t\t\tD. A self-aware robot",
		"\t\t\t\t\t\t12. What is a significant challenge Bill Joy mentions in his article 'Why the Future Doesn't Need Us'?\n\n\t\t\t\t\t\t\tA. The extinction of human beings due to Al and other technologies\n\t\t\t\t\t\t\tB. The limited functionality of current Al\n\t\t\t\t\t\t\tC. The difficulty in building Super Al\n\t\t\t\t\t\t\tD. The risk of Al becoming economically obsolete",
		"\t\t\t\t\t\t13. How does Limited Memory Al improve over time? \n\n\t\t\t\t\t\t\tA. By retaining data and recalling it after years\n\t\t\t\t\t\t\tB. By becoming self-aware and making decisions independently\n\t\t\t\t\t\t\tC. By increasing processing speed\n\t\t\t\t\t\t\tD. By training on more data and refining its performance",
		"\t\t\t\t\t\t14. What term is used to describe Al that simulates human learning, problem-solving, and creativity?\n\n\t\t\t\t\t\t\tA. Artificial Intelligence\n\t\t\t\t\t\t\tB. Artificial General Intelligence\n\t\t\t\t\t\t\tC. Artificial Narrow Intelligence\n\t\t\t\t\t\t\tD. Deep Learning",
		"\t\t\t\t\t\t15. Which of the following is an example of Reactive Machine Al? \n\n\t\t\t\t\t\t\tA. ChatGPT \n\t\t\t\t\t\t\tB. IBM Deep Blue \n\t\t\t\t\t\t\tC. Self-driving cars \n\t\t\t\t\t\t\tD. Siri",
		"\t\t\t\t\t\t16. Which of the following tasks can Al perform? \n\n\t\t\t\t\t\t\tA. Performing tasks that require human intelligence, such as problem-solving \n\t\t\t\t\t\t\tB. Traveling through time \n\t\t\t\t\t\t\tC. Calculating distances faster than the speed of light \n\t\t\t\t\t\t\tD. Building human-like robots",
		"\t\t\t\t\t\t17. What type of Al can recall past events and outcomes? \n\n\t\t\t\t\t\t\tA. Limited Memory Al \n\t\t\t\t\t\t\tB. Reactive Machine Al \n\t\t\t\t\t\t\tC. Theory of Mind Al \n\t\t\t\t\t\t\tD. Super AI",
		"\t\t\t\t\t\t18. What is Artificial Intelligence (AI)? \n\n\t\t\t\t\t\t\tA. A machine that can repair itself without human intervention \n\t\t\t\t\t\t\tB. A system that allows humans to control computers remotely \n\t\t\t\t\t\t\tC. A program designed to generate random numbers \n\t\t\t\t\t\t\tD. Technology enabling computers and machines to simulate human capabilities",
		"\t\t\t\t\t\t19. Which of the following is NOT an example of Limited Memory Al? \n\n\t\t\t\t\t\t\tA. ChatGPT \n\t\t\t\t\t\t\tB. IBM Deep Blue \n\t\t\t\t\t\t\tC. Netflix recommendation engine \n\t\t\t\t\t\t\tD. Siri",
		"\t\t\t\t\t\t20. According to Marx's view, what is the potential benefit of machines performing all laborious tasks? \n\n\t\t\t\t\t\t\tA. Increased productivity \n\t\t\t\t\t\t\tB. Reducing the cost of labor \n\t\t\t\t\t\t\tC. Enhancing machine intelligence \n\t\t\t\t\t\t\tD. Freeing humans to engage in more meaningful self-fulfilling activities",
		"\t\t\t\t\t\t21. How might Marx's view of technological advancement differ from Bill Joy's perspective on Al, based on the provided text? \n\n\t\t\t\t\t\t\tA. Marx believed technological progress would lead to human redundancy, while Joy was more optimistic about Al enhancing productivity. \n\t\t\t\t\t\t\tB. Joy supported Marx's idea that machines will always work in human interests. \n\t\t\t\t\t\t\tC. Both Marx and Joy advocated for a future where machines and humans coexist in harmony. \n\t\t\t\t\t\t\tD. Marx viewed machines as liberating humans from labor, allowing them to pursue self-realization, while Joy feared Al could lead to human extinction.",
		"\t\t\t\t\t\t22. Which of the following best explains the potential implications of Artificial General Intelligence (AGI) for human society? \n\n\t\t\t\t\t\t\tA. AGI currently exists in advanced forms like ChatGPT and Siri. \n\t\t\t\t\t\t\tB.  AGI will be limited to solving specific tasks such as diagnosing diseases or playing chess. \n\t\t\t\t\t\t\tC. AGI will always require constant human supervision to make decisions. \n\t\t\t\t\t\t\tD. AGI, once developed, could perform any intellectual task a human can and adapt to new environments.",
		"\t\t\t\t\t\t23. Considering the advancements in Limited Memory Al, which of the following industries is most likely to benefit from this type of Al? \n\n\t\t\t\t\t\t\tA. Creative industries, where human emotions and expressions are critical. \n\t\t\t\t\t\t\tB. Autonomous driving, where real-time data processing and decision-making are essential. \n\t\t\t\t\t\t\tC. Historical research, due to its reliance on recalling past events. \n\t\t\t\t\t\t\tD. Manual labor, which requires repetitive physical tasks with minimal thinking.",
		"\t\t\t\t\t\t24. What might be the greatest challenge in the development of Super Al, according to the lesson? \n\n\t\t\t\t\t\t\tA. Creating Al that can learn specific tasks, such as playing games or recognizing faces. \n\t\t\t\t\t\t\tB. Ensuring that Super Al can understand and replicate human emotions, beliefs, and experiences. \n\t\t\t\t\t\t\tC. Developing enough data processing power to simulate human intelligence. \n\t\t\t\t\t\t\tD. Training Al to retain memory over long periods of time.",
		"\t\t\t\t\t\t25. Why might it be necessary to exercise caution when advancing Al technologies, according to Bill Joy's arguments? \n\n\t\t\t\t\t\t\tA. Al will always require human intervention, making its risks manageable. \n\t\t\t\t\t\t\tB. Al might replicate itself uncontrollably, leading to scenarios where human existence is threatened. \n\t\t\t\t\t\t\tC. Because machines may become economically beneficial, reducing the need for human workers. \n\t\t\t\t\t\t\tD. Because Al could enhance human creativity and autonomy.",
				};
        char correctAnswers[NUM_QUESTIONS] = {'A', 'A', 'B', 'B', 'A', 'B', 'A', 'A', 'B', 'B', 'B', 'A', 'D', 'A', 'B', 'A', 'A', 'D', 'B', 'D', 'D', 'D', 'B', 'B', 'B'};
        char userAnswers[NUM_QUESTIONS];

        // Ask Questions and Store Answers
        for (int i = 0; i < NUM_QUESTIONS; i++) {
            cout << questions[i] << "\n\n\t\t\t\t\t\tAnswer: ";
            cin >> userAnswers[i];
            cout << "\n";
        }
        
        // Review and Edit Answers
        
        
        char reviewChoice;
        int qNum;
        while (true) {

            cout << "\t\t\t\tWould you like to change an answer? (Y = Yes || N = No): ";
            cin >> reviewChoice;
            if (reviewChoice == 'N' || reviewChoice == 'n') {
                break;
            } else if(reviewChoice == 'Y' || reviewChoice == 'y'){
            cout << "\t\t\t\tEnter the question number to edit (1-" << NUM_QUESTIONS << "): ";
            cin >> qNum;
            
            if (qNum >= 1 && qNum <= NUM_QUESTIONS) {
                cout << "\n" << questions[qNum - 1] << "\nNew Answer: ";
                cin >> userAnswers[qNum - 1];
            } else {
                cout << "\t\t\t\tInvalid question number! Try again.\n";
            }
        }
        else{
        	cout << "\t\t\t\tInvalid choices!! Y = Yes || N = No" << endl;
		}
        }

        // Calculate Score
        for (int i = 0; i < NUM_QUESTIONS; i++) {
            if (toupper(userAnswers[i]) == correctAnswers[i]) {
                sts_score++;
            }
        }

        system("cls");
        cout << "You completed the Science, Technology and Society exam\n";
        cout << "Final Score: " << sts_score << "/" << NUM_QUESTIONS << endl;
        cout << "Please wait...";
        sleep(3);
        sts_taken = true;
        system("cls");
        exitprog = false;
        userpage();
        
    } else if (choose == '2') {
        cout << "Returning to Menu..." << endl;
        system("cls");
        sleep(1.5);
        exitprog = false;
        return;
    } else {
        cout << "INVALID, PLEASE CHOOSE 1 or 2" << endl;
    }
	
}

void ethics(){
	HANDLE h = GetStdHandle(STD_OUTPUT_HANDLE);
	char choose;
    system("cls");

    cout << "This is Applied Ethics subject" << endl;
    cout << "1. Take an exam" << endl;
    cout << "2. Back" << endl;
    cout << "Choose: ";
    cin >> choose;

    if (choose == '1') {
        cout << "Exam's Starting, Goodluck..." << endl;
        sleep(1.5);
        system("cls");

        // Questions & Answers
        SetConsoleTextAttribute(h,12);
        cout << "\n                             ==================================================================================================================================================\n";
        cout << "\n\t\t\t\tDIRECTIONS: PLEASE READ EACH QUESTION CAREFULLY AND THINK BEFORE YOU ANSWER. MAKE SURE TO FOLLOW ALL INSTRUCTIONS GIVEN. ALL ANSWERS MUST BE \n\t\t\t\t    WRITTEN IN CAPITAL LETTERS ONLY. FAILURE TO DO SO MAY RESULT IN YOUR ANSWER BEING MARKED INCORRECT. TAKE YOUR TIME AND DO YOUR BEST!\n" << endl;
        cout << "                             ==================================================================================================================================================\n\n";
        SetConsoleTextAttribute(h,15);
        const int NUM_QUESTIONS = 25;
        string questions[NUM_QUESTIONS] = {
		"\t\t\t\t\t\t1. What does the deontological approach to moral reasoning prioritize?\n\n\t\t\t\t\t\t\tA. Maximizing overall happiness\n\t\t\t\t\t\t\tB. The virtues of the decision-maker\n\t\t\t\t\t\t\tC. The consequences of actions\n\t\t\t\t\t\t\tD. Following universal moral principles and duties",
    	"\t\t\t\t\t\t2. What is the first step in the Seven-Step Moral Reasoning Model?\n\n\t\t\t\t\t\t\tA. Implement the Decision\n\t\t\t\t\t\t\tB. Identify the Problem\n\t\t\t\t\t\t\tC. Gather Relevant Information\n\t\t\t\t\t\t\tD. Make a Decision",
    	"\t\t\t\t\t\t3. Which ethical approach focuses on the greatest good for the greatest number of people?\n\n\t\t\t\t\t\t\tA. Deontological ethics\n\t\t\t\t\t\t\tB. Virtue ethics\n\t\t\t\t\t\t\tC. Utilitarianism\n\t\t\t\t\t\t\tD. Relativism",
    	"\t\t\t\t\t\t4. After making a decision in the moral reasoning process, what should be done next?\n\n\t\t\t\t\t\t\tA. Ignore the decision and move on\n\t\t\t\t\t\t\tB Reassess the decision without taking action\n\t\t\t\t\t\t\tC.Consult with others again to reconsider the decision\n\t\t\t\t\t\t\tD. Implement the decision and follow through",
   		"\t\t\t\t\t\t5. In the second step of the Seven-Step Moral Reasoning Model, what should an individual focus on?\n\n\t\t\t\t\t\t\tA. Implementing the decision\n\t\t\t\t\t\t\tB. Gathering facts and relevant information\n\t\t\t\t\t\t\tC. Identifying the problem\n\t\t\t\t\t\t\tD. Evaluating alternatives",
   		"\t\t\t\t\t\t6. Which of the following is NOT an ethical dilemma type? \n\n\t\t\t\t\t\t\tA. Religious ethics\n\t\t\t\t\t\t\tB. Personal ethics\n\t\t\t\t\t\t\tC. Professional ethics\n\t\t\t\t\t\t\tD. Social ethics",
    	"\t\t\t\t\t\t7. In the third step, what is the goal of identifying the ethical issues involved?\n\n\t\t\t\t\t\t\tA. To recognize the values at stake in the dilemma\n\t\t\t\t\t\t\tB. To avoid making a decision\n\t\t\t\t\t\t\tC. To justify the actions of all parties involved\n\t\t\t\t\t\t\tD. To find the quickest solution",
    	"\t\t\t\t\t\t8. When evaluating alternatives, what is essential?\n\n\t\t\t\t\t\t\tA. The focus should solely be on financial outcomes\n\t\t\t\t\t\t\tB. The moral consequences of each option should be weighed\n\t\t\t\t\t\t\tC. The longest option should always be chosen\n\t\t\t\t\t\t\tD. The decision should be made without further thought",
    	"\t\t\t\t\t\t9. What should be considered when exploring alternatives in the moral reasoning process?\n\n\t\t\t\t\t\t\tA. The speed at which the decision can be made\n\t\t\t\t\t\t\tB. What others in your group would prefer\n\t\t\t\t\t\t\tC. The most financially profitable option\n\t\t\t\t\t\t\tD. The potential ethical and practical consequences of each option",
    	"\t\t\t\t\t\t10. Which of the following is the main goal of the Seven-Step Moral Reasoning Model?\n\n\t\t\t\t\t\t\tA. To ensure compliance with the law\n\t\t\t\t\t\t\tB. To guide individuals in making ethical decisions\n\t\t\t\t\t\t\tC. To determine the most profitable decision\n\t\t\t\t\t\t\tD. To avoid making decisions",
    	"\t\t\t\t\t\t11. Which of the following is an example of a personal ethics dilemma?\n\n\t\t\t\t\t\t\tA. Deciding on the best way to allocate resources in a healthcare setting \n\t\t\t\t\t\t\tB. Deciding which team member to promote based on their work performance \n\t\t\t\t\t\t\tC. Deciding whether to take an action that could harm others for personal gain \n\t\t\t\t\t\t\tD. Deciding whether to report a colleague for unethical behavior",
    	"\t\t\t\t\t\t12. Why is moral reasoning important in professional decision-making?\n\n\t\t\t\t\t\t\tA. It promotes ethical standards and upholds the integrity of the profession \n\t\t\t\t\t\t\tB. It helps avoid legal consequences \n\t\t\t\t\t\t\tC. It focuses solely on profit maximization \n\t\t\t\t\t\t\tD. It ensures that personal blases do not affect decisions",
    	"\t\t\t\t\t\t13. How can the Seven-Step Moral Reasoning Model be used in professional decision-making?\n\n\t\t\t\t\t\t\tA. To evaluate alternatives systematically and make ethically sound decisions \n\t\t\t\t\t\t\tB. To prioritize financial profit over ethical values \n\t\t\t\t\t\t\tC. To avoid considering the consequences of a decision \n\t\t\t\t\t\t\tD. To make decisions quickly without consulting others",
    	"\t\t\t\t\t\t14. Which ethical dilemma is most likely to involve conflicting professional responsibilities?\n\n\t\t\t\t\t\t\tA. Deciding what to do with a lost wallet found in a public place \n\t\t\t\t\t\t\tB. Deciding whether to report a friend's wrongdoing \n\t\t\t\t\t\t\tC. A doctor choosing between saving two patients when resources are limited \n\t\t\t\t\t\t\tD. Deciding whether to cheat on a personal exam",
    	"\t\t\t\t\t\t15. The professional ethical dilemma of whistleblowing is best understood as: \n\n\t\t\t\t\t\t\tA. A decision to conform to societal norms \n\t\t\t\t\t\t\tB. A decision that involves risking career and relationships to address unethical practices \n\t\t\t\t\t\t\tC. An action to protect one's personal financial interests \n\t\t\t\t\t\t\tD.A decision that involves legal action only",
    	"\t\t\t\t\t\t16. When making a decision using the Seven-Step Moral Reasoning Model, what should the decision be based on? \n\n\t\t\t\t\t\t\tA. A reasoned and thoughtful consideration of ethical principies \n\t\t\t\t\t\t\tB. The most profitable option \n\t\t\t\t\t\t\tC. A quick response to avoid conflict \n\t\t\t\t\t\t\tD. The preference of the decision-maker's peers",
    	"\t\t\t\t\t\t17. A business executive discovers that a supplier is violating human rights. The ethical dilemma is about:\n\n\t\t\t\t\t\t\tA. The company's legal obligation \n\t\t\t\t\t\t\tB. The employee's personal integrity \n\t\t\t\t\t\t\tC.The company's financial interests \n\t\t\t\t\t\t\tD. The balance between profits and ethical standards",
    	"\t\t\t\t\t\t18. In a moral dilemma, what would 'gathering relevant information' primarily involve? \n\n\t\t\t\t\t\t\tA. Looking at the financial costs and benefits of each choice \n\t\t\t\t\t\t\tB. Understanding all facts, perspectives, and data about the situation \n\t\t\t\t\t\t\tC. Discussing the dilemma with as many people as possible \n\t\t\t\t\t\t\tD. Ignoring outside influences to make a personal decision",
    	"\t\t\t\t\t\t19. In which step of the moral reasoning model would you list all the possible actions you can take? \n\n\t\t\t\t\t\t\tA. Evaluate the alternatives \n\t\t\t\t\t\t\tB.Gather relevant information \n\t\t\t\t\t\t\tC.Identify the problem \n\t\t\t\t\t\t\tD. Explore the alternatives",
	    "\t\t\t\t\t\t20. Which of the following is a potential disadvantage of the deontological approach? \n\n\t\t\t\t\t\t\tA. It is too focused on the consequences of actions \n\t\t\t\t\t\t\tB. It may conflict with achieving the best outcomes in a situation \n\t\t\t\t\t\t\tC. It doesn't provide clear rules for decision-making \n\t\t\t\t\t\t\tD. It requires focusing on the individual's character",
	    "\t\t\t\t\t\t21. During a team project, you realize a solution you're working on isn't solving the problem as expected. What would you do next? \n\n\t\t\t\t\t\t\tA. Reassess the problem and develop a new solution based on feedback. \n\t\t\t\t\t\t\tB. Blame someone else for the failure. \n\t\t\t\t\t\t\tC. Give up and accept that the project will fail. \n\t\t\t\t\t\t\tD. Take a break and hope the problem resolves itself.",
   		"\t\t\t\t\t\t22. You're given a task that you have never done before, and it seems difficult. How do you handle it? \n\n\t\t\t\t\t\t\tA. Give up immediately because you're unfamiliar with it. \n\t\t\t\t\t\t\tB. Complain about the difficulty of the task to others. \n\t\t\t\t\t\t\tC. Take small steps, seek guidance, and learn as you go along. \n\t\t\t\t\t\t\tD.Avoid doing it at all and hope someone else takes it over.",
		"\t\t\t\t\t\t23. While working on a problem, you come up with a new idea that could be an innovative solution. How do you proceed? \n\n\t\t\t\t\t\t\tA. Ignore the idea because you don't have enough time to explore it. \n\t\t\t\t\t\t\tB. Keep the idea to yourself because it might be too unconventional. \n\t\t\t\t\t\t\tC. Share the idea with the team and discuss its potential benefits. \n\t\t\t\t\t\t\tD. Dismiss the idea immediately because it's too different from the traditional approach.",
    	"\t\t\t\t\t\t24. You've received feedback about your recent presentation, and it wasn't as positive as expected. How do you respond? \n\n\t\t\t\t\t\t\tA. Reflect on the feedback and identify areas for improvement in future presentations. \n\t\t\t\t\t\t\tB. Take it personally and become defensive. \n\t\t\t\t\t\t\tC. Ignore the feedback and continue doing things your way. \n\t\t\t\t\t\t\tD. Blame the audience for not understanding your points.",
    	"\t\t\t\t\t\t25. A colleague presents a new idea during a meeting that contradicts your own beliefs. What is your response? \n\n\t\t\t\t\t\t\tA. Argue passionately to prove your idea is better. \n\t\t\t\t\t\t\tB. Avoid engaging in the conversation and stay quiet. \n\t\t\t\t\t\t\tC. Listen actively and evaluate the idea logically, keeping an open mind. \n\t\t\t\t\t\t\tD. Dismiss their idea immediately without further consideration",
				};
        char correctAnswers[NUM_QUESTIONS] = {'D','B','C','D','B','A','A','B','D','B','C', 'A', 'A', 'C', 'B', 'A', 'D', 'B', 'D', 'B', 'A', 'C', 'C', 'A', 'C'};
        char userAnswers[NUM_QUESTIONS];

        // Ask Questions and Store Answers
        for (int i = 0; i < NUM_QUESTIONS; i++) {
            cout << questions[i] << "\n\n\t\t\t\t\t\tAnswer: ";
            cin >> userAnswers[i];
            cout << "\n";
        }
        
        // Review and Edit Answers
        
        
        char reviewChoice;
        int qNum;
        while (true) {

            cout << "\t\t\t\tWould you like to change an answer? (Y = Yes || N = No): ";
            cin >> reviewChoice;
            if (reviewChoice == 'N' || reviewChoice == 'n') {
                break;
            } else if(reviewChoice == 'Y' || reviewChoice == 'y'){
            cout << "\t\t\t\tEnter the question number to edit (1-" << NUM_QUESTIONS << "): ";
            cin >> qNum;
            
            if (qNum >= 1 && qNum <= NUM_QUESTIONS) {
                cout << "\n" << questions[qNum - 1] << "\n\n\t\t\t\t\t\tNew Answer: ";
                cin >> userAnswers[qNum - 1];
            } else {
                cout << "\t\t\t\tInvalid question number! Try again.\n";
            }
        }
        else{
        	cout << "\t\t\t\tInvalid choices!! Y = Yes || N = No" << endl;
		}
        }

        // Calculate Score
        for (int i = 0; i < NUM_QUESTIONS; i++) {
            if (toupper(userAnswers[i]) == correctAnswers[i]) {
                ethics_score++;
            }
        }

        system("cls");
        cout << "You completed the Applied Ethics exam\n";
        cout << "Final Score: " << ethics_score << "/" << NUM_QUESTIONS << endl;
        cout << "Please wait...";
        sleep(3);
        ethics_taken = true;
        system("cls");
        exitprog = false;
        userpage();
        
    } else if (choose == '2') {
        cout << "Returning to Menu..." << endl;
        system("cls");
        sleep(1.5);
        exitprog = false;
        return;
    } else {
        cout << "INVALID, PLEASE CHOOSE 1 or 2" << endl;
    }
}



void discrete(){
	HANDLE h = GetStdHandle(STD_OUTPUT_HANDLE);
	cout << "this is math!";
}




void pathfit(){
	HANDLE h = GetStdHandle(STD_OUTPUT_HANDLE);
	char choose;
    system("cls");

    cout << "This is PATHFIT subject" << endl;
    cout << "1. Take an exam" << endl;
    cout << "2. Back" << endl;
    cout << "Choose: ";
    cin >> choose;

    if (choose == '1') {
        cout << "Exam's Starting, Goodluck..." << endl;
        sleep(1.5);
        system("cls");

        // Questions & Answers
        SetConsoleTextAttribute(h,1);
        cout << "\n                             ==================================================================================================================================================\n";
        cout << "\n\t\t\t\tDIRECTIONS: PLEASE READ EACH QUESTION CAREFULLY AND THINK BEFORE YOU ANSWER. MAKE SURE TO FOLLOW ALL INSTRUCTIONS GIVEN. ALL ANSWERS MUST BE \n\t\t\t\t    WRITTEN IN CAPITAL LETTERS ONLY. FAILURE TO DO SO MAY RESULT IN YOUR ANSWER BEING MARKED INCORRECT. TAKE YOUR TIME AND DO YOUR BEST!\n" << endl;
        cout << "                             ==================================================================================================================================================\n\n";
        SetConsoleTextAttribute(h,15);
        const int NUM_QUESTIONS = 25;
        string questions[NUM_QUESTIONS] = {
		"\t\t\t\t\t\t1. What should you do if someone is unconscious and not breathing?\n\n\t\t\t\t\t\t\tA. Perform CPR and call emergency services\n\t\t\t\t\t\t\tB. Give them food and water\n\t\t\t\t\t\t\tC. Try to wake them up by shaking them\n\t\t\t\t\t\t\tD. Leave them and wait for help",
	    "\t\t\t\t\t\t2. What muscle group does the plank exercise primarily target?\n\n\t\t\t\t\t\t\tA. Shoulders\n\t\t\t\t\t\t\tB. Arms\n\t\t\t\t\t\t\tC. Core\n\t\t\t\t\t\t\tD. Legs",
	    "\t\t\t\t\t\t3. Which activity helps improve dynamic balance?\n\n\t\t\t\t\t\t\tA. Lifting heavy weights\n\t\t\t\t\t\t\tB. Watching TV\n\t\t\t\t\t\t\tC. Step-over drills\n\t\t\t\t\t\t\tD. Sitting still",
		"\t\t\t\t\t\t4. What is the main purpose of functional fitness in fall prevention?\n\n\t\t\t\t\t\t\tA. To increase body fat\n\t\t\t\t\t\t\tB. To reduce flexibility\n\t\t\t\t\t\t\tC. To improve balance and coordination\n\t\t\t\t\t\t\tD. To decrease muscle strength",
	    "\t\t\t\t\t\t5. What should you do first if someone falls and appears injured?\n\n\t\t\t\t\t\t\tA. Leave them alone\n\t\t\t\t\t\t\tB. Move them immediately\n\t\t\t\t\t\t\tC. Check their responsiveness\n\t\t\t\t\t\t\tD. Shake them hard",
	    "\t\t\t\t\t\t6. Which of these is a flexibility exercise that helps prevent falls?\n\n\t\t\t\t\t\t\tA. Bench press\n\t\t\t\t\t\t\tB. Deadlifts\n\t\t\t\t\t\t\tC. Hip openers\n\t\t\t\t\t\t\tD. Push-ups",
		"\t\t\t\t\t\t7. What is a safe cardiovascular exercise mentioned in the program?\n\n\t\t\t\t\t\t\tA. Sprinting uphill\n\t\t\t\t\t\t\tB. Bench pressing\n\t\t\t\t\t\t\tC. Powerlifting\n\t\t\t\t\t\t\tD. Swimming",
        "\t\t\t\t\t\t8. Which of the following exercises strengthens the lower body for better stability?\n\n\t\t\t\t\t\t\tA. Jumping jacks\n\t\t\t\t\t\t\tB. Shoulder presses\n\t\t\t\t\t\t\tC. Squats\n\t\t\t\t\t\t\tD. Bicep curls",
        "\t\t\t\t\t\t9. What is a good way to progress balance exercises?\n\n\t\t\t\t\t\t\tA. Only practice when needed\n\t\t\t\t\t\t\tB. Avoid doing them regularly\n\t\t\t\t\t\t\tC. Perform them with closed eyes\n\t\t\t\t\t\t\tD. Stop practicing once you can do them",
        "\t\t\t\t\t\t10. Which of the following is not a part of the RICE method for treating a mild sprain?\n\n\t\t\t\t\t\t\tA. Compression\n\t\t\t\t\t\t\tB. Ice\n\t\t\t\t\t\t\tC. Rest\n\t\t\t\t\t\t\tD. Exercise",
        "\t\t\t\t\t\t11. An elderly person is working on improving flexibility to prevent falls. Which stretch is most useful?\n\n\t\t\t\t\t\t\tA. Shoulder press\n\t\t\t\t\t\t\tB. Deadlift\n\t\t\t\t\t\t\tC. Hamstring stretch\n\t\t\t\t\t\t\tD. Bicep curl",
        "\t\t\t\t\t\t12. During a game, Alex trips and falls but manages to regain balance before hitting the ground. What skill helped him?\n\n\t\t\t\t\t\t\tA. Reaction time\n\t\t\t\t\t\t\tB. Endurance\n\t\t\t\t\t\t\tC.Strength\n\t\t\t\t\t\t\tD. Flexibility",
        "\t\t\t\t\t\t13. Lisa, a 70-year-old, has difficulty standing up from a chair without using her hands. Which exercise should she practice?\n\n\t\t\t\t\t\t\tA. Jumping lunges\n\t\t\t\t\t\t\tB. Shoulder presses\n\t\t\t\t\t\t\tC. Seated hamstring stretch\n\t\t\t\t\t\t\tD. Chair squats",
        "\t\t\t\t\t\t14. Emily is helping a friend who has fallen and may have a concussion. What should she do?\n\n\t\t\t\t\t\t\tA. Leave them alone to recover\n\t\t\t\t\t\t\tB. Ask them to continue walking to shake it off\n\t\t\t\t\t\t\tC. Give them painkillers and let them rest\n\t\t\t\t\t\t\tD. Keep the friend still and monitor for symptoms",
        "\t\t\t\t\t\t15. Mr. Lopez, a senior citizen, is worried about falling in his home. What should he focus on during his workouts?\n\n\t\t\t\t\t\t\tA. Heavyweight lifting\n\t\t\t\t\t\t\tB. Long-distance running\n\t\t\t\t\t\t\tC. Arm strength exercises\n\t\t\t\t\t\t\tD. Balance and core exercises",
        "\t\t\t\t\t\t16. James struggles with weak legs, making it hard for him to climb stairs. Which exercise can help?\n\n\t\t\t\t\t\t\tA. Shoulder shrugs\n\t\t\t\t\t\t\tB. Step-ups\n\t\t\t\t\t\t\tC. Jumping jacks\n\t\t\t\t\t\t\tD. Arm circles",
        "\t\t\t\t\t\t17. After spraining her ankle, Sarah wants to safely resume physical activity. What should she do first?\n\n\t\t\t\t\t\t\tA. Ignore the pain and continue workouts\n\t\t\t\t\t\t\tB. Run on it to see if the pain goes away\n\t\t\t\t\t\t\tC. Perform stretching exercises to relieve pain\n\t\t\t\t\t\t\tD. Rest and allow the injury to heal before resuming activity",
        "\t\t\t\t\t\t18. Paul wants to improve his reaction time to avoid tripping when walking on uneven surfaces. Which drill is best?\n\n\t\t\t\t\t\t\tA. Ball toss while balancing on one foot\n\t\t\t\t\t\t\tB. Bicep curls\n\t\t\t\t\t\t\tC. Jogging on a treadmill\n\t\t\t\t\t\t\tD. Seated hamstring stretch",
        "\t\t\t\t\t\t19. A PE teacher wants to incorporate a balance drill into warm-ups. Which is the best choice?\n\n\t\t\t\t\t\t\tA. Sprinting\n\t\t\t\t\t\t\tB. Push-ups\n\t\t\t\t\t\t\tC. Single-leg stands\n\t\t\t\t\t\t\tD. Heavyweight lifting",
        "\t\t\t\t\t\t20. An athlete wants to strengthen his ankles to avoid rolling them during sports. Which exercise is most beneficial?\n\n\t\t\t\t\t\t\tA. Shoulder shrugs\n\t\t\t\t\t\t\tB. Calf raises\n\t\t\t\t\t\t\tC. Bicep curls\n\t\t\t\t\t\t\tD. Bench press",
        "\t\t\t\t\t\t21. What should you do when assisting someone with a suspected fracture?\n\n\t\t\t\t\t\t\tA. Massage the area to reduce swelling\n\t\t\t\t\t\t\tB. Apply a cold compress and ask them to walk it off\n\t\t\t\t\t\t\tC. Try to move or realign the injured limb\n\t\t\t\t\t\t\tD. Immobilize the area and seek medical assistance",
        "\t\t\t\t\t\t22. How can balance exercises be modified for increased difficulty?\n\n\t\t\t\t\t\t\tA. Skipping balance exercises altogether\n\t\t\t\t\t\t\tB. Holding onto a support for all exercises\n\t\t\t\t\t\t\tC. Performing them on an unstable surface like a BOSU ball\n\t\t\t\t\t\t\tD. Reducing the range of motion",
        "\t\t\t\t\t\t23. What is the recommended response for a person with a possible concussion?\n\n\t\t\t\t\t\t\tA. Have them lie flat and shake them to wake them up\n\t\t\t\t\t\t\tB. Allow them to rest, monitor symptoms, and seek medical attention if needed\n\t\t\t\t\t\t\tC. Ignore the symptoms unless they lose consciousness\n\t\t\t\t\t\t\tD. Give them painkillers and let them continue their activity",
        "\t\t\t\t\t\t24. Why are dynamic balance exercises important in fall prevention?\n\n\t\t\t\t\t\t\tA. They only help in sports performance\n\t\t\t\t\t\t\tB. They train the body to react quickly to movement changes\n\t\t\t\t\t\t\tC. They are not as effective as static balance exercises\n\t\t\t\t\t\t\tD. They focus only on the upper body",
        "\t\t\t\t\t\t25. Which of the following exercises is a static balance drill?\n\n\t\t\t\t\t\t\tA. Step-over drills\n\t\t\t\t\t\t\tB. Side-to-side weight shifts\n\t\t\t\t\t\t\tC. Agility ladder drills\n\t\t\t\t\t\t\tD. Single-leg stands"
				};
        char correctAnswers[NUM_QUESTIONS] = {'A', 'C', 'C', 'C', 'C', 'C', 'D', 'C', 'C', 'D', 'C', 'A', 'D', 'D', 'D', 'B', 'D', 'A', 'C', 'B', 'D', 'C', 'B', 'B', 'D'};
        char userAnswers[NUM_QUESTIONS];

        // Ask Questions and Store Answers
        for (int i = 0; i < NUM_QUESTIONS; i++) {
            cout << questions[i] << "\n\n\t\t\t\t\t\tAnswer: ";
            cin >> userAnswers[i];
            cout << "\n";
        }
        
        // Review and Edit Answers
        
        
        char reviewChoice;
        int qNum;
        while (true) {

            cout << "\t\t\t\tWould you like to change an answer? (Y = Yes || N = No): ";
            cin >> reviewChoice;
            if (reviewChoice == 'N' || reviewChoice == 'n') {
                break;
            } else if(reviewChoice == 'Y' || reviewChoice == 'y'){
            cout << "\t\t\t\tEnter the question number to edit (1-" << NUM_QUESTIONS << "): ";
            cin >> qNum;
            
            if (qNum >= 1 && qNum <= NUM_QUESTIONS) {
                cout << "\n" << questions[qNum - 1] << "\n\n\t\t\t\t\t\tNew Answer: ";
                cin >> userAnswers[qNum - 1];
            } else {
                cout << "\t\t\t\tInvalid question number! Try again.\n";
            }
        }
        else{
        	cout << "\t\t\t\tInvalid choices!! Y = Yes || N = No" << endl;
		}
        }

        // Calculate Score
        for (int i = 0; i < NUM_QUESTIONS; i++) {
            if (toupper(userAnswers[i]) == correctAnswers[i]) {
                pathfit_score++;
            }
        }

        system("cls");
        cout << "You completed the PATHFIT exam\n";
        cout << "Final Score: " << pathfit_score << "/" << NUM_QUESTIONS << endl;
        cout << "Please wait...";
        sleep(3);
        pathfit_taken = true;
        system("cls");
        exitprog = false;
        userpage();
        
    } else if (choose == '2') {
        cout << "Returning to Menu..." << endl;
        system("cls");
        sleep(1.5);
        exitprog = false;
        return;
    } else {
        cout << "INVALID, PLEASE CHOOSE 1 or 2" << endl;
    }
}


void comprog() {
	HANDLE h = GetStdHandle(STD_OUTPUT_HANDLE);
    char choose;
    system("cls");

    cout << "This is Computer Programming subject" << endl;
    cout << "1. Take an exam" << endl;
    cout << "2. Back" << endl;
    cout << "Choose: ";
    cin >> choose;

    if (choose == '1') {
        cout << "Exam's Starting, Goodluck..." << endl;
        sleep(1.5);
        system("cls");

        // Questions & Answers
        SetConsoleTextAttribute(h,8);
        cout << "\n                             ==================================================================================================================================================\n";
        cout << "\n\t\t\t\tDIRECTIONS: PLEASE READ EACH QUESTION CAREFULLY AND THINK BEFORE YOU ANSWER. MAKE SURE TO FOLLOW ALL INSTRUCTIONS GIVEN. ALL ANSWERS MUST BE \n\t\t\t\t    WRITTEN IN CAPITAL LETTERS ONLY. FAILURE TO DO SO MAY RESULT IN YOUR ANSWER BEING MARKED INCORRECT. TAKE YOUR TIME AND DO YOUR BEST!\n" << endl;
        cout << "                             ==================================================================================================================================================\n\n";
        SetConsoleTextAttribute(h,15);
        const int NUM_QUESTIONS = 5;
        string questions[NUM_QUESTIONS] = {
            "What must every C++ statement end with?\n A.) Comma\n B.) Colon\n C.) Semicolon",
            "Which is the correct syntax for a for loop in C?\n A.) for(i=0; i<10;i++)\n B.) for i=0 to 10\n C.) for(i=0;i<10)i++;",
            "How do you declare an integer variable named 'age' in C++?\n A.) int age = 25;\n B.) integer age = 25;\n C.) age = 25;",
            "What does %d represent in printf?\n A.) Floating-point number\n B.) A character\n C.) An Integer",
            "What is the purpose of #include <stdio.h>?\n A.) Declare variable\n B.) Include standard I/O library\n C.) Define function"
        };
        char correctAnswers[NUM_QUESTIONS] = {'C', 'A', 'A', 'C', 'B'};
        char userAnswers[NUM_QUESTIONS];

        // Ask Questions and Store Answers
        for (int i = 0; i < NUM_QUESTIONS; i++) {
            cout << i + 1 << ". " << questions[i] << "\n\n\t\t\t\t\t\tAnswer: ";
            cin >> userAnswers[i];
        }
        
        // Review and Edit Answers
        
        
        char reviewChoice;
        int qNum;
        while (true) {
            cout << "\nReview your answers:\n";
            for (int i = 0; i < NUM_QUESTIONS; i++) {
                cout << i + 1 << ". " << questions[i] << "\nYour Answer: " << userAnswers[i] << "\n\n";
            }
            cout << "\t\t\t\tWould you like to change an answer? (Y/N): ";
            cin >> reviewChoice;
            if (reviewChoice == 'N' || reviewChoice == 'n') {
                break;
            } else if(reviewChoice == 'Y' || reviewChoice == 'y'){
            cout << "\t\t\t\tEnter the question number to edit (1-" << NUM_QUESTIONS << "): ";
            cin >> qNum;
            
            if (qNum >= 1 && qNum <= NUM_QUESTIONS) {
                cout << "\n" << questions[qNum - 1] << "\nNew Answer: ";
                cin >> userAnswers[qNum - 1];
            } else {
                cout << "Invalid question number! Try again.\n";
            }
        }
        }

        // Calculate Score
        comprog_score = 0;
        for (int i = 0; i < NUM_QUESTIONS; i++) {
            if (toupper(userAnswers[i]) == correctAnswers[i]) {
                comprog_score++;
            }
        }

        system("cls");
        cout << "You completed the Computer Programming exam!\n";
        cout << "Final Score: " << comprog_score << "/" << NUM_QUESTIONS << endl;
        cout << "Please wait...";
        sleep(3);
        comprog_taken = true;
        system("cls");
        exitprog = false;
        return;
        
    } else if (choose == '2') {
        cout << "Returning to Menu..." << endl;
        system("cls");
        sleep(1.5);
        exitprog = false;
        return;
    } else {
        cout << "INVALID, PLEASE CHOOSE 1 or 2" << endl;
    }
}


void purcomm() {
	HANDLE h = GetStdHandle(STD_OUTPUT_HANDLE);
    char choose;
    system("cls");

    cout << "This is Purposive Communication subject" << endl;
    cout << "1. Take an exam" << endl;
    cout << "2. Back" << endl;
    cout << "Choose: ";
    cin >> choose;

    if (choose == '1') {
        cout << "Exam's Starting, Goodluck..." << endl;
        sleep(1.5);
        system("cls");

        // Questions & Answers
        SetConsoleTextAttribute(h,13);
        cout << "\n                             ==================================================================================================================================================\n";
        cout << "\n\t\t\t\tDIRECTIONS: PLEASE READ EACH QUESTION CAREFULLY AND THINK BEFORE YOU ANSWER. MAKE SURE TO FOLLOW ALL INSTRUCTIONS GIVEN. ALL ANSWERS MUST BE \n\t\t\t\t    WRITTEN IN CAPITAL LETTERS ONLY. FAILURE TO DO SO MAY RESULT IN YOUR ANSWER BEING MARKED INCORRECT. TAKE YOUR TIME AND DO YOUR BEST!\n" << endl;
        cout << "                             ==================================================================================================================================================\n\n";
        SetConsoleTextAttribute(h,15);
        const int NUM_QUESTIONS = 25;
        string questions[NUM_QUESTIONS] = {
		"\t\t\t\t\t\t1. What is the most important element of an effective persuasive speech?\n\n\t\t\t\t\t\t\tA. A controversial topic\n\t\t\t\t\t\t\tB. A strong emotional appeal\n\t\t\t\t\t\t\tC. A charismatic speaker\n\t\t\t\t\t\t\tD. A well-organized structure",
		"\t\t\t\t\t\t2. Which of the following is NOT a technique commonly used in entertainment speeches?\n\n\t\t\t\t\t\t\tA. Sharing personal experiences\n\t\t\t\t\t\t\tB. Using metaphors and vivid imagery\n\t\t\t\t\t\t\tC. Telling jokes\n\t\t\t\t\t\t\tD. Presenting factual data and statistics",
		"\t\t\t\t\t\t3. What is the difference between an informative speech and a persuasive speech?\n\n\t\t\t\t\t\t\tA. An Informative speech aims to persuade, while a persuasive speech aims to inspire.\n\t\t\t\t\t\t\tB. An informative speech aims to inform, while a persuasive speech aims to convince.\n\t\t\t\t\t\t\tC. An informative speech aims to entertain, while a persuasive speech aims to inform.\n\t\t\t\t\t\t\tD. There is no difference between an informative speech and a persuasive speech.",
		"\t\t\t\t\t\t4. What is the primary goal of an informative speech?\n\n\t\t\t\t\t\t\tA. To provide the audience with knowledge and understanding of a topic\n\t\t\t\t\t\t\tB. To entertain the audience\n\t\t\t\t\t\t\tC. To inspire the audience to take action\n\t\t\t\t\t\t\tD. To persuade the audience to agree with a specific viewpoint",
		"\t\t\t\t\t\t5. Which of the following is NOT a category of informative speech topics?\n\n\t\t\t\t\t\t\tA. Opinions\n\t\t\t\t\t\t\tB. Events\n\t\t\t\t\t\t\tC. Processes\n\t\t\t\t\t\t\tD. Objects",
		"\t\t\t\t\t\t6. What is the primary goal of a persuasive speech?\n\n\t\t\t\t\t\t\tA. To entertain the audience\n\t\t\t\t\t\t\tB. To inspire the audierice to take action\n\t\t\t\t\t\t\tC. To inform the audience about a specific topic\n\t\t\t\t\t\t\tD. To convince the audience to accept a particular viewpoint",
		"\t\t\t\t\t\t7. Which of the following is a good tip for writing an effective persuasive speech?\n\n\t\t\t\t\t\t\tA. Focus on presenting your own viewpoint without considering opposing arguments\n\t\t\t\t\t\t\tB. Rely on personal anecdotes and stories to make your argument more compelling\n\t\t\t\t\t\t\tC. Use emotional language to evoke strong feelings in the audience\n\t\t\t\t\t\t\tD. Use facts and evidence to support your claim",
		"\t\t\t\t\t\t8. What is the main purpose of an entertainment speech?\n\n\t\t\t\t\t\t\tA. To inform the audience about a specific topic\n\t\t\t\t\t\t\tB. To make the audience laugh and enjoy themselves.\n\t\t\t\t\t\t\tC. To persuade the audience to take action\n\t\t\t\t\t\t\tD. To inspire the audience to change their beliefs",
		"\t\t\t\t\t\t9. Which of the following is a common organizational pattern for an informative speech?\n\n\t\t\t\t\t\t\tA. All of the choices\n\t\t\t\t\t\t\tB. Problem-Solution\n\t\t\t\t\t\t\tC. Topical Order\n\t\t\t\t\t\t\tD. Chronological Order",
		"\t\t\t\t\t\t10. A speech that aims to inspire the audience to pursue their dreams.\n\n\t\t\t\t\t\t\tA. Persuasive Speech\n\t\t\t\t\t\t\tB. Informative Speech\n\t\t\t\t\t\t\tC. Entertainment Speech",
		"\t\t\t\t\t\t11. A speech that aims to describe the different types of clouds.\n\n\t\t\t\t\t\t\tA. Entertainment Speech\n\t\t\t\t\t\t\tB. Persuasive Speech\n\t\t\t\t\t\t\tC. Informative Speech",
		"\t\t\t\t\t\t12. A speech that aims to share a funny story about a embarrassing experience.\n\n\t\t\t\t\t\t\tA. Informative Speech\n\t\t\t\t\t\t\tB. Persuasive Speech\n\t\t\t\t\t\t\tC. Entertainment Speech",
		"\t\t\t\t\t\t13. A speech that aims to explain the process of making a traditional Japanese dish.\n\n\t\t\t\t\t\t\tA. Informative Speech\n\t\t\t\t\t\t\tB. Persuasive Speech\n\t\t\t\t\t\t\tC. Entertainment Speech",
		"\t\t\t\t\t\t14. A speech that aims to make the audience laugh with jokes about everyday life.\n\n\t\t\t\t\t\t\tA. Entertainment Speech\n\t\t\t\t\t\t\tB. Persuasive Speech\n\t\t\t\t\t\t\tC. Informative Speech",
		"\t\t\t\t\t\t15. A speech that aims to convince the audience to donate to a local charity.\n\n\t\t\t\t\t\t\tA. Persuasive Speech\n\t\t\t\t\t\t\tB. Informative Speech\n\t\t\t\t\t\t\tC. Entertainment Speech",
		"\t\t\t\t\t\t16. A speech that aims to share a funny story about a disastrous camping trip.\n\n\t\t\t\t\t\t\tA. Entertainment Speech\n\t\t\t\t\t\t\tB. Informative Speech\n\t\t\t\t\t\t\tC. Persuasive Speech",
		"\t\t\t\t\t\t17. A speech that aims to make the audience laugh with jokes about pop culture.\n\n\t\t\t\t\t\t\tA. Entertainment Speech\n\t\t\t\t\t\t\tB. Informative Speech\n\t\t\t\t\t\t\tC. Persuasive Speech",
		"\t\t\t\t\t\t18. A speech that aims to describe the different types of flowers.\n\n\t\t\t\t\t\t\tA. Entertainment Speech\n\t\t\t\t\t\t\tB. Informative Speech\n\t\t\t\t\t\t\tC. Persuasive Speech",
		"\t\t\t\t\t\t19. A speech that aims to share a personal story about overcoming a challenge.\n\n\t\t\t\t\t\t\tA. Persuasive Speech\n\t\t\t\t\t\t\tB. Informative Speech\n\t\t\t\t\t\t\tC. Entertainment Speech",
		"\t\t\t\t\t\t20. You are a guest speaker at a company picnic and have been asked to share a funny story about your time working \n\t\t\t\t\t\t    at the company.\n\n\t\t\t\t\t\t\tA. Informative Speech\n\t\t\t\t\t\t\tB. Persuasive Speech\n\t\t\t\t\t\t\tC. Entertainment Speech",
		"\t\t\t\t\t\t21. You are a volunteer at a local animal shelter and have been asked to give a presentation to a group of high school \n\t\t\t\t\t\t    students about the importance of pet adoption.\n\n\t\t\t\t\t\t\tA. Informative Speech\n\t\t\t\t\t\t\tB. Persuasive Speech\n\t\t\t\t\t\t\tC. Entertainment Speech",
		"\t\t\t\t\t\t22. You are a student leader giving a presentation to your class about the benefits of recycling and how to reduce \n\t\t\t\t\t\t    your carbon footprint.\n\n\t\t\t\t\t\t\tA. Entertainment Speech\n\t\t\t\t\t\t\tB. Persuasive Speech\n\t\t\t\t\t\t\tC. Informative Speech",
		"\t\t\t\t\t\t23. You are a history buff and have been invited to give a talk at a local museum about the history of your city.\n\n\t\t\t\t\t\t\tA. Informative Speech\n\t\t\t\t\t\t\tB. Entertainment Speech\n\t\t\t\t\t\t\tC. Persuasive Speech",
		"\t\t\t\t\t\t24. Which of the following is not a example of informative speech\n\n\t\t\t\t\t\t\tA. Seminar\n\t\t\t\t\t\t\tB. Lecture\n\t\t\t\t\t\t\tC. Court Hearing",
		"\t\t\t\t\t\t25. The following are example of informative speech except?\n\n\t\t\t\t\t\t\tA. Lecture\n\t\t\t\t\t\t\tB. Seminar\n\t\t\t\t\t\t\tC. Tv Show"
		};
        char correctAnswers[NUM_QUESTIONS] = {'D', 'D', 'B', 'A', 'A', 'D', 'A', 'B', 'A', 'A', 'C', 'C', 'A', 'A', 'A', 'A', 'A', 'B', 'C', 'C', 'A', 'C', 'A', 'C', 'C'};
        char userAnswers[NUM_QUESTIONS];

        // Ask Questions and Store Answers
        for (int i = 0; i < NUM_QUESTIONS; i++) {
            cout << questions[i] << "\n\n\t\t\t\t\t\tAnswer: ";
            cin >> userAnswers[i];
            cout << "\n";
        }
        
        // Review and Edit Answers
        
        
        char reviewChoice;
        int qNum;
        while (true) {

            cout << "\t\t\t\tWould you like to change an answer? (Y = Yes || N = No): ";
            cin >> reviewChoice;
            if (reviewChoice == 'N' || reviewChoice == 'n') {
                break;
            } else if(reviewChoice == 'Y' || reviewChoice == 'y'){
            cout << "\t\t\t\tEnter the question number to edit (1-" << NUM_QUESTIONS << "): ";
            cin >> qNum;
            
            if (qNum >= 1 && qNum <= NUM_QUESTIONS) {
                cout << "\n" << questions[qNum - 1] << "\n\n\t\t\t\t\t\tNew Answer: ";
                cin >> userAnswers[qNum - 1];
            } else {
                cout << "\t\t\t\tInvalid question number! Try again.\n";
            }
        }
        else{
        	cout << "\t\t\t\tInvalid choices!! Y = Yes || N = No" << endl;
		}
        }

        // Calculate Score
        for (int i = 0; i < NUM_QUESTIONS; i++) {
            if (toupper(userAnswers[i]) == correctAnswers[i]) {
                purcomm_score++;
            }
        }

        system("cls");
        cout << "You completed the Purposive Communication exam!\n";
        cout << "Final Score: " << purcomm_score << "/" << NUM_QUESTIONS << endl;
        cout << "Please wait...";
        sleep(3);
        purcomm_taken = true;
        system("cls");
        exitprog = false;
        userpage();
        
    } else if (choose == '2') {
        cout << "Returning to Menu..." << endl;
        system("cls");
        sleep(1.5);
        exitprog = false;
        return;
    } else {
        cout << "INVALID, PLEASE CHOOSE 1 or 2" << endl;
    }
	
}

void subscore() {
	HANDLE h = GetStdHandle(STD_OUTPUT_HANDLE);
    char select;
    system("cls");
    SetConsoleTextAttribute(h,1);
   	cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   	cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
 	cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
 	cout << "\t\t\t\t\t\t|\t\t|";
   	SetConsoleTextAttribute(h,3);
	cout << "===============================================================================";
	SetConsoleTextAttribute(h,1);
	cout << "|\t\t|\n";
   	cout << "\t\t\t\t\t\t|\t\t|";
   	SetConsoleTextAttribute(h,3);
	cout << "===============================================================================";
	SetConsoleTextAttribute(h,1);
	cout << "|\t\t|\n";
 	cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
 	cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
 	cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
 	SetConsoleTextAttribute(h,3);
    cout << "\t\t\t\t=================================================================================================================================================\n\n";
    SetConsoleTextAttribute(h,15);
    cout << "\t\t\t\t                                                          EVALUATION FOR THE HIGHER UPS\n" << endl;
    cout << "\t\t\t\t                                                              SCORE OF THE SUBJECTS\n" << endl;
    SetConsoleTextAttribute(h,3);
    cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n\n";
    SetConsoleTextAttribute(h,15);
    cout << "                                                                    Subject:                                                      ";
	SetConsoleTextAttribute(h,14);
	cout << "Scores\n\n";
	SetConsoleTextAttribute(h,15);
    cout << "                                                                         Purposive Communication                                   ";
	SetConsoleTextAttribute(h,14);
	cout << purcomm_score << "/25" << endl;
	SetConsoleTextAttribute(h,15);
    cout << "                                                                         Art Appreciation                                          ";
    SetConsoleTextAttribute(h,14);
	cout << artapp_score << "/25" << endl;
	SetConsoleTextAttribute(h,15);
    cout << "                                                                         Science and Technology (ST) and Society                   ";
	SetConsoleTextAttribute(h,14);
	cout << sts_score << "/25" << endl;
	SetConsoleTextAttribute(h,15);
    cout << "                                                                         Applied Ethics                                            ";
	SetConsoleTextAttribute(h,14);
	cout << ethics_score << "/25" << endl;
	SetConsoleTextAttribute(h,15);
    cout << "                                                                         Discrete Mathemathics                                     ";
	SetConsoleTextAttribute(h,14);
	cout << discrete_score << "/25" << endl;
	SetConsoleTextAttribute(h,15);
    cout << "                                                                         Computer Programming 2                                    ";
	SetConsoleTextAttribute(h,14);
	cout << comprog_score << "/25" << endl;
	SetConsoleTextAttribute(h,15);
    cout << "                                                                         Filipino sa iba't ibang Disiplina                         ";
	SetConsoleTextAttribute(h,14);
	cout << fildis_score << "/25" << endl;
	SetConsoleTextAttribute(h,15);
    cout << "                                                                         National Service Training Program                         ";
	SetConsoleTextAttribute(h,14);
	cout << nstp_score << "/25" << endl;
	SetConsoleTextAttribute(h,15);
    cout << "                                                                         PATHFIT2                                                  ";
	SetConsoleTextAttribute(h,14);
	cout << pathfit_score << "/25" << endl;
    SetConsoleTextAttribute(h,3);
    cout << "\n\n\n\n\t\t\t\t================================================================================================================================================\n\n\n";
    SetConsoleTextAttribute(h,15);
	cout << "\t\t\t\t\t\t\t\t    Do you want to go back to subject selection? (1 = Yes, 2 = Check Grades)" << endl;
    cout << "\t\t\t\t\t\t\t\t    Choose: ";
    cin >> select;
    if(select == '1') {
        cout << "\n\n\n\n\t\t\t\t\t\t\t Returning..." << endl;
        sleep(1.5);
        exitprog = false;
        system("cls");
        return;
    } else if(select == '2') {
        cout << "\n\n\n\n\t\t\t\t\t\t\t Returning to grades..." << endl;
        sleep(1.5);
        system("cls");
        sub_grade();
    } else {
        cout << "\n\n\n\n\t\t\t\t\t\t\t Invalid! please choose 1 or 2" << endl;
    }
}



int main() {
   //loadingScreen();
	userpage();
//   	HANDLE h = GetStdHandle(STD_OUTPUT_HANDLE);
//   	SetConsoleTextAttribute(h,1);
//    
//    bool error = false;
//    
//    while (!((name == adminname && pass == adminpass) || (name == username && pass == userpass))){
//   	cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
//   	cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
//   	cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
//   	cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
//   	cout << "\t\t\t\t\t\t|\t\t|";
//   	SetConsoleTextAttribute(h,3);
//	cout << "===============================================================================";
//	SetConsoleTextAttribute(h,1);
//	cout << "|\t\t|\n";
//   	cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
//   	cout << "\t\t\t\t\t\t|\t\t|";
//   	SetConsoleTextAttribute(h,15);
//   	cout << " -   -   -   -   -   -   -   -   -   -   -   -   -   -   -   -   -   -   -   - ";
//	SetConsoleTextAttribute(h,1);
//	cout << "|\t\t|" << endl;
//   	cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
//   	cout << "\t\t\t\t\t\t|\t\t|";
//   	SetConsoleTextAttribute(h,3);
//	cout << "===============================================================================";
//	SetConsoleTextAttribute(h,1);
//	cout << "|\t\t|\n";
// 	cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
// 	cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
// 	cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
// 	cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
// 	SetConsoleTextAttribute(h,3);
//    cout << "\t\t\t\t=================================================================================================================================================\n\n\n";
//    SetConsoleTextAttribute(h,15);
//    cout << "\t\t\t\t   --      --      --      --      --      --      --     EVALUATION FOR THE HIGHER UPS    --      --      --      --      --      --      --   \n\n" << endl;
//    SetConsoleTextAttribute(h,3);
//    cout << "\t\t\t\t=================================================================================================================================================\n";
//    SetConsoleTextAttribute(h,1);
//    cout << "\t\t\t\t\t\t\t\t\t|\t|\t\t\t\t\t\t|\t|" << endl;
//   	cout << "\t\t\t\t\t\t\t\t\t|\t|\t\t\t\t\t\t|\t|" << endl;
//   	cout << "\t\t\t\t\t\t\t\t\t|\t|\t\t\t\t\t\t|\t|" << endl;
//    SetConsoleTextAttribute(h,3);
//	cout << "\t\t\t\t\t\t\t\t ===============================================================================\n";
//	SetConsoleTextAttribute(h,1);
//	cout << "\t\t\t\t                                                              |                   |\n";
//	cout << "\t\t\t\t                                                              |                   |\n";
//	SetConsoleTextAttribute(h,3);
//	cout << "\t\t\t\t                                                        =================================\n";
//	
//if (error) {
//        cout << "\t\t\t\t                                                              Error Credentials!! \n\n ";
//    }
//    SetConsoleTextAttribute(h,14);
//	cout << "\n\t\t\t\t                                                              USERNAME*\n ";
//    cout << "\t\t\t\t                                                                 = ";
//    SetConsoleTextAttribute(h,15);
//    getline(cin, name);
//     SetConsoleTextAttribute(h, 14);
//        cout << "\t\t\t\t                                                              PASSWORD*\n ";
//        cout << "\t\t\t\t                                                                 = ";
//        SetConsoleTextAttribute(h, 15);
//        pass = "";
//    SetConsoleTextAttribute(h,15);
//     while ((ch = _getch()) != '\r') { 
//        if (ch == '\b') {
//            if (!pass.empty()) {
//               pass.erase(pass.size() - 1);
//                cout << "\b \b"; 
//            }
//        } else {
//            pass += ch;
//            cout << '*';
//        }
//    }
//    
//    if(pass != userpass || pass != adminpass){
//    	cin.clear();
//    	error = true;
//	}
//    SetConsoleTextAttribute(h,15);
//    
//    SetConsoleTextAttribute(h,3);
//	cout << "\n\n\t\t\t\t                                                        =================================\n";
//	sleep(1.5);
//	if(name == adminname && pass == adminpass){
//    	adminpage();
//	}else if(name == username && pass == userpass)
//	{
//	userpage();	
//	}else{
//error = true;
//cin.clear();
//}
//system("cls");
//
//} 

    
    return 0;

}


	
void userpage(){
	HANDLE h = GetStdHandle(STD_OUTPUT_HANDLE);
	int choice;
	bool exitprog = false;
	system("cls");
    while(!exitprog) {
        SetConsoleTextAttribute(h,1);
		cout << "\t\t\t\t  |  |\t\t\t\t  |  |" << endl;
        cout << "\t\t\t\t  |  |\t\t\t\t  |  |" << endl;
        cout << "\t\t\t\t  |  |\t\t\t\t  |  |" << endl;
        cout << "\t\t\t\t  |  |\t\t\t\t  |  |" << endl;
        cout << "\t\t\t\t  |  |\t\t\t\t  |  |" << endl;
        cout << "\t\t\t\t  |  |\t\t\t\t  |  |" << endl;
        cout << "\t\t\t\t  |  |\t\t\t\t  |  |" << endl;
        SetConsoleTextAttribute(h,3);
        cout << "\t\t\t\t========================================\n\n";
        SetConsoleTextAttribute(h,15);
        cout << "\t\t\t\t\tHello," << name << endl;
        cout << "\t\t\t\t\t  Welcome to Main Menu\n" << endl;
        SetConsoleTextAttribute(h,3);
        cout << "\t\t\t\t========================================\n\n\n\n\n\n";
        SetConsoleTextAttribute(h,15);
        cout << "\t\t\t\t\t\t\tHere's your LMS Subject:\t\t\t\t\t\t      Course Code\n" << endl;
        cout << "\t\t\t\t\t\t\t\t [1] Purposive Communication \t\t\t\t\t\t";
        SetConsoleTextAttribute(h,13);
		cout << "(GE5)" << endl;
		SetConsoleTextAttribute(h,15);
        cout << "\t\t\t\t\t\t\t\t [2] Art Appreciation        \t\t\t\t\t\t";
        SetConsoleTextAttribute(h,6);
		cout << "(GE6)" << endl;
		SetConsoleTextAttribute(h,15);
        cout << "\t\t\t\t\t\t\t\t [3] Science and Technology (ST) and Society \t\t\t\t";
        SetConsoleTextAttribute(h,7);
		cout << "(GE7)" << endl;
		SetConsoleTextAttribute(h,15);
        cout << "\t\t\t\t\t\t\t\t [4] Applied Ethics          \t\t\t\t\t\t";
        SetConsoleTextAttribute(h,12);
		cout << "(GE8)" << endl;
		SetConsoleTextAttribute(h,15);
        cout << "\t\t\t\t\t\t\t\t [5] Discrete Mathemathics   \t\t\t\t\t\t";
        SetConsoleTextAttribute(h,2);
		cout << "(MS101)" << endl;
		SetConsoleTextAttribute(h,15);
        cout << "\t\t\t\t\t\t\t\t [6] Computer Programming 2  \t\t\t\t\t\t";
        SetConsoleTextAttribute(h,8);
		cout << "(CC103)" << endl;
		SetConsoleTextAttribute(h,15);
        cout << "\t\t\t\t\t\t\t\t [7] Filipino sa iba't ibang Disiplina \t\t\t\t\t";
        SetConsoleTextAttribute(h,5);
		cout << "(FILDIS)" << endl;
		SetConsoleTextAttribute(h,15);
        cout << "\t\t\t\t\t\t\t\t [8] National Service Training Program \t\t\t\t\t";
        SetConsoleTextAttribute(h,3);
		cout << "(NSTP2)" << endl;
		SetConsoleTextAttribute(h,15);
        cout << "\t\t\t\t\t\t\t\t [9] PATHFIT2                \t\t\t\t\t\t";
        SetConsoleTextAttribute(h,1);
		cout << "(PE2)" << endl;
        SetConsoleTextAttribute(h,14);
        cout << "\t\t\t\t\t\t\t\t [10] View scores" << endl;
        SetConsoleTextAttribute(h,4);
        cout << "\t\t\t\t\t\t\t\t [11] Close" << endl;
        SetConsoleTextAttribute(h,3);
        cout << "\n\n\n\n\n\t\t\t\t================================================================================================================================================\n\n";
        SetConsoleTextAttribute(h,15);
        cout << "\n\n\t\t\t\t\t\t\t Please choose your selection: ";
        cin >> choice;

        char cont;
        switch(choice) {
        case 1:
          system("cls");
          SetConsoleTextAttribute(h,13);
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			SetConsoleTextAttribute(h,15);
          	cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
            SetConsoleTextAttribute(h,13);
			cout << "\t\t\t\t\t\t\t\t\t Do you want to take Purposive communication? (1 = Yes, 2 = No) \n\n\n\n" << endl;
            SetConsoleTextAttribute(h,15);
            cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
            SetConsoleTextAttribute(h,13);
			cout << "\t\t\t\t\t\t\t\t\t\t\t\t Answer: ";
            cin >> cont;
            if(cont == '1') {
                if(purcomm_taken == true) {
                    cout << "\n\n\n\n\t\t\t\t\t\t\t You already taken the purposive communication exam!!" << endl;
                    sleep(1.5);
                    system("cls");
                    exitprog = false;
                }
                else if(comprog_taken == false) {
                    cout << "\n\n\n\n\t\t\t\t\t\t\t Loading...." << endl;
                    sleep(1.5);
                    exitprog = true;
                    purcomm();
                }
            } else if(cont == '2') {
                cout << "\n\n\n\n\t\t\t\t\t\t\t Returning to subject selection...\n";
                sleep(1.5);
                system("cls");
            } else {
                cout << "\n\n\n\n\t\t\t\t\t\t\t Invalid Operator!" << endl;
            }
            break;

        case 2:
            system("cls");
            SetConsoleTextAttribute(h,6);
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			SetConsoleTextAttribute(h,15);
   			cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
            SetConsoleTextAttribute(h,6);
			cout << "\t\t\t\t\t\t\t\t\t     Do you want to take Art Appreciation? (1 = Yes, 2 = No) \n\n\n\n" << endl;
            SetConsoleTextAttribute(h,15);
            cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
            SetConsoleTextAttribute(h,6);
			cout << "\t\t\t\t\t\t\t\t\t\t\t\t Answer: ";
            cin >> cont;
            if(cont == '1') {
                if(artapp_taken == true) {
                    cout << "\n\n\n\n\t\t\t\t\t\t\t You already taken the Art Appreciation exam!!" << endl;
                    sleep(1.5);
                    system("cls");
                    exitprog = false;
                } else if(purcomm_taken == false) {
                    cout << "\n\n\n\n\t\t\t\t\t\t\t Loading...." << endl;
                    sleep(1.5);
                    exitprog = true;
                    artapp();
                }
            } else if(cont == '2') {
                cout << "\n\n\n\n\t\t\t\t\t\t\t Returning to subject selection...\n" << endl;
                sleep(1.5);
                system("cls");
            } else {
                system("cls");
                cout << "\n\n\n\n\t\t\t\t\t\t\t Invalid operator" << endl;
            }
            break;

        case 3:
            system("cls");
            SetConsoleTextAttribute(h,7);
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			SetConsoleTextAttribute(h,15);
   			cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
            SetConsoleTextAttribute(h,7);
			cout << "\t\t\t\t\t\t\t\t     Do you want to take Science, Technology, and Society? (1 = Yes, 2 = No) \n\n\n\n" << endl;
            SetConsoleTextAttribute(h,15);
            cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
            SetConsoleTextAttribute(h,7);
			cout << "\t\t\t\t\t\t\t\t\t\t\t\t Answer: ";
            cin >> cont;
            if(cont == '1'){
              if(sts_taken == true){
              cout << "\n\n\n\n\t\t\t\t\t\t\t You already taken the STS exam!!" << endl;
              sleep(1.5);
              system("cls");
              exitprog = false;
              } else if(sts_taken == false){
              cout << "\n\n\n\n\t\t\t\t\t\t\t Loading..." << endl;
              sleep(1.5);
              system("cls");
              exitprog = true;
              sts();
              }
            } else if(cont == '2'){
            cout << "\n\n\n\n\t\t\t\t\t\t\t Returning to subject selection..." << endl;
            sleep(1.5);
            system("cls");
            } else {
            system("cls");
            cout << "\n\n\n\n\t\t\t\t\t\t\t Invalid Operator" << endl;
            }
          break;
        
        
        case 4:
         system("cls");
         SetConsoleTextAttribute(h,12);
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			SetConsoleTextAttribute(h,15);
   			cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
        	SetConsoleTextAttribute(h,12);
			cout << "\t\t\t\t\t\t\t\t\t       Do you want to take Applied Ethics? (1 = Yes, 2 = No) \n\n\n\n" << endl;
        	SetConsoleTextAttribute(h,15);
        	cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
        	SetConsoleTextAttribute(h,12);
			cout << "\t\t\t\t\t\t\t\t\t\t\t\t Answer: ";
       	 	cin >> cont;
         	if(cont == '1'){
         		if(ethics_taken = true){
         		cout << "\n\n\n\n\t\t\t\t\t\t\t You already take the exam\n";
         		sleep(1);
         		system("cls");
			 } 
			 }else if(ethics_taken = false){
         	cout << "\n\n\n\n\t\t\t\t\t\t\t Loading..." << endl;
         	exitprog = true; 
            system("cls");
         	ethics();
		 } else if(cont == '2'){
		 	cout << "\n\n\n\n\t\t\t\t\t\t\t Returning to subject selection...";
		 	sleep(1.5);
		 	system("cls");
		 	exitprog = false;
	
		 } else {
		 	cout << "\n\n\n\n\t\t\t\t\t\t\t Invalid Operator" << endl;
		 }
		 
		 break;
         
         
         case 5: //discrete
         	system("cls");
         	SetConsoleTextAttribute(h,2);
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			SetConsoleTextAttribute(h,15);
   			cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
         	SetConsoleTextAttribute(h,2);
			 cout << "\t\t\t\t\t\t\t\t\t      Do you want to take Discrete Math? (1 = Yes, 2 = No) \n\n\n\n" << endl;
         	SetConsoleTextAttribute(h,15);
         	cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
        	SetConsoleTextAttribute(h,2);
			cout << "\t\t\t\t\t\t\t\t\t\t\t\t Answer: ";
         	cin >> cont;
         	if(cont == '1'){
			 
         		if(discrete_taken = true){
         		cout << "\n\n\n\n\t\t\t\t\t\t\t You already take the exam\n";
         		cout << "\n\n\n\n\t\t\t\t\t\t\t Returning to subject....";
         		sleep(1);
         		system("cls");
			 }
			 } else if(discrete_taken = false){
			cout << "\n\n\n\n\t\t\t\t\t\t\t Loading..." << endl;
         	exitprog = true;
            system("cls");
         	discrete();
			 }  else if(cont == '2'){
		 	cout << "\n\n\n\n\t\t\t\t\t\t\t Returning to subject selection...";
		 	sleep(1.5);
		 	system("cls");
		 	exitprog = false;
		 } else {
		 	cout << "\n\n\n\n\t\t\t\t\t\t\t Invalid Operator" << endl;
		 }
		 break;
		 case 6: //comprog
			system("cls");
			SetConsoleTextAttribute(h,8);
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			SetConsoleTextAttribute(h,15);
   			cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
         	SetConsoleTextAttribute(h,8);
			cout << "\t\t\t\t\t\t\t\t\t Do you want to take Computer Programming? (1 = Yes, 2 = No) \n\n\n\n" << endl;
         	SetConsoleTextAttribute(h,15);
         	cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
        	SetConsoleTextAttribute(h,8);
			cout << "\t\t\t\t\t\t\t\t\t\t\t\t Answer: ";
         	cin >> cont;
         	if(cont == '1'){
         		if(comprog_taken == true){
         		cout << "\n\n\n\n\t\t\t\t\t\t\t You already take the exam\n";
         		cout << "\n\n\n\n\t\t\t\t\t\t\t Returning to subject....";
         		sleep(1);
         		system("cls");
         		} else if(comprog_taken == false){
         	 cout << "\n\n\n\n\t\t\t\t\t\t\t Loading...." << endl;
                     sleep(1.5);
                    exitprog = true;
                system("cls");
         	    comprog();
            }
			}else if(cont == '2'){
         	  cout << "\n\n\n\n\t\t\t\t\t\t\t Returning to subject selection...\n";
                sleep(1.5);
                system("cls");
            } else {
                cout << "\n\n\n\n\t\t\t\t\t\t\t Invalid Operator!" << endl;
            
		 }
         
				 
				 break;
				 
		case 7: //fildis
			system("cls");
			SetConsoleTextAttribute(h,5);
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
			SetConsoleTextAttribute(h,15);
   			cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
			SetConsoleTextAttribute(h,5);
			cout << "\t\t\t\t\t\t\t\t\t\t Do you want to take FILDIS? (1 = Yes, 2 = No) \n\n\n\n " << endl;
			SetConsoleTextAttribute(h,15);
			cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
        	SetConsoleTextAttribute(h,5);
			cout << "\t\t\t\t\t\t\t\t\t\t\t\t Answer: ";
				cin >> cont;
				 	if(cont == '1'){
         		if(fildis_taken == true){
         		cout << "\n\n\n\n\t\t\t\t\t\t\t You already take the exam\n";
         		cout << "\n\n\n\n\t\t\t\t\t\t\t Returning to subject....";
         		sleep(1);
         		system("cls");
         		} else if(fildis_taken == false){
         	 cout << "\n\n\n\n\t\t\t\t\t\t\t Loading...." << endl;
                     sleep(1.5);
                    exitprog = true;
                system("cls");
         	    fildis();
            }
			}else if(cont == '2'){
         	  cout << "\n\n\n\n\t\t\t\t\t\t\t Returning to subject selection...\n";
                sleep(1.5);
                system("cls");
            } else {
                cout << "\n\n\n\n\t\t\t\t\t\t\t Invalid Operator!" << endl;
            
		 }
				 
				 
				 break;
				 
			case 8: //nstp
			system("cls");
			SetConsoleTextAttribute(h,3);
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			SetConsoleTextAttribute(h,15);
   			cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;	 
			SetConsoleTextAttribute(h,3);
			cout << "\t\t\t\t\t\t\t\t\t\t Do you want to take NSTP2? (1 = Yes, 2 = No) \n\n\n\n " << endl;
			SetConsoleTextAttribute(h,15);
			cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
        	SetConsoleTextAttribute(h,3);
			cout << "\t\t\t\t\t\t\t\t\t\t\t\t Answer: ";
				 cin >> cont;
					if(cont == '1'){
         		if(nstp_taken == true){
         		cout << "\n\n\n\n\t\t\t\t\t\t\t You already take the exam\n";
         		cout << "\n\n\n\n\t\t\t\t\t\t\t Returning to subject....";
         		sleep(1);
         		system("cls");
         		} else if(nstp_taken == false){
         	 cout << "\n\n\n\n\t\t\t\t\t\t\t Loading...." << endl;
                     sleep(1.5);
                    exitprog = true;
                system("cls");
         	    nstp();
            }
			}else if(cont == '2'){
         	  cout << "\n\n\n\n\t\t\t\t\t\t\t Returning to subject selection...\n";
                sleep(1.5);
                system("cls");
            } else {
                cout << "\n\n\n\n\t\t\t\t\t\t\t Invalid Operator!" << endl;
            
		 }
		 
		 break;
		 
		 	case 9: //pathfit
		 	system("cls");
		 	SetConsoleTextAttribute(h,1);
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			cout << "\t\t\t\t\t\t|\t\t|\t\t\t\t\t\t\t\t\t\t|\t\t|" << endl;
   			SetConsoleTextAttribute(h,15);
   			cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
			SetConsoleTextAttribute(h,1);
			cout << "\t\t\t\t\t\t\t\t\t\t Do you want to take NSTP2? (1 = Yes, 2 = No) \n\n\n\n " << endl;
			SetConsoleTextAttribute(h,15);
		 	cout << "\t\t\t\t=================================================================================================================================================\n\n\n\n" << endl;
        	SetConsoleTextAttribute(h,1);
			cout << "\t\t\t\t\t\t\t\t\t\t\t\t Answer: ";
		 	cin >> cont;
		 	if(cont == '1'){
         		if(pathfit_taken == true){
         		cout << "\n\n\n\n\t\t\t\t\t\t\t You already take the exam\n";
         		cout << "\n\n\n\n\t\t\t\t\t\t\t Returning to subject....";
         		sleep(1);
         		system("cls");
         		} else if(pathfit_taken == false){
         	 cout << "\n\n\n\n\t\t\t\t\t\t\t Loading...." << endl;
                     sleep(1.5);
                    exitprog = true;
                system("cls");
         	    pathfit();
            }
			}else if(cont == '2'){
         	  cout << "\n\n\n\n\t\t\t\t\t\t\t Returning to subject selection...\n";
                sleep(1.5);
                system("cls");
            } else {
                cout << "\n\n\n\n\t\t\t\t\t\t\t Invalid Operator!" << endl;
            
		 }
		 
		 break;
		 
				 
				 
        
		case 10:
            cout << "\n\n\n\n\t\t\t\t\t\t Returning to scores..." << endl;
            sleep(1.5);
            exitprog = true;
            subscore();
            break;

       
            
        
        	
        case 11:
            cout << "\n\n\n\n\t\t\t\t\t\t Exiting LMS... Thank You" << endl;
            sleep(1.5);
            exitprog = true;
            exit;
            break;
            
     
		        
        default:
            system("cls");
            cout << "\nInvalid Operator! " << endl;
            exitprog = false;
        }
    }
    
}






	string name;
	HANDLE h = GetStdHandle(STD_OUTPUT_HANDLE);
	int choice;
	bool exitprog = false;
	system("cls");
    while(!exitprog) {
        SetConsoleTextAttribute(h,1);
        cout << "\t\t\t\t \\____________________________________/" << endl;
        cout << "\t\t\t\t  |  |\t\t\t\t  |  |" << endl;
        cout << "\t\t\t\t  |  |\t\t\t\t  |  |" << endl;
        SetConsoleTextAttribute(h,3);
        cout << "\t\t\t\t========================================\n\n";
        SetConsoleTextAttribute(h,15);
        cout << "\t\t\t\t\tHello," << name << endl;
        cout << "\t\t\t\t\t  Welcome to Main Menu\n" << endl;
        SetConsoleTextAttribute(h,3);
        cout << "\t\t\t\t========================================\n";
        SetConsoleTextAttribute(h,1);
        cout << "\t\t\t\t  |  |\t\t\t\t  |  |" << endl;
        cout << "\t\t\t\t  |  |\t\t\t\t  |  |" << endl;
        SetConsoleTextAttribute(h,3);
        cout << "\t\t\t\t================================================================================================================================================\n\n";
        SetConsoleTextAttribute(h,15);
        cout << "\t\t\t\t\tHere's your LMS Subject:\n" << endl;
        SetConsoleTextAttribute(h,13);
        cout << "\t\t\t\t                |============================|";
		SetConsoleTextAttribute(h,6);
		cout << "		|============================|";
		SetConsoleTextAttribute(h,7);
		cout << "		|============================|" << endl;
		SetConsoleTextAttribute(h,13);
        cout << "\t\t\t\t                |                            |";
		SetConsoleTextAttribute(h,6);
		cout << "		|                            |";
		SetConsoleTextAttribute(h,7);
		cout << "		|                            |" << endl;
		SetConsoleTextAttribute(h,13);
		cout << "\t\t\t\t                |       [1] Purposive        |";
		SetConsoleTextAttribute(h,6);
		cout << "		|    [2] Art Appreciation    |";
		SetConsoleTextAttribute(h,7);
		cout << "		| [3] Science Technology and |" << endl;
		SetConsoleTextAttribute(h,13);
    	cout << "\t\t\t\t                |     Communication (GE5)    |";
		SetConsoleTextAttribute(h,6);
		cout << "		|            (GE6)           |";
		SetConsoleTextAttribute(h,7);
		cout << "		|        Society (GE7)       |" << endl;
		SetConsoleTextAttribute(h,13);
        cout << "\t\t\t\t                |                            |";
		SetConsoleTextAttribute(h,6);
		cout << "		|                            |";
		SetConsoleTextAttribute(h,7);
		cout << "		|                            |" << endl;
		SetConsoleTextAttribute(h,13);
        cout << "\t\t\t\t                |============================|";
		SetConsoleTextAttribute(h,6);
		cout << "		|============================|";
		SetConsoleTextAttribute(h,7);
		cout << "		|============================|\n\n" << endl;
		SetConsoleTextAttribute(h,12);
        cout << "\t\t\t\t                |============================|";
		SetConsoleTextAttribute(h,2);
		cout << "		|============================|";
		SetConsoleTextAttribute(h,8);
		cout << "		|============================|" << endl;
		SetConsoleTextAttribute(h,12);
        cout << "\t\t\t\t                |                            |";
		SetConsoleTextAttribute(h,2);
		cout << "		|                            |";
		SetConsoleTextAttribute(h,8);
		cout << "		|                            |" << endl;
		SetConsoleTextAttribute(h,12);
		cout << "\t\t\t\t                |     [4] Applied Ethics     |";
		SetConsoleTextAttribute(h,2);
		cout << "		|        [5] Discrete        |";
		SetConsoleTextAttribute(h,8);
		cout << "		| [6] Computer Programming 2 |" << endl;
		SetConsoleTextAttribute(h,12);
    	cout << "\t\t\t\t                |            (GE8)           |";
		SetConsoleTextAttribute(h,2);
		cout << "		|    Mathemathics (MS101)    |";
		SetConsoleTextAttribute(h,8);
		cout << "		|           (CC103)          |" << endl;
        SetConsoleTextAttribute(h,12);
        cout << "\t\t\t\t                |                            |";
		SetConsoleTextAttribute(h,2);
		cout << "		|                            |";
		SetConsoleTextAttribute(h,8);
		cout << "		|                            |" << endl;
		SetConsoleTextAttribute(h,12);
        cout << "\t\t\t\t                |============================|";
		SetConsoleTextAttribute(h,2);
		cout << "		|============================|";
		SetConsoleTextAttribute(h,8);
		cout << "		|============================|\n\n" << endl;
		SetConsoleTextAttribute(h,5);
        cout << "\t\t\t\t                |============================|";
		SetConsoleTextAttribute(h,3);
		cout << "		|============================|";
		SetConsoleTextAttribute(h,1);
		cout << "		|============================|" << endl;
		SetConsoleTextAttribute(h,5);
		cout << "\t\t\t\t                |                            |";
		SetConsoleTextAttribute(h,3);
		cout << "		|                            |";
		SetConsoleTextAttribute(h,1);
		cout << "		|                            |" << endl;
		SetConsoleTextAttribute(h,5);
		cout << "\t\t\t\t                |   [7] Filipino sa iba't    |";
		SetConsoleTextAttribute(h,3);
		cout << "		|    [8] National Service    |";
		SetConsoleTextAttribute(h,1);
		cout << "		|        [9] PATHFIT2        |" << endl;
		SetConsoleTextAttribute(h,5);
        cout << "\t\t\t\t                |  ibang Disiplina (FILDIS)  |";
		SetConsoleTextAttribute(h,3);
		cout << "		|  Training Program (NSTP2)  |";
		SetConsoleTextAttribute(h,1);
		cout << "		|            (PE2)           |" << endl;
		SetConsoleTextAttribute(h,5);
		cout << "\t\t\t\t                |                            |";
		SetConsoleTextAttribute(h,3);
		cout << "		|                            |";
		SetConsoleTextAttribute(h,1);
		cout << "		|                            |" << endl;
		SetConsoleTextAttribute(h,5);
        cout << "\t\t\t\t                |============================|";
		SetConsoleTextAttribute(h,3);
		cout << "		|============================|";
		SetConsoleTextAttribute(h,1);
		cout << "		|============================|\n" << endl;
        SetConsoleTextAttribute(h,14);
        cout << "\t\t\t\t                                    |============================|";
        SetConsoleTextAttribute(h,4);
        cout << "          |============================|" << endl;
        SetConsoleTextAttribute(h,14);
        cout << "\t\t\t\t                                    |      [10] View scores      |"; 
        SetConsoleTextAttribute(h,4);
        cout << "          |         [11] Close         |" << endl;
        SetConsoleTextAttribute(h,14);
		cout << "\t\t\t\t                                    |============================|";   
        SetConsoleTextAttribute(h,4);
        cout << "          |============================|" << endl;
        SetConsoleTextAttribute(h,3);
        cout << "\n\t\t\t\t================================================================================================================================================\n\n";
        SetConsoleTextAttribute(h,15);
        cout << "\t\t\t\t\t\t\t Please choose your selection: ";
        cin >> choice;
    }
	return 0;
}
