3.3:
To find if an array is sorted or not we must first get the array from the user and store it in a variable and name it myArray for example
after that we asked to check it in a bool method so we create a method that has two arguman in it as Array and Size
```
public bool IsSorted(Array,Size)
```
first of all if size if  less than one it is sorted by default
and it returns true after that we need a for loop and compair element i and i-1 and
```
if(Array[i] > Array[i-1])
```
it returns false and if this condition is not stablished by the end of loop the Array is sorted
this is the input
```
Array =>{5,12,85,4,23,9,0,360}
size => Array.Length
```
this is the Code
```
public bool IsSorted(Array,Size)
{
    if(size < 1)
        return true
    for(i = 1 ; i <= size ; i++)
        if(Array[i] > Array [i - 1])
            return false;
    return true;
}
```