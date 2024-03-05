#include<stdio.h>
int main(){
char oparator,c;
int a,b;
jump:
printf("Enter the oparator:(+,-,*,/)");
scanf("%c",& oparator);
printf("Enter two number:");
scanf("%d %d",&a,&b);
switch(oparator){

case'+':
    printf("%d+%d=%d",a,b,a+b);
    break;
case'-':
    printf("%d-%d=%d",a,b,a-b);
    break;
case'*':
printf("%d*%d=%d",a,b,a*b);
break;
case'/':
    printf("%d/%d=%d",a,b,a/b);
    break;
default:
    printf("your input is not currect & try again");
    scanf("%c",&c);
    goto jump;
}
return 0;
}
