class ubin:
      def __init__(self):
           self.balance=0
           print("welcome to UBIN")
      def deposit(self):
          amount=float(input("enter amount to be deposited:"))
          self.balance+=amount
          print("\n Deposited amount :",amount)
      def withdraw(self):
          amount=float(input("enter amount to be withdrawn:"))
          if self.balance>=amount:
              self.balance-=amount
              print("\n withdraw :",amount)
          else:
              print("\n Insufficient balance")
      def checkbal(self):
          print("\n Net available balance:",self.balance)
#driver code
p=ubin()
p.deposit()
p.withdraw()
p.checkbal
     
