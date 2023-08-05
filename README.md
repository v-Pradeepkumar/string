# string
//in string if we use \ for consider next line space also but if we use"" for avoid that space. o/pHello bro.    how are you, Hello bro.how are you
#include <stdio.h>

int main() {
   
    printf("%s\n", "Hello bro.\
    how are you");

    printf("%s\n", "Hello bro."
    "how are you");
    return 0;
}






// try to copy a string to array (without null character in array so undefined error occurs)
#include <stdio.h>

int main() {
   char s[5] = "hello";
   char t[5] ;
   int i ;
   for(i = 0 ; s[i] !='\0' ; i++)
   {
       t[i] = s[i] ;
   }
    printf("%s", t) ;
    return 0;
}







// try to copy a string to array with null character then gives correct answer o/p>> hello
#include <stdio.h>

int main() {
   char s[6] = "hello";
   char t[6] ;
   int i ;
   for(i = 0 ; s[i] !='\0' ; i++)
   {
       t[i] = s[i] ;
   }
   t[i] = '\0' ;
    printf("%s", t) ;
    return 0;
}










// writing string using puts(),here we use 2 puts() so it prints 2 times o/p hello hello
#include <stdio.h>

int main() {
    char *s = "hello";
    puts(s);
    puts(s);
    return 0;
}





//"%m.ns" here m is size of string we want to print .n is how many character we want to print in that string , s is for print string datatype
#include <stdio.h>

int main() {
    char *s = "hello";
   printf ("%6.3s",s);      //o/p >> hel
    return 0;
}





// reading  string using scanf i/p>>enter the string:>>   you are most welcome         o/p>>you
// string doesnot print space in string
#include <stdio.h>

int main() {
    char a[10] ;
   printf ("enter the string:\n ");     
   scanf("%s",a) ;
   printf("%s",a);
    return 0;
}




// reading  string using gets() i/p>>enter the string:>>  you are most           o/p>>you are m
// gets() for print space in a string.here we consder the length of the array when it exceed in printf program will segmentation fault 
#include <stdio.h>

int main() {
    char a[10] ;
   printf ("enter the string:\n ");     
   gets(a) ;
   printf("%.9s",a);
    return 0;
}






// designing input function using getchar() i/p >>hello o/p >>5 hello  here o/p contain how many string and actual string 
#include <stdio.h>
int input(char str[], int n)
{
    int ch, i = 0;
    while((ch = getchar()) != '\n')
    if (i < n)
    str[i++] = ch ;
    str[i] = '\0' ;
    return i ;
}
int main() {
    char str[100] ;
    int n = input (str , 5) ;
    printf("%d %s", n , str);

    return 0;
}







// putchar() function in C putchar() is used for print a character  using integer input  o/p >> ABCDEFGHIJKLMNOPQRSTUVWXYZ
#include <stdio.h>

int main() {
    int ch ;
    for(ch = 'A' ; ch <= 'Z' ; ch++)
    putchar( ch ) ;

    return 0;
}









