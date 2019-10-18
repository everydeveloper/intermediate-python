Wow, it only took {{ rollNum }} rolls? 🤩 You must be lucky! 🍀

With the conditionals added, your code should look something like this:

```python
import random
dice_rolls = 2
dice_sum = 0
for i in range(0,dice_rolls):
    roll = random.randint(1,6)
    dice_sum += roll
    if roll == 1:
        print(f'You rolled a {roll}! Critical Fail')
    elif roll == 6:
        print(f'You rolled a {roll}! Critical Success!')
    else:
        print(f'You rolled a {roll}')
print(f'You have rolled a total of {dice_sum}')
```

We have a working dice roller right now! It's useful for a very specific situation: rolling two six-sided dice. What if we want to change the number of dice we roll? We can manually edit the code each time, but there's a better way to do this: adding a user `input`.

Instead of having `dice_rolls` set to a specific value, let's set it equal to:
```python
int(input('How many dice would you like to roll?'))
```

Running the code will give a prompt with that question and we can input our desired number of dice. One thing to note: the value a user inputs defaults to a `str` type and we need it to be a whole number, or an `int` in Python; that's why we encompass the `input` command in an `int()`. Try it out!

Tabletop games use dice with all number of sides so it'll be useful to add a user input for that too. Below where you set `dice_rolls` add this line:

```python
dice_size = int(input('How many sides are the dice?'))
```

When changing a value we had assumed to be a specific number previously, we need to make sure the rest of our code still makes sense. All dice start with one, so our `if` statement regarding one still makes sense. Our `elif` statement regarding six doesn't though, as it is no longer guaranteed to be the highest number. Let's make it so our "Critical Success" line is printed to whatever the highest number of our desired dice is. The highest number a dice can roll is the same as the number of sides, so we just to replace our `elif` statement with:

```python
elif roll == dice_size:
```

Try it out! Now you can manually input the number of dice and number of sides on the dice knowing that the `Critical Success!` line will realign accordingly. 

*[push your code]({{ repoUrl }}/issues/1) to GitHub to finish the course!*