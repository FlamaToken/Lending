# Lending with negative interest

We are building a protocol that will allow borrowers to pay negative interest on their loans thanks to farming/staking.
How can we achieve that? Let’s see that with an example:

**Current methods:**

Alice deposits 100 coins in a platform to borrow 100 USD with a 5% interest rate.
After 1 year, Alice will have to deposit back the amount borrowed (100 USD) + 5% (5 USD) = 105 USD in order to claim back her 100 coins.
With current borrowing methods, Alice pays 1.05 USD (= 105/100) to claim each coin.

**The inverse lending method:**

Alice deposits 100 coins in a platform to borrow 100 USD with a 5% interest rate.
The 100 coins Alice deposited are sent to the highest yield paying farming/staking protocol.

**Option 1 - Collateral-currency yield**

The 100 "coins" are sent to a protocol that pays the yield in the same "coins" as the collateral (deposited).
After 1 year, Alice's collateral has grown from 100 to 110 "coins".
Alice will have to deposit 105 USD to claim 110 coins.
With this new method, Alice pays 0,9545 USD (= 105/110) to claim each coin.

**Option 2 - Borrow-currency yield**

The 100 "coins" are sent to a protocol that pays the yield in the same "coins" as the borrowed (withdrawn).
After 1 year, Alice's withdrawn amount + interest has been reduced (repayed) from 105 USD to 95 USD.
Alice will have to deposit 95 USD to claim 110 coins.
With this new method, Alice pays 0,95 USD (= 95/100) to claim each coin.

**Option 3 - Different-currency yield**

If there's a protocol that pays a higher yield in a different type of curreny, Alice can choose to convert it to either the Collateral or Borrow currency and enjoy the same advantages of options 1 and 2

**Now Alice can borrow money without missing on the cost of opportunity of farming/staking!**

**Code:**
- https://github.com/FlamaToken/Lending/
