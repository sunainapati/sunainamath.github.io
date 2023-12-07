[[0. Class 9 -11]]
[[Foldr, Foldr1, Foldl and Fold']]
### Anonymous functions

naming is hard. So we use `\` .

``length = foldr (\ x n -> n+1) 0


```haskell
length [4,5,6] 
= foldr (\ x n -> n+1) 0 [4,5,6] 
= (\ x n -> n+1) 4 (foldr \ x n -> n+1 0 [5,6])
= (\ x n -> n+1) 4 ( (\ x n -> n+1) 5(foldr \ x n -> n+1 0 [6]) )
= (\ x n -> n+1) 4 ( (\ x n -> n+1) 5  ((\ x n -> n+1) 6 (foldr \ x n -> n+1 0 [])))
= (\ x n -> n+1) 4 ( (\ x n -> n+1) 5  ((\ x n -> n+1) 6 0))
=  (\ x n -> n+1) 4 ( (\ x n -> n+1) 5 1)
=   (\ x n -> n+1) 4  2
= 3
```
