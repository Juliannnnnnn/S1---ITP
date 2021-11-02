# S1---ITP


#include <iostream>
#include <string>
using namespace std;
  
  int main (){
  int age {};
  string name {};
  
  cout <<"Enter your name:" << endl;
  cout <<"Enter your age:" <<endl;
  cin >> name;
  
  if (cin.fail()) {
  
      std::cin.clear();
        std::cout << "Incorrect input\n ";
    }
  
     else { cout <<"Enter the letter of your location, ('R' - Rak, 'U' - Umm-Al-Quwain, 'F' - Fujairah, 'A' - Ajman, 'S' - Sharjah, 'D' - Dubai, 'B' - Abu Dhabi, 'L' - Al Ain" <<endl;
           char letter;
           cin >> letter;
           
        } 
        switch ('R','U','F','A','S','D','B','L')
        {
        
        case 'R': {
            cout <<"Rak, transportation charges are 250 aed" <<endl;
            break;
        }
        case 'U':{
            cout <<"Umm-Al-Quwain, transportation charges are 300 aed" <<endl; 
            break;
        }case 'F':{
            cout <<"Fujairah, transportation charges are 300 aed" <<endl;
            break;
        }case 'A':{
            cout <<"Ajman, transportation charges are 390 aed" <<endl;
            break;
        }case 'S':{
            cout <<"Sharjah, transportation charges are 500 aed" <<endl;
            break;
        }case 'D':{
            cout <<"Dubai, transportation charges are 650 aed" <<endl;
            break;
        }case 'B':{
            cout <<"Abu Dhabi, transportation charges are 1000 aed" <<endl;
            break;
        }case 'L':{
            cout <<"Al Ain, transportation charges are 1000 aed" <<endl;
            break;
        }
        default:
            cout <<"other, no transportation available"; 
            break;
        }
        
        cout << "Do you want to avail transportation? Enter:(Y/N): "; 
		char answer; 
		cin >> answer; 

			switch (answer)
			{ 
			
			case 'Y':
			case 'y':
			{
				cout << "Your transportation is confirmed";
				break;
			}
					
			case 'N':
			case 'n':
			{
				cout << "Your transporatation is cancelled";
				break;
			}
					
			default: 
			{
				cout << "incorrect command";
			}

			} {
		cin.get(); 
		return 0;
}
}
