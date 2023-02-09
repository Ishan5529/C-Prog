**Dynamic Memory Allocation**

 Ex: 
 ```C
 int *x;  
 x=(int*) malloc(5*sizeof(int));
 ```
 here, we allocated space for 5 integers  
 now, assigning the space.
```C
 x=(int*) mallx(5*sizeof(int));
```
 This is for 1D Array... for 2D Array, we use 2D Pointer..

 Ex:
 ```C  
 int **p;  
 p=(int**) malloc(sizeof(int));  
 for (i=0;i<m;i++)   
    p[i]=(int*)malloc(sizeof(int));
```

**Multiple Dynamic Memory Allocation**

   here, we use calloc()  
   syntax: <variable>=(call type*) calloc(n,<block_size>)  
   ex: ptr=(int*) calloc(5,sizeof(int));  
  
**Reallocating Memory**

   we use realloc() for this.  
   syntax: <variable>=(call type*) realloc(<variable>,<block_size>);  
   ex: ```ptr = (int*) realloc(ptr, *sizeof(int));```

**NOTE**
   
   1. To free up memory allocation, we use free()  
   syntax: ```free(<Variable_name>);```  
   ex: ```free(ptr);```  
   this frees up the memory space used by the variable ptr.

   2. A pointer, which is defined within a function and now, we leave the function now, that pointer is called dangling pointer.

   3. valgrind --> This is a tool which helps determining memory access and memory leakage of the application.

   4. gprof() --> GNU Profiler --> This is a tool which gives the time taken by each segment to run.

   5. gcov() --> This tool checks how much portion of the testcases are being covered by the program.