# Python
Python programmes
import math
from math import sqrt
def get_sides():
    a=int(input('Enter integer for side a: '))
    b=int(input('Enter integer for side b: '))
    c=int(input('Enter integer for side c: '))
    return a,b,c
def determinant(a,b,c):
    deter=(pow(b,2)-4*a*c)
    if deter >0:
        root1=(-b+(sqrt(deter)))/(2*a)
        root2=(-b-(sqrt(deter)))/(2*a)
        print('root1 =',root1)
        print('root2 =',root2)
        return root1, root2
    elif deter==0:
        root1=-b/(2*a)
        root2=root1
        print('root1 =',root1)
        print('root2 =',root2)
        return root1,root2
    else:
        print('No real roots ')
a,b,c=get_sides()
print('******************************')
print('a =',a)
print('b =',b)
print('c =',c)
an=determinant(a,b,c)
