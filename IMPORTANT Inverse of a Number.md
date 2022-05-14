# My solution
```
int n = scn.nextInt();
int dig = 0; 
int count = 0;
int res = 0;		
while(n>0) {
	dig = n%10;
	count++;
	res = res + count *(int)Math.pow(10, dig-1);
	n/=10;
	}
System.out.println(res);
```

# Sir solution

```
int n = scn.nextInt();
int inverse = 0; 
int originalPlace = 1;		
while(n!=0) {
	int originalDigit = n%10;
	int inverseDigit = originalPlace;
	int inversePlace = originalDigit;			
	inverse = inverse + inverseDigit * (int)Math.pow(10, inversePlace-1);
	n/=10;
	originalPlace++;
}
System.out.println(inverse);
```
