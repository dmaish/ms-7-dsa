```java
package toyproblem1;
import java.util.Arrays;
public class minmax {
public static void main(String [] args){
	int[]arraymain={2,43,46,75,3};
	Arrays.sort(arraymain);
	int min=arraymain[0];
	int max=arraymain[arraymain.length-1];
	
	int[] minA=new int[1];
	int[] maxA=new int[1];
	
	for(int i=0;i<arraymain.length;i++){
		if(arraymain[i]<=max){
			maxA[0]=arraymain[i];
		}
		if(arraymain[i]<=min){
			minA[0]=arraymain[i];
		}
	}
	System.out.println(Arrays.toString(arraymain));
	System.out.println("maximum integer si"+Arrays.toString(maxA));
	System.out.println("minimum integer si"+Arrays.toString(minA));
	
}
}
