dic={}
dic2={}
j=0
for i in 'abcdefghijklmnopqrstuvwxyz':
    j+=1
    dic[i]=j
    dic2[j]=[i]
j=0
for i in 'ABCDEFGHIJKLMNOPQRSTUVWXYZ':
    j+=1
    dic[i]=j
    dic2[j]+=[i]

def reclist(n):
    if n==1: return ([i for i in 'abcdefghijklmnopqrstuvwxyz']+[i for i in 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'])
    else:
        l1=reclist(n-1)
        l2=[]
        for i in l1:
            k=dic[i[0]]
            j=0
            while j<k:
                j+=1
                l2+=[dic2[j][0]+i,dic2[j][1]+i]
        return l2

def answer(n):
    l1=reclist(n)
    l2=[i[::-1] for i in l1]
    return l2
