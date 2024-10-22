# Bioinformatics Quiz 1

## Question 1a:
### You are about to start a new project and are currently in your home directory. You want to create a new directory  called "Project1" and then move into that directory to ccntinue working. What two commands do you use to acheive this?
#### Answer 1a:
```
mkdir Project1
cd Project1
```
## Question 1b:
### You realize that you don't want Project1 to be in your home directory, so you want to navigate back to your home directory and then remove it. What commands do you use to acheive this?
#### Answer 1b:
```
cd ../
rm -r Project1
```

## Question 2a:

### You have a matrix with four rows (1-4) and one column (1), and are considering turning your matrix into a data frame if it will be easier to manipulate. You are considering how you will access your column in either case. You know that in both matrices and data frames you can use [,1] to access your first column. What is the difference in the result you will get between mymatrix[,1] and mydf[,1] ?

#### Answer 2a: mymatrix[,1] will return all of the values in the 1st column of the matrix, without the rows numbered 1-4. mydf[,1] will return all the values in the 1st column as a set of two columns, one being the corresponding numbered rows.

## Question 2b: 
### What is the difference between what mydf[1] and mydf[[1]] will return to you?

#### Answer 2b: mydf[1] will return the first column of the data frame alongside the columns corresponding numbered rows 1-4. mydf[[1]] will return the first column of the data frame and it will just be the values of that column, like in mymatrix[,1].


## Question 3:
### You want to share a directory named "genome" and a file named "genomereads" from your home directory "home" with a labmate without exposing your entire directory. How do you modify the file permissions using chmod (not using octal permissions)?
#### Answer 3:
```
chmod g+x home/genome
chmod g+rx home/genome/genomereads
```


