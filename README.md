# snake-water-gun-game
# author-shreya mishra

import random

def gamewin (comp,you):
    if Comp== you:
        return None
    elif comp == 's':
        if you =='w':
            return False
        elif you =='g':
            return True
    elif comp == 'w':
        if you =='g':
            return False
        elif you =='s':
            return True
    elif comp == 'g':
        if you =='s':
            return False
        elif you =='w':
            return True
    
print("Comp Turn:Snake(s),Water(w),Gun(g)?")
randNo =random.randint (1,3)
if randNo == 1:
    Comp = 's'
elif randNo == 2:
    Comp = 'w'
elif randNo == 3:
    Comp = 'g'

you= input("Your Turn:Snake(s) Water(w) Gun(g)?")
a= gamewin (Comp,you)

print(f"Computer chose{Comp}")
print(f"You chose{you}")



if a == None:
    print("The game is tie!")
elif a:
    print("You Win!")
elif a:
    print("You Lose!")
