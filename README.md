# codbat-answer
I just put some functional cod form codBat for those of u need some insight about it how to do it !!!!.
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
  
  
  
}
I want ot add somthing
&&]&&&)(


