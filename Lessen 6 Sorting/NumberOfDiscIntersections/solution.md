
![image](https://i.imgur.com/Z0Zb7MB.jpg)


def solution(A):

    Range = []
    
    for i,radius in enumerate(A):
    
        Range.append((i,i-radius,i+radius))
    
    Range.sort(key = lambda s:s[1])
    #print(Range)
    count = 0
    for i in range(len(A)):
        for j in range(i+1,len(A)):
            if Range[j][1]<=Range[i][2]:
                count+=1
    
    if count>10000000:
        return -1
    else:
        return count
    # write your code in Python 3.6
    pass
