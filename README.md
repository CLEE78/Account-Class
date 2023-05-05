# Account-Class
# Python program to create Bankaccount class
# with both a deposit() and a withdraw() function
class Bank_Account:
    def __init__(self):
        self.balance=0
        print("Hello!!! Welcome to the Account Deposit & Withdrawal ")
 
    def deposit(self):
        amount=float(input("Enter deposit amount: "))
        self.balance += amount
        print("\n Amount Deposited:",amount)
 
    def withdraw(self):
        amount = float(input("Enter withdrawal amount: "))
        if self.balance>=amount:
            self.balance-=amount
            print("\n Amount withdrawn:", amount)
        else:
            print("\n Insufficient balance  ")
 
    def display(self):
        print("\n Net Available Balance=",self.balance)
 
# Driver code
  
# creating an object of class
s = Bank_Account()
  
# Calling functions with that class object
s.deposit()
s.withdraw()
s.display()
