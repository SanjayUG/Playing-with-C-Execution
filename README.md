
# Before C execution 

## Steps:

### 1. Preprocessing
File Inclusion: The preprocessor includes the content of header files (like stdio.h) into the source code.
Macro Expansion: If there are any macros, they are expanded.

### 2. Compilation
Syntax Checking: Ensures that the code follows the C language syntax rules.
Generation of Assembly Code: The compiler generates assembly code, which is a low-level representation of the program.

### 3. Assembly
The assembler converts the assembly code into object code, which is a binary format understood by the machine but still not executable. 

### 4. Linking
Static Libraries: The linker adds the actual code from these libraries into the executable.
Dynamic Libraries: The linker adds references to these libraries, which are loaded when the program is executed.

### 5. Execution
Oerating system will load it into memory and processor executes it.

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