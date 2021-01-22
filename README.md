# porzadkowanie-przez-wstawianie
def insertationSort(T):
  n=len(T)
  for i in range(1,n):
    pom=T[i]
    k=i-1
    while k>=0 and T[k]>pom:
      T[k+1]=T[k]
      k=k-1
    T[k+1]=pom
    i=i+1
  return T


from random import randint 
T=[randint(1,100) for x in range(10)]
print(insertationSort(T))
