# hackerrank-digit-frequency-


#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    char s[1024],compare[10]; // string bna liye do kyuki char char se hi comapre hoyega
    fgets(s,1024,stdin);
    puts(s);
    printf("%lu \n",strlen(s));
    int len=strlen(s);
    printf("%d \n",len);
    
    for(int i=0;i<10;i++)
    {   compare[i]=i+'0';  // coverting the int in character
    // printf("%c",compare[i]);
        int count=0;
        for(int j=0;j<len;j++)
        {
            if(s[j]==compare[i]){
            count++;}
            if(j==len-1)
            {
                printf("%d ",count);
            }
        }
        
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
