# WavePrint
import java.util.ArrayList;
public class Solution {
	public static int[] wavePrint(int a[][], int m, int n) {
		// Write your code here.
    int b[]=new int[m*n];
        int k=0;
        for(int j=0;j<n;j++){
            
if(j%2==0){
   for(int i=0;i<m;i++){
b[k++]=a[i][j];
   }
}
else
{
     for(int i=m-1;i>=0;i--){
b[k++]=a[i][j];
   }
    
}
        }
        return b;
	}
}


