# My solution

```
int n = scn.nextInt();
		int k = scn.nextInt();
		int count = 0;
		int temp = n;
		while(temp!=0) {
			temp/=10;
			count++;
		}
		
		//logic for: if k > no. of digits
		k = k%count;
		//logic for: if k is negative
		if(k<0) {
			k = k + count;
		}
		
		
		int div = (int)Math.pow(10, k);
		int mul = (int)Math.pow(10, count-k);

		int rem = n % div;
		int quo = n / div;

		
		int rotate = (rem * mul) + quo;
		System.out.println(rotate);
```

# Sir Solution

```
int n = scn.nextInt();
		int k = scn.nextInt();
		
		
		int nod = 0;
		int temp = n;
		while(temp!=0) {
			temp/=10;
			nod++;
		}
		
		// if k is greater than nod
		k =  k % nod;
		
		// if k is negative
		if(k < 0) {
			k = k + nod;
		}
		
		int div = 1;
		int mul = 1;
		for(int i=1;i<=nod;i++) {
			if(i<=k) {
				div = div *10;
			}
			else {
				mul = mul*10;
			}
		}
		
		int rem = n%div;
		int quo = n/div;
		
		int r = rem * mul + quo;
		System.out.println(r);
```
