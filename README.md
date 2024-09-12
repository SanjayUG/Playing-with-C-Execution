
# Before C execution 

## Steps:

1. Preprocessing
2. Compilation
3. Assembly
4. Linking
5. Execution


## 1. Command for Preprocessing

``` gcc -E addition_of_two_nums.c -o addition_of_two_nums.i ```

## 2. Command for Compilation

``` gcc -S addition_of_two_nums.i -o addition_of_two_nums.s  ```

## 3. Assembly

``` gcc -c addition_of_two_nums.s -o addition_of_two_nums.o  ```

## 4. Linking

``` gcc addition_of_two_nums.o -o addition_of_two_nums  ```

## 5. Execution

``` ./addition_of_two_nums  ```