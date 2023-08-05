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











