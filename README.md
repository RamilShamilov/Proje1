# Proje1
Chapter 1
Your first day at your new job 👩‍💻👨‍💻
You are starting a new job as a junior software developer in an IT company.

The company’s HR department asks you to fill out a form, so you start by assigning your personal information to corresponding variables.

📌 Create a variable for your name, surname, age, ID number, place of residence, to specify if you have active health insurance or not, and lastly one for specifying your nationality.

#Please assign your personal information to variables
my_name =  "Ramil"
my_surname = "Shamilov"
my_age = 18
id_number = 123456789
where_i_live = "Ganja"
health_ansurance = True
my_nationality = "Azerbaijan"
###Meet And Greet Introduce yourself to your new co-workers.

📌 Use a f-string to print "My name is Joey Tribbiani I am 25 years old and I live in London”.

#Write a sentence using the print function to describe yourself using the variables above in the correct data type
print(f"My name is {my_name} {my_surname} I am {str(my_age)} years old, I live in {where_i_live}")
My name is Ramil Shamilov I am 18 years old, I live in Ganja
Equipment starter pack
The HR department asks you to list the items you would need to improve your work efficiency

Mandatory:

Laptop
Headset
Second monitor
Optional:

Mousepad
USB drive
External drive
📌 Create a shopping list that contains items above and print it.

#Create the item_list
item_list = ['Laptop', 'Headset', 'Second Monitor', 'Mousepad' 'USB Drive', 'External Drive']
#Print the list
print(item_list)
['Laptop', 'Headset', 'Second Monitor', 'MousepadUSB Drive', 'External Drive']
####What is mandatory and what is optional?

📌 Use list slicing to devide your list in two list: 'mandatory_item_list' and 'optional_item_list' and print both to the screen.

#Use list slicing to divide the mandatory items
mandatory_item_list = item_list[0:3]
#Use list slicing to divide the optional items
optional_item_list = item_list[3:6]
#Print both to the screen
print(mandatory_item_list)
print(optional_item_list)
['Laptop', 'Headset', 'Second Monitor']
['MousepadUSB Drive', 'External Drive']
Go Shopping
Next, you will have to go and purchase these items, the finance department confirmed a budget of $5000.

📌 Assign 5000 to a variable called limit, so you know how much you can spend.

#Assign the spending limit value to a variable called limit
limit = 5000
####Price dictionary

Before you start shopping yo need to find the best items that you can buy within the company budget.

📌 Prepare a dictionary called “price_sheet” that includes the items as keys and the prices as values.

#Create a dictionary that contains each item and its price
price_sheet = {
    'Laptop': 1500,
    'Headset': 100,
    'Second Monitor': 200,
    'Mousepad': 50,
    'USB Drive': 70,
    'External Drive': 250
}
####Shopping functions

You need to define three functions that will help you during shopping.

📌 First, create an empty list that will be your shopping cart. Here you will add the items you need to purchase.

Define a function for both adding items to the cart and removing them from the item_list.
📌 The "add_to_cart" function should take the item name and the quantity to buy as an argument.

Define a function that will create an invoice.
📌 The "create_invoice" function should calculate the taxes of each item (18%) and add it to the total amount.

Define a function for the checkout.
📌 The "checkout" function should subtract the total amount from the budget and print a statement to inform if the payment was successful.

#Initialize the cart list
cart_list = []
#Define the "add_to_cart" function
def add_to_cart_list(item, quantity):
    cart.append((item, quantity))
    cart_list.remove(item)
#Define the "create_invoice" function
def create_invoice():
    total_amount_inc_tax = 0
    for item, quantity in cart:
        price = price_sheet[item]
        tax = 0.18 * price
        total = (tax + price) * quantity
        total_amount_inc_tax += total
        print('Item:', item, '\t', 'Price:', price, '\t', 'Quantity:', '\t', 'Tax:', tax, 'Total:', total, '\n')
    
        print("After the taxes are applied the total amount is:", '\t', total_amount_inc_tax )
     
        return total_amount_inc_tax
#Define the "checkout" function
def checkout():
    global limit 
    total_amount = create_invoice()
    if limit == 0: 
        print("You dont have any budget")
    elif total_amount > limit:
        print("The amoount you have to pay is above the spending limit. You have to drop some items.")
    else: 
        limit = total_amount 
        print(f"The total amount (incl. taxes) youve paid is {total_amount}. You have {limit} dollars left.")
Let's shop!

#Call the "add_to_cart" function for each item
def add_to_cart():
#Add first item to cart
    add_to_cart("Laptop", 1)
 
 #Add second item to cart
    add_to_cart("Headset", 8)
 
 #Add third item to cart
    add_to_cart("Second Monitor", 1)
 
 #Add fourth item to cart
    add_to_cart("Mousepad", 1)
 
 #Add fifth item to cart
    add_to_cart("USB Drive", 2)
   
 #Add last item to cart
    add_to_cart("External Drive", 4)
​
 #Call the create "checkout" function to pay for all your items 
def checkout(cart_list):
  Input In [53]
    def checkout(cart_list):
                            ^
IndentationError: expected an indented block


###Game Night

You are back at the office and the HR department organizes a welcome party for new employees.

You decide to create a Rock-Paper-Scissor game.

📌 Create a Rock-Paper-Scissor game in which the user plays against the computer. The player will choose one of the actions, and the computer will choose its action randomly.

#Import the random library
import random 
#create a list containing the three actions of the game.
action_list = ['rock', 'paper', 'scissors']
#Set the scores of players to 0
computer_score = 0
player_score = 0 
​
#Ask the user how many rounds they want to play
total_rounds = input("How many rounds do you want to play? Please enter a number here: ")
​
#Add a round_counter that is 0 at the beginning
round_counter = 0
​
#Write a while loop and put the game inside
​
while True:
  #Increase round_counter by and print it
    round_counter += 1
    print("Round number:", round_counter)
​
  #Select a random action for computer
    computer_choice = random.choice(section_list)
​
  #Ask player to choose an action
    player_choice = input("Please choose your acttion:")
​
  #Print the players choices
    print("Computer:", computer_choice)
    print("Player:", player_choice)
​
​
  #tie condition
    if computer_choice == player_choice:
        print("Tie! Both players choose the same action.")
​
  #Remaining conditions
    elif computer_choice == 'paper'
    if player_choice == 'rock' 
      print("Winner is: Computer")
      computer_score += 1 
    else: 
        print("Winner is: player")
        player_score += 1
    elif computer_choice == 'rock'
      if player_choice == 'paper'
        print("Winner is: Player")
        player_score += 1
      else:
        print("Winner is: Computer")
        computer_score += 1
    elif computer_choice == 'scissors'
      if player_choicece == 'paper'
        print("Winner is: Computer")
        computer_score += 1
      else:
        print("Winner is: Computer")
        computer_score += 1
      else:
        print("Winner is: Player")
      player_score += 1
  #Stop the while loop if the round_counter equals the number of total rounds
      if round_counter == int(total_rounds):
      break
​
#Print the outcome of the game by using conditional statements
if computer_score == player_score:
  print("There is no winner, tie.", computer_score, ":", player_score)
elif computer_score > player_score:
  print("Computer won with score", computer_score, ":", player_score)
elif computer_score < player_score:
  print("Player won with score ", computer_score , ":", player_score)
  Input In [47]
    elif computer_choice == "paper"
                                   ^
SyntaxError: invalid syntax


Your first task
Rachel asks you to write a program to track the name and revenue each employee brings.

Create the "salesperson_revenue" dictionary to see the employee name as a key and the revenue as a value.

📌 Every employee starts with 0 revenue.

Define the "enter_revenue" function.

📌 The function takes the name and revenue as an argument and updates the salesperson_revenue dictionary.

#Create salesperson_revenue dictionary
salesperson_revenue = {
    "Ben": 0,
    "Omer": 0,
    "Karen": 0,
    "Ramil": 0,
    "Shahin": 0,
    "Rasim": 0,
    "Bora": 0, 
    "Ross": 0,
    "Ellen": 0, 
}
​
#Define enter_revenue function
def enter_revenue(name, revenue):
  global salesperson_revenue
  salesperson_revenue[name] += revenue
​
####Try out the functions

In a while loop ask the user to give the name of the employee and for the revenue

📌 If the user enters “quit” the loop should break.

After that, print out the salesperson_revenue dictionary.

#Asking user employee name as input
def enter_revenue():
        name = input("Employee name: ")
        if name == "quit":
            break
            revenue = list(input("Enter revenue: "))
            enter_revenue(name, revenue)
            print("{name}s revenue is {salesperson_revenue{name}} ")
  Input In [51]
    break
    ^
SyntaxError: 'break' outside loop


#Print the salesperson_revenue dictionary
print(salesperson_revenue)
{'Ben': 0, 'Omer': 0, 'Karen': 0, 'Ramil': 0, 'Shahin': 0, 'Rasim': 0, 'Bora': 0, 'Ross': 0, 'Ellen': 0}
​
