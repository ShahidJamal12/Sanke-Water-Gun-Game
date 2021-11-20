# Sanke-Water-Gun-Game
import random
print('Welcome To Snake water and gun game\n')
rou = int(input('Enter the numbers of rounds: '))
ro = 1
while ro<=rou:
	if ro<rou:
		print(f"\nRound {ro}")
	if ro==rou:
		print("\nFinal Round")
	a = random.randint(1,3)
	if a == 1:
		a = 's'
	elif a == 2:
		a = 'w'
	elif a == 3:
		a = 'g'
	b = input('Snake(s), Water(w) and Gun(g)\n')
	if b == 's' and a == 'g':
		print(f'\nComp = {a}\nYou = {b}\nYou loose!')
	elif b == 's' and a == 'w':
		print(f'\nComp = {a}\nYou = {b}\nYou Win!')
	if b == 'w' and a == 's':
		print(f'\nComp = {a}\nYou = {b}\nYou loose!')
	elif b == 'w' and a == 'g':
		print(f'\nComp = {a}\nYou = {b}\nYou Win!')
	if b == 'g' and a == 'w':
		print(f'\nComp = {a}\nYou = {b}\nYou loose!')
	elif b == 'g' and a == 's':
		print(f'\nComp = {a}\nYou = {b}\nYou Win!')
	if b == 's' and a == 's':
		print(f'\nComp = {a}\nYou = {b}\nTie')
	elif b == 'g' and a == 'g':
		print(f'\nComp = {a}\nYou = {b}\nTie')
	elif b == 'w' and a == 'w':
		print(f'\nComp = {a}\nYou = {b}\nTie')
	ro = ro + 1
	
