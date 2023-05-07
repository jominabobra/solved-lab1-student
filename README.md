Download Link: https://assignmentchef.com/product/solved-lab1-student
<br>
5/5 - (1 vote)

 Using the provided java source code template lab1-student.java, complete the recursive method public static long recStirling(int m, int n) //assume m,n =1 to compute and return the value of S(m, n) using the recurrence given above.



The input to the method will be m and n which you can assume to be positive integers. Then complete the iterative method public static long iterStirling(int m, int n) //assume m,n =1 to compute and return the value S(m, n) for postive integer inputs m, n. This method must use a loops (instead of recursion) and a 2-dimensional array (to store the numbers as you compute them from S(1, 1) to S(m, n)).

The idea for the iterative method: using the recurrence relation, compute and put S(i, j) into position (i, j) of the array, for i from 1 to m and j from 1 to n. Use the base cases to initialize the array and be careful the order in which you compute array entries.

You need to ensure that if you are computing S(i, j) that S(i − 1, j − 1) and S(i − 1, j) have already be computed and stored in the array. Finally, use the main method provided that calls each of the above methods to find S(20, 12). The main method reports how much time each of the two methods takes to compute S(20, 12) and prints the answer computed by each. Ensure that the two answers are the same.

public class lab1 {

public static void main(String args[]) {long timestamp;

final int m = 20, n = 12;long result;long start, stop, elapsedTime;

start = System.nanoTime();result = recStirling(m,n);stop = System.nanoTime();elapsedTime = stop – start;System.out.println(“Elapsed time for recursive call:”+elapsedTime+” nanoseconds.”);System.out.println(“S(“+m+”,”+n+”)=”+result);

start = System.nanoTime();result = iterStirling(m,n);stop = System.nanoTime();elapsedTime = stop – start;System.out.println(“Elapsed time for iterative call:”+elapsedTime+” nanoseconds.”);System.out.println(“S(“+m+”,”+n+”)=”+result);

}

//recursive method for computing Stirling number S(m,n)public static long recStirling(int m, int n) { //assume that 1 &lt; n &lt;= m

}

//iterative method for computing Stirling number S(m,n)public static long iterStirling(int m, int n) { //assume that 1 &lt; n &lt;= m

}