# Set-Mismatch
from collections import Counter
nums=list(map(int,input("Enter the numbers:").split()))
n=len(nums)
count=Counter(nums)
r=[]
for i,c in count.items():
    if c==2:
        r.append(i)
for i in range(1,n+1):
    if i not in count:
        r.append(i)
print("Output:",r)
