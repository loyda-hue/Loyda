we1
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




#membership operators
#1.in
#
#2.not in
word= 'Betty code'
letter= input(' guess a letter in the word   ')
if letter not in word:
	print(f" there is not {letter}")
else:
	print(f'{letter} is  found')


students=('betty', 'dan', 'roba', 'zorba', 'nadu')
student=input('enter student name')
if student in students:
	print(f'{student} was found')
else:
	print(f' {student} was not found')
	
email= 'bettycode@gmail.com'
if "@" in email and '.' in email:
	print(' valid email')
else:
	print(' invalid email')





#list compressions

doubles= [x*2 for x in range (1,11)]
triples=[y*3 for y in range (1,11)]
square=[z*z for z in range (1,11)]
print(doubles)
print (triples)
print(square)
fruits=('apple', 'banana', 'orange',  'mango')
fruit_chars=[fruits[0] for fruit in fruits]
print(fruit_chars)
n=[1,2,-3,-4,5,6]
p_n=[n for n in n if n>=0]
n_n=[n for n in n if n<=0]
e_n=[n for n in n if n%2==0]
o_n=[n for n in n if n%2==1]
print(p_n)
print(n_n)
print(e_n)
print(o_n)
grades= [65,80,92,43,21,31,48,79]
passing_grade=[grade for grade in grades if grade>=50]
print(passing_grade)




😃

#include <iostream>
using namespace std;
int main()
{
float num1,num2, add, sub, mult, div;

cout<< " enter the first number :"<<endl;
cin>>num1;
cout<<"enter the second number :"<<endl;
cin>>num2;
add= num1+num2;
sub=num1-num2;
mult=num1*num2;
div=num1/num2;

cout<<"the sum of the two numbers is " <<add<<endl;
cout<<" the subtraction of the two numbers is "<<sub<<endl;
cout<<" the multiplication of the two numbers is "<<mult<<endl;
cout <<" the division of the two numbers is "<<div<<endl;
return 0;
} 


#include <iostream>
using namespace std;
int main()
{ int length, width, area;
cout<<" enter the length: ";
cin>>length;
cout<<" enter the width: ";
cin>>width;
area=length*width;
cout<<"  the area of the rectangle is: "<<area<<" square meters." <<endl;
return 0;
}
    #include<iostream>
using namespace std;
int main ()

{
    int age, num, year, width, length, area;
    cout<<"Hello world!"<<endl;
    cout<<" Enter your age:"<<endl;
    cin>>age;
    cout<<" you are "<< age<< " years old."<<endl;
    cout<<" enter a number"<<endl;
    cin>>num;
    cout<<" You entered number " <<num<<endl;
    cout<<"enter acadamic year: " <<endl;
    cin>>year;
    cout<<"Enter your age: "<<endl;
    cin>>age;
    cout<<"year :"<< year<<endl;
    cout<<"age :"<<age<<endl;
    cout<<"Enter the width of the room:";
    cin>>width;
    cout<<" Enter the length of the room:";
    cin>> length;
    area= length*width;
    cout<<"the area of the the room is " <<area<< " square meters. "<<endl;


    return 0;
}


#include <iostream>
using namespace std;

int main() {
    int apple;
    apple=10;
    cout<<"we have bought " <<apple<< " apples."<<endl;
    return 0;
    } 


#include<iostream>
using namespace std;
enum days {mon=1,tue,wed,thu,fri,sat,sun};
int main()
{
days yesterday= mon ;
days today = thu ;
days tomorrow = fri ;

cout<<"yesterday value "<< yesterday<< endl;
cout<<"tomorrow value" <<tomorrow<<endl;
cout<<"today value"<<today<<endl;
return 0;
    
}




#include <iostream>
using namespace std;

int main() {
    double hours, pay;
    cout<<" Enter hours worked" << endl;
    cin>>hours;
    if (hours<=40)
    pay= hours*180.25;
    else
    pay= hours*180.25 + (hours-40)*120;
    cout<<"total wedges = "<<pay<<"ETB";
    return 0;
    }

#include <iostream>
using namespace std;

int main() {
    double fahrenheit, celcius;
    cout<<" Enter temperature in Fahrenheit: " << endl;
    cin>>fahrenheit;
    celcius= (fahrenheit-32)*5/9;
    cout<<"The temperature in celcius is " <<celcius<<endl;
    return 0;
    }



#include <iostream>
using namespace std;

int main() {
    int mark;
    cout<<"Enter your grade :";
    cin>> mark;
    if (mark>=50)
    cout<< "congratulations you are passed";
    else
    cout<<" sorry you are not passed"<<endl;
    return 0;
    }