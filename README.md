# palindrome
import java.util.*;

public class Palindrome 
{
	
	public static boolean palin(String input)
	{
		if(input.length() <= 2)
		{
			System.out.print("true");
			return true;
		}
		else if(input.charAt(0) == input.charAt(input.length() -1))
		{
			palin(input.substring(1, input.length() -2));
			System.out.print("true");
			return true;
			
		}
		else
		{
			System.out.print("false");
			return false;
		}
	}
	
}
