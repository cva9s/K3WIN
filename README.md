# K3WIN
//code starts from here
#include <stdio.h>
#include<string.h>

int main(void) {
	// your code goes here
	int n;
	scanf("%d",&n);
	char ch[n];
	int i,count=0,sum=0;
	scanf("%s",ch);
	n=strlen(ch);
	for(i=0;ch[i]!='\0';i++)
	{
	    if(ch[i]=='a' ||ch[i]=='A' ||ch[i]=='e' ||ch[i]=='E' ||ch[i]=='i' 
	    ||ch[i]=='I' ||ch[i]=='o' ||ch[i]=='O' ||ch[i]=='u' ||ch[i]=='U')
	 {   count++;
	 }
    if(ch[i]>='A' && ch[i]<='Z')
    {
        sum++;
    }
	}
	if(sum>count)
	printf("YES");
	else
	printf("NO");
	
	return 0;
}
