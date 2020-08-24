# largestNumInList
Finding the largest number in a list concept is rather simple - we temporarilly assume that the first element is the largest one, andcheck the hypotheses agains all the remaining element in the list. The range() function returns a sequence of numbers, starting from 0 by default, and increments by 1 (by default), and stops before a specified number. To save some computer power, you can use a slice. 

Test Data
=

[Code]()


```
myList = [30, 17, 3, 11, 5, 100, 1, 9, 7, 15, 13]
#The concept is rather simple - we temporarilly assume that the first element is the largest one, andcheck the hypotheses agains all the remaining element in the list
largest = myList[0]

#The range() function returns a sequence of numbers, starting from 0 by default, and increments by 1 (by default), and stops before a specified number.
for i in range(1, len(myList)):
    if myList[i] > largest:
        largest = myList[i]

print(largest)

#If you need to save some computer power, you can use a slice
myList = [30, 17, 3, 11, 5, 100, 1, 9, 7, 15, 13]
largest = myList[0]

for i in myList[1:]:
    if i > largest:
        largest = i

print(largest)
```

Expeted Output:
```
100
100
```
