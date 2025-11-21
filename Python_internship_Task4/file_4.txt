#Create a Number Guessing Game 
import random
def guessthenum():
  name=input('Enter your name:')
  num=random.randint(1,100)
  unum=int(input('Enter your guess:'))
  chance=1
  while unum!=num:
    if unum>num:
      print('Your guess is too high')
    if unum<num:
      print('Your guess is too low')
    chance = chance+1
    unum=int(input('Enter your guess:'))
  print(f'Bingo!!! You took {chance} chances')
  print('The number was')
  print(num)
  ##Calling
guessthenum()