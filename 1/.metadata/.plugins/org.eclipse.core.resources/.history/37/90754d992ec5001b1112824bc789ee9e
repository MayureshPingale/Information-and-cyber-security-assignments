import java.util.*;

public class DiffieHellman {
	
	private static long power(long a, long b, long p)
	{
	    if (b == 1)
	        return a;
	    else
	        return (((long)Math.pow(a, b)) % p);
	}
	 
	public static void main(String[] args)
	{
		Scanner sc = new Scanner(System.in);
		
	    long P, G, x, a, y, b, ka, kb;
	     
	    P = 23;
	    System.out.println("The value of P:" + P);
	     
	    G = 9;
	    System.out.println("The value of G:" + G);
	     
	    // Alice will choose the private key a
	    System.out.println("Enter Private Key for Alice (A < P)");
	    a = sc.nextLong();
	    
	    // Bob will choose the private key b
	    System.out.println("Enter Private Key for Bob (B < P)");
	    b = sc.nextLong();
	    
	    System.out.println("The private key a for Alice:" + a);
	    System.out.println("The private key b for Bob:" + b);
	    
	    x = power(G, a, P);    
	    y = power(G, b, P);
	     
	    // Generating the secret key after the exchange of keys
	    ka = power(y, a, P);
	    kb = power(x, b, P);
	     
	    System.out.println("Secret key for the Alice is:" + ka);
	    System.out.println("Secret key for the Bob is:" + kb);
	    
	    sc.close();
	}

}
