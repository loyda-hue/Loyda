1
# Loyda
Every commit is a step forward in my coding journey. One day, this repo will tell the story of my growth.

capitals={"usa":"wash",
                  "eth": "addis",
                  "china": "beging"
                  }
#print(dir(capitals))
#print(capitals.get("usa"))
#capitals.update({"germany":"berlin"})
#capitals.update({"usa":"bb"})
#print(capitals)
#capitals.pop("usa")
#print(capitals)
#capitals.popitem()
#print(capitals.keys())
#keys=capitals.keys()

#for key in capitals.keys():
#	print(key)
#print(capitals.values())
#values=capitals.values
#for value in capitals.values():
#	print(value)
#items=capitals.items
#for item in capitals.items():
#	print(item)
#for key, value in capitals.items():
#	print(f"{key}: {value}")

2

#Cocession stand program
menu={"pizza":50,
              "bread":30,
              "eag": 3,
              "coffee":6
              }
print("-------------Menu------------")
for key, value in menu.items():
	print(f"{key}: ${value}")
print("--------------------------------")

cart=[]
total=0
while True:
	food= input("select an item (q to quit): " ).lower()
	if food=="q":
		break
	elif menu.get(food) is not None:
		cart.append(food)
	else:
		print("sorry the item does't exist")

print("-------*----*----*----*----*----*----")
for food in cart:
	total+=menu.get(food)

print("********YOUR ORDER*********")

print(food, end=" ")

print(f"the total amount is ${total}")

3

import random

#print(help(random))
#print(random.randint(1,6))
low=3
high=10
options=("rock", "paper", "scissors")
cards=["1","2","3","4","a","b"]
#print(random.randint(low, high))
#print(random.random())
#print(random.choice(options))
#random.shuffle(cards)
#print(cards)
lowest_num=1
highest_num=100
guesses=0
is_running=True
answer= random.randint(lowest_num, highest_num)
#print(answer)
print(" python number guessing game")
print(f" please select a numbet between {lowest_num} and {highest_num}")
while is_running:
	guess= input( "enter your guess: ")
	if guess.isdigit():
		guess=int(guess)
		guess+= 1
		if guess<lowest_num or guess>highest_num:
			print("sorry that number is out of range")
			print("please select a number between { lowest_num} and {highest_num}")
		elif guess<answer:
			print("too low! try again! ")
		elif guess>answer:
			print("to high! try again!")
		else:
			print(f"correct! the answer was {answer}.")
			print(f"number of giesses: {guesses}")
	else:
		print(" invalid guess")
		print("please select a number between { lowest_num} and {highest_num}")



#def student(name, age, grade, average, rank):
#	print(f" welcome {name} to twuld amare school. ")
#	print(f"you are {age} years old. ")
#	print(f"you are grade {grade} student.")
	#print(f"your average mark is: {average} ")
#	print(f"you are {rank} out of 30")
#student("Beza", 9, 3, 86, 24)
#print("-*-*-*-*-*-*")

#student("Naod", 4,"kg1", 92, 6)
#print("-*-*-*-*-*-*+*")

#student("Betelhem", 20, "first year", 95, 2)

#import random
##for a in range(2):
#	print(random.randint(1,4))
