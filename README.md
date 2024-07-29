letters=['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z','A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z']

symbols=['!','@','$','#','%','^','&','*','(',')','_','-','+','=','/',':',';','?']

numbers=['1','2','3','4','5','6','7','8','9','0']

import random

print("Welcome to the Pypassword Generator!")

nr_letters=int(input("How many letters woould you like in password? \n"))

nr_symbols=int(input("How many symbols would you like? \n"))

nr_numbers=int(input("How many numbers wolud you like?\n"))


#Easy Password

#password=""


#for char in range(1,nr_letters+1):

#random_letters=random.choice(letters)

#password+=random_letters

#We can directly write Password +=random.choice(letters)

#    password +=random.choice(letters)

#for char in range(1,nr_symbols+1):

 #   password+=random.choice(symbols)
    
#for char in range(1,nr_numbers+1):
 
 #   password+=random.choice(numbers)
    
#print(f"You Easy Password is: {password}")

#Hard Password

password_list=[]

for char in range(1,nr_letters+1):
    
     password_list.append(random.choice(letters))

for char in range(1,nr_symbols+1):
    
     password_list.append(random.choice(symbols))

for char in range(1,nr_numbers+1):
    
     password_list.append(random.choice(numbers))
    
#print(password_list)

random.shuffle(password_list)

#print(password_list)

password=""

for char in password_list:
    
     password+=char


print(f"Your Password is: {password}")
