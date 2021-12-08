def Add ():
    print("Addition")
    n = float(input("Enter a number: "))
    t = 0
    ans = 0
    while n != 0:
        ans = ans + n
        t+=1
        n = float(input("Enter another number (0 to calculate): "))
    return [ans,t]
def Sub ():
    print("Substraction");
    n = float(input("Enter a number: "))
    t = 0
    sum = 0
    while n != 0:
        ans = ans - n
        t+=1
        n = float(input("Enter another number (0 to calculate): "))
    return [ans,t]
def Multiply ():
    print("Multiplication")
    n = float(input("Enter a number: "))
    t = 0
    ans = 1
    while n != 0:
        ans = ans * n
        t+=1
        n = float(input("Enter another number (0 to calculate): "))
    return [ans,t]
def Average():
    an = []
    an = addition()
    t = an[1]
    a = an[0]
    ans = a / t
    return [ans,t]
while True:
    list = []
    print("Python 7 Sem Assignment-1!")
    print(" Simple Calculator-->")
    print(" Enter 'a' for Addition")
    print(" Enter 's' for Substraction")
    print(" Enter 'm' for Multiplication")
    print(" Enter 'v' for Average")
    print(" Enter 'q' for Quit")
    c = input(" ")
    if c != 'q':
        if c == 'a':
            list = Add()
            print("Ans = ", list[0], " total inputs ",list[1])
        elif c == 's':
            list = Sub()
            print("Ans = ", list[0], " total inputs ",list[1])
        elif c == 'm':
            list = Multiply()
            print("Ans = ", list[0], " total inputs ",list[1])
        elif c == 'v':
            list = Average()
            print("Ans = ", list[0], " total inputs ",list[1])
        else:
            print ("Sorry, invalid character")
    else:
        break