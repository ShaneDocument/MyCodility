
![image](https://i.imgur.com/Hyi7SKR.jpg)

  # you can write to stdout for debugging purposes, e.g.
  # print("this is a debug message")

def solution(A):
    
    A.sort()
    for i in range(len(A)):
        if i+2<len(A):
            if A[i]+A[i+1]>A[i+2]:
                return 1
    return 0
    # write your code in Python 3.6
    pass
