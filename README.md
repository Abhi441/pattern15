# pattern15
coding block







import java.util.Scanner;
public class Main{
  public static void main(String[] args){
    Scanner sc = new Scanner(System.in);
    int n = sc.nextInt();
    int nr = 2*n -1;
    int nsp = 0;
    int nst = n;
    // row
    int row = 1;
    while(row <= nr){
      // work space 
		int csp = 1;
		while (csp <= nsp) {
			System.out.print(" ");
			csp++;
		}
			
			//work stars
			int cst = 1;
			while(cst <= nst) {
				System.out.print("*");
			
				cst++;
				
			}
				
			// prep
			System.out.println();
			if(row <= nr/2){
			  nst = nst +1;
			  nsp = nsp + 2;
			}
			else{
			  nst = nst - 1;
			  nsp = nsp -2;
			}
			row = row + 1;
			
        
    }
  }
}
