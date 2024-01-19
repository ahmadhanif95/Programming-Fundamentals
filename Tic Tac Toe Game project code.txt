
#include <iostream>
using namespace std;
char board[3][3]={{1,2,3},{4,5,6},{7,8,9}};
int position;
char x,o;
void displaystructure()
{
	board[0][0] = '1';
	board[0][1] = '2';
	board[0][2] = '3';
	board[1][0] = '4';
	board[1][1] = '5';
	board[1][2] = '6';
	board[2][0] = '7';
	board[2][1] = '8';
	board[2][2] = '9';
	cout<<"                              *******************************"<<endl;
	cout<<"                                   TIC TAC TOE PLAY BORAD    "<<endl;
	cout<<"                              *******************************"<<endl;
    cout<<"                             PLAYER NO 1 = X : PLAYER NO 2 = O"<<endl;
	cout<<"   "<<endl; 
	cout<<"   "<<endl;
	cout<<"   "<<endl;
	cout<<"   "<<endl;
	cout<<"   "<<endl;
	cout<<"                             _____________________________________"<<endl;
    cout<<"                             ||          ||           ||        ||"<<endl; 
    cout<<"                                   "<<board[0][0]<<"           "<<board[0][1]<<"            "<<board[0][2]<<endl;
	cout<<"                             ||          ||           ||        ||"<<endl;
    cout<<"                             _____________________________________"<<endl;
    cout<<"                             ||          ||           ||        ||"<<endl;
    cout<<"                                   "<<board[1][0]<<"           "<<board[1][1]<<"            "<<board[1][2]<<endl;;
	cout<<"                             ||          ||           ||        ||"<<endl;
    cout<<"                             _____________________________________"<<endl;
    cout<<"                             ||          ||           ||        ||"<<endl;
    cout<<"                                   "<<board[2][0]<<"           "<<board[2][1]<<"            "<<board[2][2]<<endl;
	cout<<"                             ||          ||           ||        ||"<<endl;
	cout<<"                             _____________________________________"<<endl;
    system("pause");
    players();
}
void players()
{
	if()
	{
	cout<<"ENTER THE POSITION PLAYER NO 1:";
	cin>>position;
	}
	else if()
	{
	cout<<"ENTER THE POSITION PLAYER NO 2:";
	cin>>position;
	}
	switch(position)
	{
	case 1:
		board[0][0];
	    break;
	case 2:
		board[0][1];
		break;
	case 3:
		board[0][2];
		break;
	case 4:
		board[1][0];
		break;
	case 5:
		board[1][1];
		break;
	case 6:
		board[1][2];
		break;
	case 7:
		board[2][0];
		break;
	case 8:
		board[2][1];
		break;
	case 9:
		board[2][2];
		break;
	default:
		cout<<"INVALID POSITION YOU ENTERED"<<endl;
		break;
	}
	displaystructure();
	check();

} 
bool check()
{
	if(board[0][0]==board[0][1] && board[0][1]==board[0][2])
	{
	
	} 
	else if(board[1][0]==board[1][1] && board[1][1]==board[1][2])
	{
	
	} 
	else if(board[2][0]==board[2][1] && board[2][1]==board[2][2])
	{
	
	} 
	else if(board[0][0]==board[1][0] && board[1][0]==board[2][0])
	{
	
	}
	else if(board[0][1]==board[1][1] && board[1][1]==board[2][1])
	{
	
	}
	else if(board[0][2]==board[1][2] && board[1][2]==board[2][2])
	{
	
	} 
	else if(board[0][0]==board[1][1] && board[1][1]==board[2][2])
	{
	
	}
	else if(board[0][2]==board[1][1] && board[1][1]==board[2][0])
	{
	
	} 
	else
	{

	}

}
int main()
{
	
	while(check())
	{
		displaystructure();
	    players();
		check();
	}
	if()
	{
		cout<<"                              *    *   *    *   *    *   * "<<endl;
		cout<<"                            *   *    *    *    *   *    *  "<<endl; 
		cout<<"                              *    *   *    *   *    *    *"<<endl;
		cout<<"                            * PLAYER NO 1 WINS THE GAME   *"<<endl;
		cout<<"                            *   *    *    *    *   *    *  "<<endl; 
		cout<<"                              *    *   *    *   *    *    *"<<endl;
		cout<<"                            *   *  CONGRAGULATIONS *   *   "<<endl;
		cout<<"                              *    *   *    *   *    *   * "<<endl; 
		cout<<"                            *   *    *    *    *   *    *  "<<endl;
		cout<<"                              *    *   *    *   *    *   * "<<endl;
	
	}
	else if()
	{   
		cout<<"                              *    *   *    *   *    *   * "<<endl;
		cout<<"                            *   *    *    *    *   *    *  "<<endl; 
		cout<<"                              *    *   *    *   *    *    *"<<endl;
		cout<<"                            * PLAYER NO 2 WINS THE GAME   *"<<endl;
		cout<<"                            *   *    *    *    *   *    *  "<<endl; 
		cout<<"                              *    *   *    *   *    *    *"<<endl;
		cout<<"                            *   *  CONGRAGULATIONS *   *   "<<endl;
		cout<<"                              *    *   *    *   *    *   * "<<endl; 
		cout<<"                            *   *    *    *    *   *    *  "<<endl;
		cout<<"                              *    *   *    *   *    *   * "<<endl;
	}
	else
	{
		cout<<"                                YOUR GAME IS END NO ONE WINS"<<endl;
	}
	
    return 0;
}
