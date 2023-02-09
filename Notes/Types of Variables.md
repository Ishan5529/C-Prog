**Types of Variables:**
1) Auto or local
2) External or global
3) Static (Local or Global)
4) Register (Local or global)


Specified on basis of:  
-> Visibility  
-> Lifetime  
-> Accessibility

**Local Variables**

    Visible/Accessible only inside the function.
    Lifetime = Till the execution of function.

**Global Variables**

    Visible/Accessible everywhere within the file, where it is defined.
    Lifetime = Till the execution of that file
    To access the variables from another file, we use keyword extern.
    Ex: int a is defined in a file to access it in another file, we use extern int a;


**Register Variables**

    Keyword Register is used to define this type of variable.
    Syntax: register <datatype> <Variable_Name>;
    ex: register int a;
    Use: It assigns variables to registers part of ram, which is the fastest type of memory so, we use these types of variables, when we want faster processing.


**Static Variables**

    Syntax: static <datatype> <Variable_Name>;
    ex: static int a;
    Use: It keeps the value of a variable constant. Can be accessed within function only.
    
    Ex:
    while (condn)
    {
        static x=0;
        x+=10;
        printf("%d",x);
    }
    
    Here, the value of x becomes 10 then 20 then 30, it wont become 0 after each iteration.