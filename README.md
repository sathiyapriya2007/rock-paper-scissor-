# rock-paper-scissor-game
import random
choice=input('choose to play pc/person:')
if choice=='pc':
    a=input("enter rock/scissor/paper(Player):")
    elements=['rock','paper','scissor']
    c=random.choice(elements)
    print('computer choice:',c)
    if a==c:
        print(" It's a tie ")
    elif (a=='rock' and c=='paper') or (a=='scissor' and c=='paper') or (a=='rock' and c=='scissor') :
        print('You won')
    else:
        print('You lose')
else:
    p1=input("Player 1(enter rock/scissor/paper):")
    p2=input("Player 2(enter rock/scissor/paper):")
    if p1==p2:
        print(" It's a tie ")
    elif (p1=='rock' and p2=='paper') or (p1=='scissor' and p2=='paper') or (p1=='rock' and p2=='scissor') :
        print(" Player 1 wins")
    else:
        print("Player 2 wins")

