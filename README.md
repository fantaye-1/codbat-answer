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
Return true if the given string contains between 1 and 3 'e' chars.
stringE("Hello") → true
stringE("Heelle") → true
stringE("Heelele") → false

Answer:-  public boolean stringE(String str) {
          int count =0;
          for(int i= 0; i < str.length(); i++){
            if(str.charAt(i) == 'e'){
              count++;
            }
          }
          return (count >0)&&(count <= 3);
        }
Given a string, return a new string where the last 3 chars are now in upper case. If the string has less than 3 chars, uppercase whatever is there. Note that str.toUpperCase() returns the uppercase version of a string.
endUp("Hello") → "HeLLO"
endUp("hi there") → "hi thERE"
endUp("hi") → "HI"

Answer :- public String endUp(String str) {
          int len = str.length();
          if(len >= 3){
            return str.substring(0, len-3) + str.substring(len-3 , len).toUpperCase();
          }
            return str.toUpperCase();
        }



Given a non-empty string and an int N, return the string made starting with char 0, and then every Nth char of the string. So if N is 3, use char 0, 3, 6, ... and so on. N is 1 or more.
everyNth("Miracle", 2) → "Mrce"
everyNth("abcdefg", 2) → "aceg"
everyNth("abcdefg", 3) → "adg"

Answer:-  public String everyNth(String str, int n) {
              int len = str.length();
              String val = "";

              for(int i=n; i < len; i=i+n){
                val =val +  str.substring(i,i+1);
              }

              return str.substring(0,1) + val;
            }

We have two monkeys, a and b, and the parameters aSmile and bSmile indicate if each is smiling. We are in trouble if they are both smiling or if neither of them is smiling. Return true if we are in trouble.
monkeyTrouble(true, true) → true
monkeyTrouble(false, false) → true
monkeyTrouble(true, false) → false

Answer:-\   public boolean monkeyTrouble(boolean aSmile, boolean bSmile) {
              return aSmile == bSmile;
            }
            
 Given two int values, return their sum. Unless the two values are the same, then return double their sum.
sumDouble(1, 2) → 3
sumDouble(3, 2) → 5
sumDouble(2, 2) → 8      

Ansewr:-    public int sumDouble(int a, int b) {
                int dsum =1;
                if(a == b){
                  dsum = 2;
                }
                return dsum*(a +b) ;
              }
Given an int n, return the absolute difference between n and 21, except return double the absolute difference if n is over 21.


diff21(19) → 2
diff21(10) → 11
diff21(21) → 0

 Answer :-     public int diff21(int n) {
                  int dvalue = 1;
                  if(n > 21) dvalue = 2;

                  return dvalue *(Math.abs(21 - n));        
                }

We have a loud talking parrot. The "hour" parameter is the current hour time in the range 0..23. We are in trouble if the parrot is talking and the hour is before 7 or after 20. Return true if we are in trouble.
parrotTrouble(true, 6) → true
parrotTrouble(true, 7) → false
parrotTrouble(false, 6) → false

Answer:-         public boolean parrotTrouble(boolean talking, int hour) {
                   if((talking == true) && (hour > 20 || hour < 7 ) ){
                     return true;
                   }
                     return false;
                  }
Given 2 ints, a and b, return true if one if them is 10 or if their sum is 10.
makes10(9, 10) → true
makes10(9, 9) → false
makes10(1, 9) → true

Answer:- public boolean makes10(int a, int b) {
            if(a == 10 || b == 10  || (a+b)== 10){
              return true;
            }
            return false;
          }
          

Given an int n, return true if it is within 10 of 100 or 200. Note: Math.abs(num) computes the absolute value of a number.
nearHundred(93) → true
nearHundred(90) → true
nearHundred(89) → false   

Answer:-     public boolean nearHundred(int n) {
                if(Math.abs(n-100) <= 10 || Math.abs(n-200)<=10 ){
                  return true;
                }
                return false;
              }


 Answer :-     public boolean posNeg(int a, int b, boolean negative) {

                  if((negative == true) && a < 0 && b < 0){
                    return true;
                  }else if((negative == false) && (a < 0 || b < 0 )&&( a > 0 || b > 0)){ 
                    return true;
                  }
                  return false;
                }













