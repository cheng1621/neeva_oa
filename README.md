# neeva_oa
# how to run my code.
**g++ -std=c++11 -g search.cpp -o a.out** and **./a.out**.
if you want to change the file name, go to **main** function and change it.

### test cases.
1. "up & neeVA";
2. "neeva & !very";
3. "this & neeVa ";
4. "this & neeva & !time";

# Introduction.
## problem 1: searching faster on a large set of tweets.
Implemented a **TrieTree** to store all the data. like
```
            root
           /     \
          n .     h:[timestamp]
         /         \
        e ..       i:[timestamp]
       /             \
      e...            s:[timestamp]
     /
    v...
   /
  a[timestamp].
        
```
timestamp is a tuple meaning that the word **neeva** appears in timestamp.
time complexity: O(n).


## problem 2 & problem 3. 
Implemented a parser.

# some ideas.
## starter codes.
if the query consists of m words. and there are n lines of data in .csv file. Suppose there are k words in tweet in average.
time complexity: O(m * n * k) , space complexity: O(1);; 

## new ideas
if I have all the data in the main memory and use **TrieTree** as the basic structure. we can easily get the timestamp. we can optimize it to  
```
if I ignore the preprocessing phase.(time needs to construct TrieTree.)
time complexity: O(m) , space complexity :O(n);  
```





