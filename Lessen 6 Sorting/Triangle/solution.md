
![image](https://i.imgur.com/Hyi7SKR.jpg)


  def solution(A):
    
    A.sort()
    for i in range(len(A)):
        if i+2<len(A):
            if A[i]+A[i+1]>A[i+2]:
                return 1
    return 0
    pass
