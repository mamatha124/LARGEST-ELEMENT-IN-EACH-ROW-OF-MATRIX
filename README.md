# LARGEST-ELEMENT-IN-EACH-ROW-OF-MATRIX
import java.util.*;
class Main {
    public static void main(String[] args) {
        int c=0;
        Scanner sc= new Scanner(System.in);
          System.out.println("Enter array length: ");
        int n=sc.nextInt();// Array length
         int [][]a=new int[n][n];
         int []b=new int[n];
         int l=0;
         System.out.println("Enter array elements: ");
        for(int i=0;i<n;i++){
            
            for(int j=0;j<n;j++){
            int k=sc.nextInt();
            a[i][j]=k;
            if (l<k)
                b[i]=k;
                l=k;
            }
        }
        System.out.println("largest element in each row elements: ");
        for (int i=0;i<n;i++){
             System.out.print(b[i]+" ");
        }
    }
}
