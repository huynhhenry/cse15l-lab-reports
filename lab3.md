# Lab Report 3 
## Henry Huynh | CSE 15L
  	@Test
	public void testReversedWithBug() {
  		int[] input = { 1, 2, 3 };
		assertArrayEquals(new int[]{ 3, 2, 1 }, ArrayExamples.reversed(input));
	}
 
    @Test
    public void testAverageWithoutLowest() {
      double[] input = { 3.0, 1.0, 2.0, 4.0, 5.0 };
      double expected = 3.5;
      
      double result = ArrayExamples.averageWithoutLowest(input);
      assertEquals(expected, result, 0.001);
    }

![image](https://i.imgur.com/Cw5ww8u.png)
![image](https://i.imgur.com/n8kUP9O.png)
Here is the symptom of running the tests, everything works except the one intended to fail.  
Since reversed has the bug that we identified with the Junit test here it is before fixing.    

    static int[] reversed(int[] arr) {
        int[] newArray = new int[arr.length];
        for(int i = 0; i < arr.length; i += 1) {
          arr[i] = newArray[arr.length - i - 1];
        }
        return arr;
    }
    
Here is the method after fixing the bug.    

    static int[] reversed(int[] arr) {
        int[] newArray = new int[arr.length];
        for (int i = 0; i < arr.length; i += 1) {
            newArray[i] = arr[arr.length - i - 1];
        }
        return newArray;
    }
The problem with the reversed method was that it was copying the arrays the wrong way.   
The fix, addressed the issue because now it properly copies the array the correct way to be reveresed. 

![iamge](https://i.imgur.com/ouMhHnc.png)
![image](https://i.imgur.com/mVHMWwG.png)    
Here is two uses of -i which gives us the option to be case insensitive for the string we search for with grep. 
Very useful becasue sometimes words are at the beginning of sentences and are capitalized.   

![image](https://i.imgur.com/EGWIIss.png)
![image](https://github.com/huynhhenry/cse15l-lab-reports/assets/146884910/eb3c465c-d460-4d3f-85a6-b4fe1ae00040)    
This is the addition to the command -c which counts how many times the string is findable. In both cases "henry" and "mixtape"   
were not in any of the files which is a bit surprising. 

![image](https://i.imgur.com/gYVVEBU.png)
![image](https://i.imgur.com/SdQcS8W.png)
This addition -w finds the exact string, so in the case there was none of "Superman" but alot of "Mary", almost the exact oposite of -i,    
this is much more narrow and we know exactly what we want including the case sensitivity and separated by spaces.

![image](https://i.imgur.com/FyEOM1b.png)
This last section of the command in where we add and "^" at the beginning of the string. It signifies a new line so any line that starts with introduction.   
However as we can see, it doesnt work on this library, for the reason that none of the text files start with letters but rather indents. 
So after I edited the file to remove the indent from the first line, it shows the file that I edited with introduction as a start of a line. 

https://www.geeksforgeeks.org/grep-command-in-unixlinux/
This website is what I used to find basic information on grep. The man command was too hard to read, and this website had it esaily readable. It was on the first page of google. 



