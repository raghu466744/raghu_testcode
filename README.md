# raghu_testcode
raghu_testcode_rep
n = int(input("enter the number :"))
num = [1,3,12,60]
result=[]
dif=n

def callfun(n,cnt) :
  
  for i in num:
    
    if i==n:
      result.append(chr(65+cnt))
      break
    elif n<i:
      print(n)
      n=n-num[cnt-1]
      print(n)
      result.append(chr(65+int(cnt-1)))
      print(result)
      return n
    cnt=cnt+1 
  
while True:
    cnt=0
    callfun(n,cnt)
    
    print(n)
    if (n == 0) :
      break
