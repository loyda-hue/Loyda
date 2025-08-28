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