# rock-paper-scissors-lizard-spock
C++ based rpsls beginner code!

#include <iostream>
#include <stdlib.h>
#include <ctime>
#include <locale>

int main(){
  srand(time(NULL));
  int computer = rand() % 3+1;
  int user = 0;
  char answer;
  bool play_again = false;
  while(!play_again){
  std::cout << "==================================\n";
  std::cout << "Rock Paper Scissors Lizard Spock!\n";
  std::cout << "==================================\n";

  std::cout << "1) Eock\n";
  std::cout << "2) Paper\n";
  std::cout << "3) Scissors\n";
  std::cout << "4) Lizard\n";
  std::cout << "5) Spock\n";

  std::cout << "Choose one! ";
  std::cin>>user;
  if(user == 1){
    std::cout<<"You choose rock\n";
  }else if(user ==2){
    std::cout<<"You choose paper\n";
  }else if(user ==3){
    std::cout<<"You choose scissors\n";
  }else if(user ==4){
    std::cout<<"You choose lizard\n";
  }else if(user ==5){
    std::cout<<"You choose spock\n";
  }
  else{
    std::cout<<"Invalid input.";
  }

  if(computer == 1){
    std::cout<<"Computer chooses rock\n";
  }else if(computer ==2){
    std::cout<<"Computer chooses paper\n";
  }else if(computer ==3){
    std::cout<<"Computer chooses scissors\n";
  }else if(computer ==4){
    std::cout<<"Computer chooses lizard\n";
  }else if(computer ==5){
    std::cout<<"Computer chooses spock\n";
  }
  else{
    std::cout<<"Invalid input.";
  }

if(user == computer){
  std::cout<<"It's a tie!";

//Scissors cuts Paper,Paper covers Rock,Rock crushes Lizard,Lizard poisons Spock,Spock smashes Scissors,Scissors decapitate Lizard,Lizard eats Paper,Paper disproves Spock,Spock vaporizes Rock, Rock crushes Scissors.
// 1 rock 2 paper 3 scissors 4 lizard 5 spock

//you choose rock
}else if (user == 1){
  if (computer == 2){
    std::cout <<"You got covered! boo";
  }
  if (computer == 3){
    std::cout <<"You crush the computer! yay";
  }
  if (computer == 4){
    std::cout <<"You crush the computer! yay";
  }
  if (computer ==5){
    std::cout<<"You got vaporized! boo";
  }

//Scissors cuts Paper,Paper covers Rock,Rock crushes Lizard,Lizard poisons Spock,Spock smashes Scissors,Scissors decapitate Lizard,Lizard eats Paper,Paper disproves Spock,Spock vaporizes Rock, Rock crushes Scissors.
// 1 rock 2 paper 3 scissors 4 lizard 5 spock

//you choose paper
}else if(user ==2){
  if (computer == 1){
    std::cout <<"You cover the computer! yay";
  }
  if (computer ==3){
    std::cout <<"You got cut! boo";
  }
  if (computer ==4){
    std::cout<<"You got eaten! boo";
  }
  if (computer ==5){
    std::cout <<"You disproves the computer! yay";
  }

//Scissors cuts Paper,Paper covers Rock,Rock crushes Lizard,Lizard poisons Spock,Spock smashes Scissors,Scissors decapitate Lizard,Lizard eats Paper,Paper disproves Spock,Spock vaporizes Rock, Rock crushes Scissors.
// 1 rock 2 paper 3 scissors 4 lizard 5 spock

//you choose scissors
}else if(user ==3){
  if (computer ==1){
    std::cout<<"You got crushed! boo";
  }
  if (computer ==2){
    std::cout <<"You cut the computer! yay";
  }
  if (computer == 4){
    std::cout <<"You decapitate the computer! yay";
  }
  if (computer ==5){
    std::cout <<"You got smashed! boo";
  }

//Scissors cuts Paper,Paper covers Rock,Rock crushes Lizard,Lizard poisons Spock,Spock smashes Scissors,Scissors decapitate Lizard,Lizard eats Paper,Paper disproves Spock,Spock vaporizes Rock, Rock crushes Scissors.
// 1 rock 2 paper 3 scissors 4 lizard 5 spock

//you choose lizard
}else if(user ==4){
  if (computer ==1){
    std::cout<<"You got crushed! boo";
  }
  if (computer ==2){
    std::cout <<"You eat the computer! yay";
  }
  if (computer ==3){
    std::cout<<"You got decapitated! boo";
  }
  if (computer ==5){
    std::cout<<"You poison the computer! yay";
  }
//Scissors cuts Paper,Paper covers Rock,Rock crushes Lizard,Lizard poisons Spock,Spock smashes Scissors,Scissors decapitate Lizard,Lizard eats Paper,Paper disproves Spock,Spock vaporizes Rock, Rock crushes Scissors.
// 1 rock 2 paper 3 scissors 4 lizard 5 spock

//you choose spock
}else if(user ==5){
  if (computer ==1){
    std::cout<<"You vaporize the computer! yay";
  }
  if (computer ==2){
    std::cout <<"You got disproved! boo";
  }
  if (computer ==3){
    std::cout<<"You smash the computer! yay";
  }
  if (computer ==4){
    std::cout<<"You got poisoned! boo";
  }
}
std::cout <<"\n Thank you for playing! ^^";

std::cout << "\nWant to play again (y / n)?";
std::cin >> answer;
answer = std::toupper(answer);
if (answer=='y'){
    play_again = true;
}else{
    std::cout<<"Bye then!";
    return 0;
}
}
}
