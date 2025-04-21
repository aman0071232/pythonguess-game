# pythonguess-game
import random
yourstr=input("Enter ur value from,s,w,g = " )
yourdict={"s":1,"w":-1,"g":0}
computer=random.choice([1,0,-1])
you=yourdict[yourstr]
if(computer==you):
    print("its a draw")
else:
    if(computer==-1 and you==0):
        print("you lose")
    elif(computer==-1 and you==1):
        print("you win")
    elif(computer==1 and you==0):
        print("you win")
    elif(computer==1 and you==-1):
        print("you lose")
    elif(computer==0 and you==1):
        print("you lose")
    elif(computer==0 and you==-1):
        print("you win")
    else:
        print("something went wrong!")
