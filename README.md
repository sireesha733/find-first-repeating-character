# find-first-repeating-character
#problem-1
t=int(input())
for i in range(t):
  d={}
  s=input()
  for i in s:
    if i not in d:
      d[i]=1
    else:
      d[i]=d[i]+1
  for i in d:
    if d[i]>1:
      print(i)
      break
    else:
      print(".")
