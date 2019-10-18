## Adding Conditionals
Now our code is developing some complexity! By adding our variable manipulation into our `for` loop, the code now looks like this:

```python
import random
dice_rolls = 2
dice_sum = 0
for i in range(0,dice_rolls):
  roll = random.randint(1,6)
  dice_sum += roll
  print(f'You rolled a {roll}')
print('You have rolled a total of {dice_sum}')`
```

Let's add some flavor to our responses, dependent on how we roll. We can do this by using conditionals. We'll put a command that only triggers if a certain condition is met. For example, let's add "Critical Fail" in the printed statement if the die roll is a one.

In Python, we can set this as the criteria by replacing our print statement with:

```python
if roll == 1:
  print(f'You rolled a {roll}! Critical Fail')
```

But what if it's *not* a one? We need a catch-all for all the other conditions it could be. This is done in Python with the `else` command. Below our `if` statement and the related print function, add an `else` statement:

```python
else:
  print(f'You rolled a {roll}')
```
    
Now we have two different statements that can be printed. Try running your code until you have a roll that is a one and a roll that is something else.

If we have additional conditions we want to add, we can use a third type of conditional in Python: `elif`. This is used for a specific condition after `if` has been used. Try adding this `elif` statement between the `if` and `else` statements:

```python
elif roll == 6:
  print(f'You rolled a {roll}! Critical Success!')
```

Leave a comment with the *number of rolls* it took to get a Critical Success. 