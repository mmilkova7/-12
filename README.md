#include<iostream>
#include<cstring>
using namespace std;
void reverse (char *rstr, char *wstr)
{
  int rstr_lenght=strlen(rstr);
  for (int i=0;i<rstr_lenght;i++)
  {
       wstr[i]=rstr[rstr_lenght-i-1];
  }
  wstr[rstr_lenght]='\0';
}
int main ()
{
char word[30],drow[30];
for(;;)
{
  cout"\n Enter a word:) Enter a symbol for end\n";
  cin << word;
  reverse(word,drow);  
  cout << drow << endl; 
}
}
