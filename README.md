# BinarySearch
```
public class Test {
    public static int binarySearch(int num, int[] A) {
        int leftA = 0, rightA = A.length -1;
        while (leftA <= rightA) {
            int midA = (leftA + rightA) / 2;
            if (num == A[midA])
                return (1);
            else if (num > A[midA])
                leftA = midA + 1;
            else rightA = midA - 1;
        }
        return (-1);

    }

    public static void main(String[] args) {
        int[] A = {0,2,8,10,99};
        int indexB = 5;
        System.out.println(binarySearch(indexB,A));


    }
}
```
