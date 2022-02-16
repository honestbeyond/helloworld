# helloworld
test1
//in a queue input I and O,I mean input ,O mean output,judge a series queue IOIO
#include <iostream>
using namespace std;
void Judge()
{
  char A[MaxSize] = {0};
  cout << "input chars:";
  cin.getline(A, MaxSize);
  int j = 0;
  for (int i = 0; A[i] != '\0' && j >= 0; i++)
    if (A[i] == 'I')
      j++;
    else
      j--;
  if (j == 0)
    cout << "pass" << endl;
  else
    cout << "illegal" << endl;
}
int main()
{
  Judge();
  return 0;
}
