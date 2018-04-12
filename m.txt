#include <stdio.h>
int main ()
{
char answer;
int Table; int length;
printf("\n Do you wan to continue?: (Y/N) ");
scanf("%c",&answer);

if(answer=='y'||answer=='Y')
{

jump_point:

printf("\n Please enter the Multiplication Table: ");
scanf("%d",&Table);
printf("\n Enter the Length of the Table: ");
scanf("%d",&length);

for(int x=1; x<=length; x=x+1)
{
printf("\n %d*%d=%d", x, Table, x*Table);
}
}

printf("\n Do you want to try another Table? (Y/N)");
scanf("%s",&answer);

if(answer=='y'||answer=='Y')
    goto jump_point;

else(answer=='n'||answer=='N');

return 0;
}
