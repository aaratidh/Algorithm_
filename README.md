# Algorithm_

This repo include my learning of algorithm. 

Day_1  # problem solving using Stack in

Problem: 
![image](https://user-images.githubusercontent.com/35992124/218293713-513ac47f-3b06-4964-8cfc-c5b6e30879c4.png)


l = [2,4,3,2,1,2,1,2,4]
ln =len(l)
height = []
length = []
stack = []
stack.append(l[0])
for  i in range(1,ln):
     if l[i-1]>l[i]:
          stack.append(l[i])
     else:
          st = stack.pop()
          while((l[st]<=l[i])):
               if(l[st]==l[i]):
                    stack.append(i)
                    height.append(l[i])
                    length.append(i-st-1)
                    stack.append(st)
                    stack.append(i)
                    if(len(stack)!=0):
                         st = stack.pop()

print(height,"height")
print(length,"length")





Day_2
