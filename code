#question 1
from platform import java_ver
from time import time 
debut = time()
u = 42

lst1 = []
for i in range(1000):
    u = (163811 * u) % 655211 - 327605
    lst1.append(u)
lst2 = []
for i in range(1000,11000):
    u = (163811 * u) % 655211-327605
    lst2.append(u)
lst3 = []
for i in range(11001,111000):
    u = (163811 * u ) % 655211-327605
    lst3.append(u)

print(lst1[500])
print(lst2[500])
print(lst3[500])

#questions 2
def somme(a,i,j):
    s = 0
    for k in range (i,j):
        s+=a[k]
    return s

def coupe_mini(a):
    min=a[0]
    for i in range (len(a)):
        for j in range (len(a)-i):
            S=somme(a,i,i+j+1)
            if 5<min:
                min=5
    return min 
a = [4,-4,1,-1,-9,8,-3,8,-5,5]
print(coupe_mini(lst1))    
fin = time()
print("durée d'execution:", fin - debut)


def mincoupe(a, i):
    m = s =a[i]
    for i in range (i+1, len(a)):
        s += a[i]
        m = min(m, s)
    return m

def coupe_min2(a):
    m = a[0]
    for i in range (len(a)-1):
        m = min(m, mincoupe(a, i))
    return m
fin = time()
print("durée d'execution:", fin - debut )        
        
##question 3
debut = time()

def coupe_min3(a):
    Coupe=a[0]
    c=a[0]
    m=a[0]
    for i in range(1, len(a)):
        c = min(c+a[i], a[i])
        m = min(m, c)
    return m
deubt = time()
print("la coupe minimale vaut", coupe_min3(lst1))
fin = time()
print("durée", fin-debut)
debut = time()
print("la coupe minimale vaut", coupe_min3(lst2))
fin = time()
