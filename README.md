# Task3_report
github pages
Name: Ereny Eleya
BN: 18
SEC: 1
1) ‘const’ keyword stands for constant. In C++ it is used to make some values constant throughout the program. If we make an artifact of a C++ program as constant then its value cannot be changed during the program execution.


   a)Constant Variables:
     While declaring a variable as const it must be initialized as well. Once declared as const then we cannot change its value later on as shown in the example below.
     ![Image1](https://imgur.com/a/NqxzXKm)
     We can see that a variable ‘a’ is declared as const at line 7. It is initialized as well with a value 1.23 at the same time. If we try to change its value later on (as at line 8), then C++ compiler will raise an error as below.

     error C3892: ‘a’ : you cannot assign to a variable that is const





   b)Constant Pointers

     Just like constant variable, the value of constant pointer is initialized at the time of declaration and once declared then we can change the pointer variable. We can also say that if we want that a pointer variable must always point to the same variable then we can make it constant as shown in the example given below.
     ![Image2](https://imgur.com/WSAffhK)
      We can see that a constant pointer variable ‘p’ is declared at line 8 that points to variable x. As the pointer variable ‘p’ is declared as const so it will always point to variable x. At line 12, we tried to change the value of pointer variable ‘p’ which will lead to a compilation error as below. If the pointer variable was not declared as const then the same code will execute without any error as one pointer variable can point to more than variables at different times.
      error C3892: ‘p’ : you cannot assign to a variable that is const.





   c)Pointer to Constant Variables

     A pointer to const means that we can access the value of the variable through pointer variable but cannot change the value of the pointed variable through the pointer variable as explained in the following example.
     ![image3](https://imgur.com/e6wF6db)
     The pointer to constant variable is declared at line 8. It is important to note that the variable to what the pointer is pointing to is not constant itself which means that its value can be changed itself (line 11) but cannot be changed through the pointer variable (line 12). If we try to change its value through the pointer variable as at line 12, then it will generate a compilation error as below.

     error C2297: ‘*’ : illegal, right operand has type ‘const int *’




   d)Constant Function Arguments

     We can use the const keyword with the arguments of a function. If an argument is declared as const then the function will not be allowed to change its value. The same is explained in the following code.
     ![image4](https://imgur.com/D1M0ZD9)
     At line 5, a constant argument ‘a’ is declared which cannot be changed in the function. If tried (as at line 7) then an error will be raised by compiler as given below.

     error C3892: ‘a’ : you cannot assign to a variable that is const





   e)Constant Data Members of a Class

     The keyword ‘const’ can also be used with the data members of a class. If we define a const data member of a class then we must have to initialize that data member through the constructor of the class. The value of const data members cannot be changed through the object of the variable as shown in the code below.
     ![image5](https://imgur.com/KxE8nq5)
     In the above code a const data member of a class is declared at line 8 and initialized by the constructor at line 9. This data member can be accessed by the object of the class but cannot be modified. For example at line 15, the value of the const data member is accessed by the object of the class but when tried to change the value of const data member at line 16 then the compiler will not allow it and generates an error.
   
2)"&" operator:
     a)The ampersand symbol & is used in C++ as a reference declarator in addition to being the address operator. The meanings are related but not identical.

     int target;
     int &rTarg = target;  // rTarg is a reference to an integer.
                        // The reference is initialized to refer to target.
         void f(int*& p);      // p is a reference to a pointer


     If you take the address of a reference, it returns the address of its target. Using the previous declarations, &rTarg is the same memory address as &target.
     You may take the address of a register variable.
     You can use the & operator with overloaded functions only in an initialization or assignment where the left side uniquely determines which version of the overloaded function is used.


     

     b)The & (address) operator yields a pointer to its operand. The operand must be an lvalue, a function designator, or a qualified name. It cannot be a bit field, nor can it have the storage class register.
     If the operand is an lvalue or function, the resulting type is a pointer to the expression type. For example, if the expression has type int, the result is a pointer to an object having type int.
     If the operand is a qualified name and the member is not static, the result is a pointer to a member of class and has the same type as the member. The result is not an lvalue.
     If p_to_y is defined as a pointer to an int and y as an int, the following expression assigns the address of the variable y to the pointer p_to_y :
     EX:     p_to_y = &y;


     c) && operator:
     Logical AND.
     True only if all the operands are true.


     Link of Github pages: https://erenyeleya.github.io/Task3_report/





