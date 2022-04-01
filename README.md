# Shopping-List
# : This is my shopping list
ShoppingList = []

# : This is the code for my loop
x= True
while x == True:

# : This is the beginning of the loop
    print("This is your shopping list. What item would you like to add? ")
# : This is the variable that is going to add things to my shopping list
    UserList1 = input("Please enter an item: ")
# : ShoppingList is the actual shopping list
    ShoppingList.append(UserList1)
    print(ShoppingList)

# : This is the variable that removes stuff from my shopping list
    UserRemove = input("Are there any items you want to remove? Type yes or no : ")
    if UserRemove == "yes":
        Remove = input("Type the item you would like to remove: ")
        ShoppingList.remove(Remove)
# : After UserRemove removes stuff, it reprints the shopping list with the stuff removed
        print(ShoppingList)
# : If the user says no, then they just go and enter another item
    elif UserRemove == "no":
        UserList2 = input("Please enter an item: ")
        ShoppingList.append(UserList2)
# : Then it just prints the shopping list with the added item
        print(ShoppingList)
#: This is the part of the code where they can either exit or add more to their shopping list
    UserExit = input('''If you would like to exit, press 1.
                     If you would like to see your current shopping list, press 2: ''')
    if UserExit == "1":
        exit(0)
    elif UserExit == "2":
        print(ShoppingList)
# : if they don't click the right option it will tell them to follow the instructions and the code will loop again
    else:
        print("you stupid boi read the instructions")
        print(ShoppingList)
