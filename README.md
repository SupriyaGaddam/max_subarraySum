# max_subarraySum
def maxsubarraySum(a):
    total=a[0]
    curr=a[0]
    for i in range(1,len(a)):
        curr=max(a[i]+curr,a[i])
        total=max(total,curr)
    return total
mylist=[-2,-3,4,-1,-2,1,5,-3]
print(maxsubarraySum(mylist))
