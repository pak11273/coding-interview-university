## Arrays Big O
	* adding an element or subtracting, from the end => O(1)
	* adding an element or subtracting, from the beginning => O(n)
	* adding an element or subtracting, from the middle => O(n)
      * Read or write to an array => O(1)  
      * linear time === O(n) ??
## Exercises
  * execute this function on paper
  ```js
public static void printPrimes(int n) {
    boolean[] prime = new boolean[n + 1];
    int i;
    for(i = 2; i <= n; i++) {
      prime[i] = true;  	
    }
    for(int divisor = 2; divisor * divisor <= n; divisor++) {   // divisor <= sq.rt(n) 
      if(prime[divisor]) {
        for(i = 2 * divisor; i <= n; i= i+ divisor) {
          prime[i] = false;
        }
      }
    }
    for(i=2; i <= n; i++) {
      if(prime[i]) {
        System.out.print(" " + i);
      }
    }  
}  
```
  

  * Implement an array in JS
  * Implement an array in Java
