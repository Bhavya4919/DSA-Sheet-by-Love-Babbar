## [Reverse a String](https://practice.geeksforgeeks.org/problems/reverse-a-string/1)
``` java
class Reverse
{
    public static String reverseWord(String str)
    {
       int n = str.length();
       char[] s = str.toCharArray();
       int start = 0;
       int end = n-1;
       while(start<end)
       {
           char temp = s[start];
           s[start] = s[end];
           s[end] = temp;
           start++;
           end--;
       }
       String string = new String(s);
       return string;
    }
}
```
- Two pointer approch\
- Function to convert string to character Array => toCharArray()\
- Function to convert char array to String => String constructor
