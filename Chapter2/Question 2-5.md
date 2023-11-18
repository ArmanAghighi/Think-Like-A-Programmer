2.5:
For this challenge I did not write any code but only think about the way the formulla works.
Let's say user input a number(an int number) and we must find out if it is valid or not and we call it mainNumber.
First of all we need a loop to preview the number and do some calculation on each number from the rightmost.
```
for(int i = 0 ; i < mainNumber.Length ; i ++)
``` 
first of all we must find out which number is on odd position so we use 
```
if(i % 2 != 0) continue;
```
we must add that number to our lastNumber(which must show the resault)
so
```
lastNumber += lastNumber + (pow(10 , i));`
```
after making sure that the position is odd we must multiply founded digit by 2 and find if the resault is more than 10 or not so we must findout that the digit itself is more than five or not
```
if(lastNumber[i] < 5) += lastNumber + (pow(10 , i));
````
and if it is more than five it we must callculate the remin value of the devided by ten
```
if(lastNumber[i] < 5) => 1 + (lastNumber[i] % 10)
```
then we must add it to the mainNumber
at the end we must see how much it needs to become valid