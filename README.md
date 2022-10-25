# Matris-Transpozunu-Bulma
---
Bu bir [patika.dev](www.patika.dev) projesidir.
```
import java.util.Arrays;
public class MatrisTranspozu {

    // This function stores transpose
    // of A[][] in B[][]
    static void transpose(int A[][], int B[][])
    {
        int i, j;
        for (i = 0; i < A[0].length; i++)
            for (j = 0; j < A.length; j++)
                B[i][j] = A[j][i];
    }

    // Driver code
    public static void main(String[] args)
    {
        int A[][] = { { 1,2,3},
                    { 4,5,6 }};

        int B[][] = new int[A[0].length][A.length], i, j;

        // Function call
        transpose(A, B);
        System.out.print("A Matris is \n");
        for (i = 0; i < A.length; i++) {
            for (j = 0; j < A[0].length; j++)
                System.out.print(A[i][j] + " ");
            System.out.print("\n");
        }

        System.out.print("Transpose A is \n");
        for (i = 0; i < A[0].length; i++) {
            for (j = 0; j < A.length; j++)
                System.out.print(B[i][j] + " ");
            System.out.print("\n");
        }
    }
}
```
