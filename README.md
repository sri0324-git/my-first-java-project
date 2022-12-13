# my-first-java-project
typing calculator 


package basics;
import java.time.LocalTime;
import java.util.Random;
import java.util.Scanner;
import java.util.concurrent.TimeUnit;

public class JavaPrograms {

  static String[] words = {"determination","technology","most","useful","science","general","population","transform","gadgets","devices"};
	
         public static void main(String[] args)  throws InterruptedException {
           System.out.println("3");
           TimeUnit.SECONDS.sleep(1);
		
	System.out.println("2");
	TimeUnit.SECONDS.sleep(1);
		
	System.out.println("1");
	TimeUnit.SECONDS.sleep(1);
	
	Random rand =new Random();
	for(int i=0;i<10;i++) {
		System.out.print(words[rand.nextInt(9)] +"  ");
	}
	System.out.println();
	
	double start = LocalTime.now().toNanoOfDay();
	
	Scanner scan = new Scanner(System.in);
	String typedWords = scan.nextLine();
	
double end = LocalTime.now().toNanoOfDay();
	double elapsedTime = end - start;
	double seconds = elapsedTime / 1000000000.0;
    int numChars = typedWords.length();
    
    int wpm = (int)((((double) numChars  /5) / seconds)*60);
    
    System.out.println(" YOUR WPM IS " + wpm + "!");
  
	
	
	}
	
}	
