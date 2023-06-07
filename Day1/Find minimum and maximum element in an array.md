## [Find minimum and maximum element in an array](https://practice.geeksforgeeks.org/problems/find-minimum-and-maximum-element-in-an-array4428/1)
``` cpp
pair<long long, long long> getMinMax(long long a[], int n) {
    
    pair<long long, long long> minmax;
    sort(a, a+n);
    minmax.first = a[0];
    minmax.second = a[n-1];
    return minmax;
    
}
```
- TC: O(nlogn)
- SC: O(1)

Optimized code

``` cpp
#include <bits/stdc++.h> 
int sumOfMaxMin(int arr[], int n){
	int small = arr[0];
	int large = arr[0];
	for(int i=1;i<n;i++)
	{
		if(arr[i]>large)
		large = arr[i];
		if(arr[i]<small)
		small = arr[i];
	}
	return large+small;
}
```
TC: O(N)
