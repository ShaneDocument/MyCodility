

![image](https://i.imgur.com/fyJqbFg.jpg)

    
    def solution(S):
      stack = []
      for i in S:
          if i=='(' or i=='[' or i=='{':
              stack.append(i)
          else:
               if len(stack)==0 or (i==')' and stack.pop()!='(') or (i==']' and stack.pop()!='[') or (i=='}' and stack.pop()!='{') :
                    return 0
          if len(stack)==0:        
                return 1
      return 0
    # write your code in Python 3.6
      pass
