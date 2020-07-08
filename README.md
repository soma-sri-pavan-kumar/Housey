import java.util.*;
 class Housey
 {
   public static void main(String args[])
   { 
    int count=0;
    Scanner l = new Scanner(System.in);
    Random a = new Random();
    HashSet<Integer> s = new HashSet<Integer> ();
    while(true){
      int r = a.nextInt(91);
      if( r == 0)
      break;
      else
      s.add(r);
      if(s.size() == count+1){
       char p= l.next().charAt(0);
       if(p == '.' && s.contains(r) && s.size() <= 90 ){
        System.out.println(r);
        count++;
        continue;
         } 
       else{                              
        System.out.println("**Game is completed**");
        break;
        }
        }
      else
       continue;
   }
  }
 }
