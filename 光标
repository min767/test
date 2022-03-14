#include <stdio.h>
#include <stdlib.h>
#include<windows.h>
#include<conio.h>

int main()
{	char str[10][17]=
	{
		"********###****",
		"###*****###****",
		"###*****###****",
		"###*****###****",
		"###*****###****",
		"###*****###****",
		"###**S**###****",
		"###*****###****",
		"###*****###****",
		"###*****###****"};
	int ch;
	COORD pos;
	pos.X = 0 ;
	pos.Y = 0 ;
	while(1)
           {    system("cls");
	int i,j;
             for(i=0;i<10;i++)
             { for(j=0;j<17;j++)
           
            	printf("%c",str[i][j]);
            	printf("\n");
            } 
	    SetConsoleCursorPosition(GetStdHandle(STD_OUTPUT_HANDLE),pos);
                    ch=getch();
         	 if (str[pos.Y][pos.X]=='S') 
	        {system("cls");
	        printf("恭喜找到了！\n");
	        break;}
		switch(ch)
		
		{    
                                  case 'w':  
                                  --pos.Y;    
		        if(pos.Y<1) pos.Y=0;
		        if(str[pos.Y][pos.X]=='#')
	                          ++pos.Y;break;
	                          
                                 case 's':
                                      ++pos.Y;
		       if(str[pos.Y][pos.X]=='#')
                                      --pos.Y;  
		        if(pos.Y>9) pos.Y=9; break;
			   
	                    case 'a':
                                      --pos.X;
                                 if(str[pos.Y][pos.X]=='#')
	                          ++pos.X;
		              if(pos.X<1) pos.X=0;break;
			
	                      case 'd':
	                           ++pos.X;
	                      if(str[pos.Y][pos.X]=='#')
	                          --pos.X;
	                      if(pos.X>14) pos.X=14;break; 			
                            } }}
