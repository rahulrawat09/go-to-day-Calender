//Hello! 
// Enter Date in the format 
 
//            DD MM YYYY (no / only spaces)
//        ex- 23 02 1999
// You will get the day of the week you were born on.    

#include <bits/stdc++.h>
using namespace std;

int main() {

int dd,mm,yy;

cin>>dd>>mm>>yy;

if(dd<1||dd>31||mm<1||mm>12||yy<1||yy%4!=0&&dd>28&&mm==2||yy%4==0&&dd>29&&mm==2||mm==4&&dd>30||mm==6&&dd>30||mm==9&&dd>30||mm==11&&dd>30){
    cout<<"Enter a valid date";
}

else{ 
    yy--;
 int y=yy%400;
 int y1=y/100;
 int l=(y%100)/4;
 int y2=((y%100)-l)+l*2;
 
 y2%=7;
 int od=0;
 
 switch(y1){
     case 1:od+=5;
     break;
     case 2:od+=3;
     break;
     case 3:od+=1;
     break;
     default:    
     break;
 }
  
  od+=y2;
  int d=0;
  yy++;
  
  for(int i=1;i<=mm;i++)
 {
  switch(i){
   case 1:
   break;
   case 2: d+=31;
   break;
   case 3: if(yy%4!=0)
           d+=28;
           else
           d+=29;
   break;
   case 4: d+=31;
   break;
   case 5: d+=30;
   break;
   case 6: d+=31;
   break;
   case 7: d+=30;
   break;
   case 8: d+=31;
   break;
   case 9: d+=31;
   break;
   case 10: d+=30;
   break;
   case 11: d+=31;
   break;
   case 12: d+=30;
   break;
   default:
   break;
  }
  
 }
 d+=dd;
 
 od+=(d%7);
 od%=7;
 
 cout<<"You were born on ";
 switch(od){
     case 1:cout<<"monday";
     break;
     case 2:cout<<"tuesday";
     break;
     case 3:cout<<"wednesday";
     break;
     case 4:cout<<"thursday";
     break;
     case 5:cout<<"friday";
     break;
     case 6:cout<<"saturday";
     break;
     default:cout<<"sunday";
     break;
 }
 cout<<"\n\n\t\t\tTHANK YOU!!!";
}
    return 0;
}
