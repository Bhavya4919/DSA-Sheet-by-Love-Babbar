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
- TC: O(nlogn)\
- SC: O(1)
