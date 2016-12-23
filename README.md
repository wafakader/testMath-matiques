Exercice 1 : 

  Let I = {1, 2, . . . , 100}
  X and Y are chosen independently and uniformly
  For every element a of I, we have these possible options: 
    a∈X		a∈Y
    a∈X		a∉ Y              Each option have the probability p=1/4
    a∉ X		a∈Y
    a∉ X		a∉ Y

  To have X a subset of Y, 3 options have to be true for every element a of I 
    a∈X		a∈Y
    a∉ X		a∈Y
    a∉ X		a∉ Y
    
  So the probability P=3/4 for each element of I
  
  For the whole set (I), the probability is equal to P=〖(3/4)〗^100

Exercice 2 :  

  n ∈ N, F(n)=2F(√n)+1
  Let the function g(n)=F(n)+1 so we have g(n)-1=2g(√n)-2+1
  Then we have g(n)=2g(√(n))
  This function g is satisfied by the function ln 
    So g(n)=ln⁡(n) which leads to F(n)=ln⁡(n)-1


Exercice 3 :  
1/	If n_1=0 then we have f(n_1,0,0,1)=1
    If n_1=1 then : 
    {x1=0,x2=1,x3=0,x4=1}, {x1=0,x2=0,x3=1,x4=1}, {x1=0,x2=0,x3=0,x4=2} so f(n_1,0,0,1)=2
    If n_1=2 then : 
    {x1=1,x2=1,x3=0,x4=1}, {x1=1,x2=0,x3=1,x4=1}, {x1=1,x2=0,x3=0,x4=2} , {x1=0,x2=2,x3=0,x4=1}, {x1=0,x2=1,x3=1,x4=1},        {x1=0,x2=1,x3=0,x4=2}, {x1=0,x2=0,x3=2,x4=2}, {x1=0,x2=0,x3=1,x4=3}, {x1=0,x2=0,x3=0,x4=4}  so f(n_1,0,0,1)=4

  After too many tries, we find out that  f(n_1,0,0,1)=2f(n_1-1,0,0,1)


2/	After doing too many tries with changing the parameters of the function Fun, we can see that it always returns a value.
In fact, the program runs until all the values (x1, x2 and x3) become equal to 0 so that it returns the value of x4. 
The point is if x3>0 then it will run and decrement x3 until it becomes 0, then it comes the turn of x2 to become (x2-1). Even when x3 will be x3+x4, the process will be the same until x3 and x2 become 0.
In that moment x1 will be the one decrementing. This process will be repeating until x1 becomes 0 and (x2, x3) equals (0, 0) then the program will return the value of x4. In other words the loop will never run forever.
