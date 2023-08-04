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
