# pratical-no-2A
SINGLE THREAD

class Prime implements Runnable {
  long j. c;
  
   Prime() {
    super();
     c=0;
}
public void run() {
    for (long i=0; i<= 100; i++) {
      for (j=2; j<=i; j++) {
        if (i %j==0)
          break;
       }   
       if (j==i) {
          c++;
          System.out.println(c +"th"+"Prime no:="+i);
        }
      }
    }
  }
  
public class MyPrime {
public static void main(String args[]) { 
     Thread ct Thread.currentThread();
     System.out.println("Main Thread name:" + ct.getName());
     Prime p = new Prime();
     Thread prime = new Thread(p, "prime");
     prime.start();
     System.out.println("Thread" + prime.getN=ame() + "Started.");
    }
  }
