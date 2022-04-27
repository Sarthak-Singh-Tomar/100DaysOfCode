# Day2:

## Analysis of Algorithm
1. Asymptotic Analysis: What we do in asymptotic analysis is measuring the order of growth of a program or algorithm in terms of input size.
2. When we do analysis of algorithms we always talk about sizes of input which are larger than or equal to zero, Because your input size can never be zero.
3. The time taken by functions should also be greater than zero because our algorithm or program can never take negative time.
4. Scenario: Jab me aur mera friend apna-apna program run karte hain own machine par to kis ka program fast hoga? mera friend ek fast machine par apna progam run kar raha hain and me ek slow machine par, so low inputs par mere friend ka program fast run karega but we will see that after at certain value of n input our program will run fast as compare to our friends program.

## Types of Graph
1. y = mx + c - straight line
2. y^2 = 4ax - Horizontal parabola
3. x^2 = 4ay - Vertical parabola
4. xy = c - hyperbola

## Order of Growth
1. The basic idea of Analysis of algorithm is to order of growth of time taken by the algorithm.
2. The limit is always tends to infinity, we always talk about large size of input theoretical analysis.
3. Order of Growth: Order of Growth is the main criteria when we do theoretical analysis of algorithms - If order of growth of the function which represent time taken by the algorithm is more compared to another algorithm then we say that this algorithm is bad algorithm.
4. A function f(n) is said to be growing faster than g(n) if:
  lim n->infinity f(n)/g(n) = infinity
  OR
  lim n->infinity g(n)/f(n) = 0
5. Direct way to find the order of growth:
      (a). Ignore lower order terms
      (b). Ignore leading constant
6. How do we know which terms are lower order?
![image](https://user-images.githubusercontent.com/86265843/165503325-0beca664-8dc0-4f59-a99b-016c704a5f08.png)

## Best, Average and Worst cases & Asymptotic Notation
1. In general, when we analyse algorithms, we do not care about best case its considered as bogus.
2. Average case, we would like to know how much average time a software is taking, but it is impractical to do.
3. Worst case is something we do most of the time - we try to find out what is the case for which our algorithm is going to take maximum time.
4. Below three are the most used mathematical notations used to represent order of growth and this function represent the time taken by the algo.
![image](https://user-images.githubusercontent.com/86265843/165509570-01a1ce89-584c-4a17-993e-828830b84e92.png)

## Analysis of Common loops
```
for(int i=0;i<n;i=i+c) {
  //some O(1) work
}
```
Order of Growth: n/c =  O(n)
```
for(int i=n;i>0;i=i-c) {
  //some O(1) work
}
```
Order of Growth: n/c = O(n)
```
for(int i=1;i<n;i=i*c) {
  //some O(1) work
}
```
Order of Growth: logn+1 = O(logn)
Note: Base of log does not matter.
```
for(int i=n;i>1;i=i/c) {
  //some O(1) work
}
```
Order of Growth: O(logn)
```
for(int i=2;i<n;i=pow(i,c)) {
  //some O(1) work
}
```
Order of Growth: lognlogn+1 = O(lognlogn)
```
void fun(int n) {
  for(int i= 0;i<n;i++) {
    //some O(1) work
  }
  for(int i=1;i<n;i=i*2) {
    //some O(1) work
  }
  for(int i=1;i<100;i++) {
    //some O(1) work
  }
}
```
work: O(n) + O(logn) + O(1) = O(n)
```
void fun(int n) {
  for(int i=0;i<n;i++) {
    for(int j=1;j<n;j=j*2) {
      //some O(1) work
    }
  }
}
```
work: O(n) * O(logn) = O(nlogn)
```
void fun(int n) {
  for(int i=0;i<n;i++) {
    for(int j=1;j<n;j=j*2) {
      //some O(1) work
    }
  }
  for(int i=0;i<n;i++) {
    for(int j=1;j<n;j++) {
      //some O(1) work
    }
  }
}
```
work: O(nlogn) + O(n^2) = O(n^2)
