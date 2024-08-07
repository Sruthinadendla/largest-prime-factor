# largest-prime-factor
def largestPrimeFactor(n):
  factor=0
  d=2
  while d*d<=n:
    if(n%d)==0:
      factor=max(factor,d)
      n//=d
    d+=1 
  if n>1:
    factor=max(factor,n)
  return factor
n=int(input())
print(largestPrimeFactor(n))
