import java.util.*;
import java.lang.*;
class Solution {
/**
·* @param String[] ops - List of operations
·* @return int - Sum of scores after performing all operatio
·*/
public static int calPoints(String[] ops) {
Stack<Integer> stack = new Stack();
for(String op : ops){
if (op.equals("+")){
int top = stack.pop();
int newtop = top + stack.peek();
stack.push(newtop);
stack.push(top);
}else if (op.equals("C")){
stack.pop();
}else if (op.equals("D")){
stack.push(2 * stack.peek());
}else {
stack.push(Integer.valueOf(op));
}
}
int result = 0;
for(int score : stack) result += score;
return result;
}
}


public class Main
{
public static void main(String args[])
{
Scanner sc = new Scanner(System.in);
String[] ops = sc.nextLine().split(" ");
System.out.println(Solution.calPoints(ops));
}
}
