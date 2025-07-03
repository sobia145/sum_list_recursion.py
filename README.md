def sums(*args):
    if not args:
        return 0
    else:
        return args[0]+sums(*args[1:])
a=input("ENTER NUMBERS TO ADD BY GIVING SPACE: ")
n=list(map(int,a.split()))
print("THE SUM: ",sums(*n))
