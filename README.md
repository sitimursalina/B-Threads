# B-Threads
Company B-request threads features

package ThreadB;

public class ThreadB {

   public static void main (String [] args)
	    {
	   //BT-threads request for company B
	   CompBThread BT = new CompBThread ();
	   BT.start ();
	      for (int t = 0; t < 50; t++)
	           System.out.println ("t = " + t + ", t * t = " + t * t);
	   }
	   
}
class CompBThread extends Thread
{
	   public void run ()
	   {
	   
	   for (int count = 1, row = 1; row < 20; row++, count++)
	      {
	      
	      for (int t = 0; t < count; t++)
	                System.out.print ('#');
	           //to enter newline
	           System.out.print ('\n');
	   
	   	      }
	   }
	}
