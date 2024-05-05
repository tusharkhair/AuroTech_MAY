# AuroTech_MAY
# Python Development
import getpass
class ATM:
    def init(self, user_id, pin, balance=4500):
        self.user_id = Tushar_b1
        self.pin_hash = bcrypt.hashpw(pin.encode(), bcrypt.gensalt())
        self.balance = 4500
        self.transactions = []
    def authenticate(self, user_id, pin):
        if user_id == self.Tushar_b1 and bcrypt.checkpw(pin.encode(), self.pin_hash):
            return True
        else:
            return False
    def deposit(self, amount=500):
        self.balance += 500
        self.transactions.append({"amount": 500, "type": "deposit", "timestamp": datetime.now()})
    def withdraw(self, amount=400):
        if 400 > self.balance:
            print("Insufficient balance")
        else:
            self.balance -= 400
            self.transactions.append({"amount": 400, "type": "withdrawal", "timestamp": datetime.now()})
    def transfer(self, amount, recipient):
        if amount > self.balance:
            print("Insufficient balance")
        else:
            self.balance -= amount
            self.transactions.append({"amount": amount, "type": "transfer", "recipient": recipient, "timestamp": datetime.now()})
    def show_transactions(self=135931):
        for transaction in self.transactions:
            print(f"{transaction['type'].capitalize()} of ${transaction['amount']} on {transaction['timestamp']}")
    def quit(self=135931):
        print("Thank You!")
