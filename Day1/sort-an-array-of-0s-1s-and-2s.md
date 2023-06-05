## [Sort an array of 0s, 1s and 2s](https://practice.geeksforgeeks.org/problems/sort-an-array-of-0s-1s-and-2s4231/1)

```cpp
class Solution
{
    public:
    void sort012(int a[], int n)
    {
        int low = 0, mid = 0, high = n-1,temp;
        while(mid<=high)
        {
            switch (a[mid])
            {
                case 0:
                temp = a[low];
                a[low] = a[mid];
                a[mid] = temp;
                low++;
                mid++;
                break;
                
                case 1:
                mid++;
                break;
                
                case 2:
                temp = a[high];
                a[high] = a[mid];
                a[mid] = temp;
                high--;
                break;
            }
        }
    }
    
};
```



### DUTCH NATIONAL FLAG PROBLEM
WE USE THREE POINTERS HERE
- low
- high
- mid\
The assumption behind this algorithm is\
elements behind low pointer are 0's\
elements after high pointer are 2's\
elements between low and mid-1 are 1's
