# Hello-World :joy:
Just getting started

## Ingredients
1. Test
2. Ideas
3. Collaboration
4. Daily Coding Problems

> am a messy writer, will continue to build and learn as i go

## DailyCoding Problems
1. Given an array of integers, return a new array such that each element at index i of the new array is the product of all the numbers in the original array except the one at i.

For example, if our input was [1, 2, 3, 4, 5], the expected output would be [120, 60, 40, 30, 24]. If our input was [3, 2, 1], the expected output would be [2, 3, 6].

>This problem was asked by Uber.

- [ ] Follow-up: what if you can't use division?
- [ ] testcases
### 1.
```
ar=[int(item) for item in input("Enter array: ").split()]
ans=[]
print(ar)
pr=1
for i in ar:
    pr=pr*i
for i in ar:
    ans.append(pr//i)
print(ans)  #fast process, doesn't work with "0"
```
### 2.
```
ar=[int(item) for item in input("Enter array: ").split()]
ans=[]
print(ar)
for i in range(len(ar)):
    product=1
    for j in range(len(ar)):
        if(i==j):
            continue
        else:
            product=product*ar[j]
    ans.insert(i,product)
print(ans)     # Brute-force method, slow process
```
