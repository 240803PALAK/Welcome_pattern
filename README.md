# Welcome_pattern
Hacker Rank problem



    import math
    def pattern(n,m):
        col1=m
        row=m
        num = 0
        n=int(n)
        m=int(m)
        pattern1="-"
        pattern2=".|."
        numoftimespattern=1
        col=int(n/2)
        for i in range(col):
            for j in range(m):
                nooftimespattern1 = m - 3
                mid=int(nooftimespattern1/2)
                for k in range(1,mid+1):
                    if k<=mid:
                        print(pattern1,end="")
                for l in range(numoftimespattern):
                    print(pattern2,end="")
                numoftimespattern=numoftimespattern+2
                for n in range(mid,mid*2):
                    if k<=mid:
                        print(pattern1,end="")
                print("\n")
                m-=6
                break
        mid2=int((row-7)/2)
        for j in range(0,mid2):
            print(pattern1,end="")
        print("WELCOME",end="")
        for j in range(mid2,row-7):
            print(pattern1, end="")
        print("\n")
        num1=col
        for i in range(col):
            for j in range(col1):
                num=0
                for k in range(num1):
                    if k==0:
                        num+=1
                    else:
                        num+=2
                nooftimerpatern1inreverse=int((col1-(num*3))/2)
                for l in range(nooftimerpatern1inreverse):
                    print(pattern1,end="")
                for m in range(num):
                    print(pattern2,end="")
                for l in range(nooftimerpatern1inreverse):
                    print(pattern1,end="")
                print("\n")
                num1-=1
                break
    
    
    
    pattern(11,33)

