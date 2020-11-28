#include<iostream>
#include<string>

using namespace std;
string player1, player2, word, underscore , guess,usedguess;
int wrong = 0;
int main(){
    string copy = word;
    cout<<"------hello.welcome to HANGMAN world!--------"<<endl;
    cout<<"enter your name, player1"<<endl;
    cin>>player1;
    cout<<"enter your name, player2"<<endl;
    cin>>player2;
    cout<<"ok\t"<<player1<<" and "<<player2<<"\tlet the game begins"<<endl;
    cout<<player1<<" Input the word you want\n"<<player2<<" you have to guess"<<endl;
    cin>>word;
    //SPACE
    for (int x = 0; x < 30; x++)
    {
        cout<< endl;
    }
    //UNDERSCORE
    while (underscore.size() !=word.size())
    {
        underscore.push_back('_');
    }
    cout<<underscore<<endl;
    // MAIN WHILE
    while (wrong<12)
    {
        cin>>guess;
    // IF GUESS ISNT LETTER
    if (guess.size()>1)
    {
        if (guess==word)
        {
            cout<<"thats the right word. congratulation!"<<endl;
            break;
        }
        else
        {
            cout<<underscore<<endl;
            cout<<"wrong word, try again"<<endl;
            cout<<"used: "<<usedguess<<endl;
            wrong++;
        }
        
    }
    
    if (underscore==word)
    {
        cout<<"you win,boyyah!"<<endl;
        break;
    }
    if (wrong==1)
    {
        cout<<"I"<<endl;
    }
    else if (wrong==2)
    {
        cout<<"I"<<endl;
        cout<<"I"<<endl;
    }
    
    else if (wrong==3)
    {
        cout<<"I"<<endl;
        cout<<"I"<<endl;
        cout<<"I"<<endl;
    }
    else if (wrong==4)
    {
        cout<<"I"<<endl;
        cout<<"I"<<endl;
        cout<<"I"<<endl;
        cout<<"I"<<endl;
    }
    else if (wrong==5)
    {
        cout<<"I"<<endl;
        cout<<"I"<<endl;
        cout<<"I"<<endl;
        cout<<"I"<<endl;
        cout<<"I"<<endl;
    }
    else if (wrong==6)
    {
        cout<<"I=="<<endl;
        cout<<"I"<<endl;
        cout<<"I"<<endl;
        cout<<"I"<<endl;
        cout<<"I"<<endl;
    }
     else if (wrong==7)
    {
        cout<<"I=="<<endl;
        cout<<"I O"<<endl;
        cout<<"I"<<endl;
        cout<<"I"<<endl;
        cout<<"I"<<endl;
    }
     else if (wrong==8)
    {
        cout<<"I=="<<endl;
        cout<<"I O"<<endl;
        cout<<"I |"<<endl;
        cout<<"I"<<endl;
        cout<<"I"<<endl;
    }
    else if (wrong==9)
    {
        cout<<"I=="<<endl;
        cout<<"I O"<<endl;
        cout<<"I -|"<<endl;
        cout<<"I"<<endl;
        cout<<"I"<<endl;
    }
    else if (wrong==10)
    {
        cout<<"I=="<<endl;
        cout<<"I O"<<endl;
        cout<<"I -|-"<<endl;
        cout<<"I"<<endl;
        cout<<"I"<<endl;
    }
     else if (wrong==11)
    {
        cout<<"I=="<<endl;
        cout<<"I O"<<endl;
        cout<<"I -|-"<<endl;
        cout<<"I /"<<endl;
        cout<<"I"<<endl;
    }
      else if (wrong==12)
    {
        cout<<"I=="<<endl;
        cout<<"I O"<<endl;
        cout<<"I -|-"<<endl;
        cout<<"I / /"<<endl;
        cout<<"I YOU DIED NIGGA"<<endl;
        cout<<"GAME OVER BRO! the word was:"<<word<<endl;
        break;
    }
    
    }
}
