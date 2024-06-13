# ant_moves_1_-1
There is a ant on your balcony.It wants to leave the rail so sometimes it moves right  and sometimes it moves left until it gets exhausted.Given an integer array A of size N  which consists of integer 1 and -1 only representing ant's moves.


moves=int(input("enter the number of moves"))
array=list(map(int,input("enter the array of -1 and 1").split()))
count=0
for i in range(len(array)):
    if sum(array[:i+1])==0:
        count=count+1
print(count)
