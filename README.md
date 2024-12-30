# code-clash
def que(n,beginword):
 
 
 wordList={}
 wordList[1]=beginword
 
 lst=[]
 for word in beginword:
  lst.append(word)  #  lsit of characters
 for x in range(n):
  if x%2==0:
   lst.append('a')
   newwor=''.join(lst)
   wordList[x+2]=newwor
  elif x%2==1:
   p=beginword[1]
   lst.remove(p)
   newwor=''.join(lst)
   wordList[x+2]=newwor

 wordList[n+2]=endword
 return endword

n=int(input('Enter number of words in dictionary:'))
begword='hello'
que(n,begword)
