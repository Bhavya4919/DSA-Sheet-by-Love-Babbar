## [Kth smallest element](https://practice.geeksforgeeks.org/problems/kth-smallest-element5635/1)
``` cpp
class Solution{
    public:
    // arr : given array
    // l : starting index of the array i.e 0
    // r : ending index of the array i.e size-1
    // k : find kth smallest element and return using this function
    int kthSmallest(int arr[], int l, int r, int k) {
        sort(arr, arr+r+1);
        return arr[k-1];
    }
};
```
## [Kth largest elements](https://practice.geeksforgeeks.org/problems/k-largest-elements4206/1)
``` cpp
class Solution{
public:	
	vector<int> kLargest(int arr[], int n, int k) {
	    sort(arr, arr+n);
	    vector<int> v;
	    for(int i=0;i<k;i++)
	    {
	        v.push_back(arr[n-1-i]);
	    }
	    return v;
	}

};
```
