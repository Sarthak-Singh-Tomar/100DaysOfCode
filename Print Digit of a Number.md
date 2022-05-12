```
int n = scn.nextInt();
		
		int nod = 0;
		int temp = n;
		
		while(temp != 0) {
			temp/=10;
			nod++;
		}
		
		int div = (int)Math.pow(10, nod-1);
		while(div != 0) {
			int res = n/div;
			System.out.println(res);
			n %=div;
			div /= 10;
		}
```
