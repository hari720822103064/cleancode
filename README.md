Fibonacci series

public class FibonacciNumbers {
    public static void main(String[] args) {
        int elementPosition = 1, count = 10, firstFibonacciNum = 0, nextFibonacciNum = 1;
        System.out.print(firstFibonacciNum + " " + nextFibonacciNum);
        for (elementPosition = 2; elementPosition < count; ++elementPosition) {
            int sumOfPrev2 = firstFibonacciNum + nextFibonacciNum;
            firstFibonacciNum = nextFibonacciNum;
            System.out.print(" " + sumOfPrev2);
            nextFibonacciNum = sumOfPrev2;
        }
    }
}

output:0 11 23 5 8 13 21 34
