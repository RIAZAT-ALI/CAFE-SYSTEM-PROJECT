# CAFE-SYSTEM-PROJECT



# PROJECT BASED ON HOTEL MENU

# In this project we use DICTIONARY and CONDITIONAL STATEMENT.

# When we go any restaurant then we see one sheet in which orders list so in list left side ITEMS name and RIGHT side his prices. so on the basis left and right we use the dictionary concept mean key and value pair.


menu = {
    'Pizza': 300,
    'Pasta': 200,
    'Burger': 100,
    'Salad': 80,
    'Finger Chips': 100,
    'Cofee': 150,

}

print("WELCOME TO PYTHON RESTAURENT")
print("Pizza: Rs.300\nPasta: Rs.200\nBurger: Rs.100\nSalad: Rs.80\nFinger Chips: Rs.100\nCofee: Rs.150")

# Make a variable for customer who add any orders items that add on.

order_total = 0
# 300 + 200 = 500

item_1 = input("Enter the name of item you want to order = ")

if item_1 in menu:   # membership opertor use for item either available in our restaurant or not.
    order_total += menu[item_1]  #0 + 150
    print(f"your item {item_1} has been added to your order")

else:
    print(f"Order item {item_1} is not available yet!")

another_order = input("Do you want to add another item? (Yes/No)")

if another_order == "Yes": 
    item_2 = input("Enter the name of second item = ")

    if item_2 in menu:   #Item either available in our restaurant or not.
        order_total += menu[item_2]
        print(f"Item {item_2} has been added to order")
    else:
        print(f"Order item {item_2} is not available!")

print(f"The total amount of items to pay is {order_total}.")        
