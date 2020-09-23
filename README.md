#1.
#include<stdio.h>
#include<conio.h>
int main()
{
    int x=10, y=10;
    int X=x,Y=y;
    char ch;
    int i=1;
    while(i!=0)
    {
        printf("Enter N,S,W or E");
        scanf("%c",&ch);
        switch (ch)
        {
        case 'N' :
        case 'n':
            y++;
            break;
        case 'S':
        case 's':
            y--;
            break;
        case 'W':
        case 'w':
            x--;
            break;
        case 'E':
        case 'e':
            x++;  
            break;
        default:
            printf("Wrong input");
            break;
        }
        if(x ==7 && y==11)
        {
            printf("Treasure found ");
            break;
        }
        else if(x==5)
        {
            printf("Maneater found");
            break;
        }
        else
        {
            continue;
        }
        
    }
}
