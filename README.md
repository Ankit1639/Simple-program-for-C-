# Simple-program-for-C
//using only two library files.
#include<fstream.h>
#include<conio.h>
void main()
{
Char x;
ifstream ifile;
ofstream o1,o2,o3;
o1.open("base.txt",ios::in);
o2.open("copy.txt",ios::out);
o3.open("copy1.txt",ios::out);
while(!ifile.eof())
{
 ifile.get(x);
 o1.put(x);
 o2.put(x);
 o3.put(x);
 }
 ifile.close();
 o1.close();
 o2.close();
 o3.close();
 getch();
 }
