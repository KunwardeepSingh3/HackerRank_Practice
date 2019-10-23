import java.io.*;
import java.math.*;
import java.security.*;
import java.text.*;
import java.util.*;
import java.util.concurrent.*;
import java.util.regex.*;

public class Solution {

    // Complete the miniMaxSum function below.
    static void miniMaxSum(int[] arr) {
        long minSum = 0, maxSum = 0;
        for (int i = 0; i<arr.length - 1; i++){
            for (int j = 0; j<arr.length-i-1; j++)
            if (arr[j] > arr[j+1]){
                swap(arr, j, j+1);
            }
        }
        for (int i = 0; i<arr.length-1; i++){
            minSum += arr[i];
            }
        for (int i = 1; i<arr.length; i++){
            maxSum += arr[i];
            }
        System.out.print(minSum + " " + maxSum);
    }

    private static void swap(int []ar, int a, int b){
        int temp = ar[a];
        ar[a] = ar[b];
        ar[b] = temp;
    }

    private static final Scanner scanner = new Scanner(System.in);

    public static void main(String[] args) {
        int[] arr = new int[5];

        String[] arrItems = scanner.nextLine().split(" ");
        scanner.skip("(\r\n|[\n\r\u2028\u2029\u0085])?");

        for (int i = 0; i < 5; i++) {
            int arrItem = Integer.parseInt(arrItems[i]);
            arr[i] = arrItem;
        }

        miniMaxSum(arr);

        scanner.close();
    }
}

