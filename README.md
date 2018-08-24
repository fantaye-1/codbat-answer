# codbat-answer
I just put some functional cod form codBat for those of u need some insight about it how to do it !!!!.
Given 2 int values, return true if they are both in the range 30..40 inclusive, or they are both in the range 40..50 inclusive.

Given 2 int values, return true if they are both in the range 30..40 inclusive, or they are both in the range 40..50 inclusive.


in3050(30, 31) → true
in3050(30, 41) → false
in3050(40, 50) → true

Answer :-     public boolean in3050(int a, int b) {
              //check if the a and b are in the range 30..40;
              boolean av = a>=30 && a<=40;
              boolean bv = b>=30 && b<=40;
              //check if the a and b are in the range 40..50;
              boolean aav = a>=40 && a<=50;
              boolean bbv = b>=40 && b<=50;
              //return tru if one of the value is in the range of 30...40 or 40..60
              return (av && bv ) || (aav && bbv);
  
  Given 2 positive int values, return the larger value that is in the range 10..20 inclusive, or return 0 if neither is in that range.
max1020(11, 19) → 19
max1020(19, 11) → 19
max1020(11, 9) → 11
  
Answer :-     public int max1020(int a, int b) {
              // chek if the value is in the range...
              boolean av = (a >= 10) && (a <=20);
              boolean bv = (b >= 10) && (b <=20);
              int value =0;

              if ((av && bv ) && (a >= b)) {
                 value = a;
              }else if ((av && bv ) && (a <= b)){
                value = b;
              }else if(av){
                value = a;
              }else if(bv){
                value = b;
              } 
              return value;
            }



