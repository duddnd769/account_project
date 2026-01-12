# account_projec!

---

### 🧩 Account 클래스 코드

```python
import random

class Account:
    def __init__(self, owner, balance):
        self.bank = "SC은행"
        self.owner = owner
        self.balance = balance
        self.account_number = self.create_account_number()

    def create_account_number(self):
        part1 = random.randint(100, 999)
        part2 = random.randint(10, 99)
        part3 = random.randint(100000, 999999)
        return f"{part1}-{part2}-{part3}"

acc = Account("정영웅", 1000000)

print(acc.bank)
print(acc.owner)
print(acc.account_number)
print(acc.balance)


import random

class Account:
    # 🔹 클래스 변수 (계좌 개수)
    account_count = 0

    def __init__(self, owner, balance):
        self.bank = "SC은행"
        self.owner = owner
        self.balance = balance
        self.account_number = self.create_account_number()

        # 🔹 계좌 생성될 때마다 +1
        Account.account_count += 1

    def create_account_number(self):
        return f"{random.randint(100,999)}-{random.randint(10,99)}-{random.randint(100000,999999)}"

acc1 = Account("정영웅", 1000)
acc2 = Account("홍길동", 2000)
acc3 = Account("김철수", 3000)

Account.get_account_num()

acc1 = Account("정영웅", 1000)
acc2 = Account("홍길동", 2000)
acc3 = Account("김철수", 3000)

Account.get_account_num()







