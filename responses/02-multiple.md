You rolled a {{ roll }}? 😄 Nice!

## Making Python Roll Multiple Dice
Before moving on, make sure the `main` function contains:

```python
import random
roll = random.randint(1, 6)
print(f'You rolled a {roll}')
```

Now, what if we wanted to roll two dice? Well, one way to do that is to run the file twice. Another way is to duplicate the print statement within the file. However, this would get tedious for larger projects, so let's make use of a great Python feature: `for` loops. A `for` loop iterates over a range of values and performs a set of commands for all of those values. 

How many dice do we want to roll? Let's go with two for now. Make a variable called `dice_rolls` below `import random` but above everything else, and set it equal to two.

Now let's make the `for loop`. Right below where you set `dice_rolls` type:

```python
for i in range(0,dice_rolls):
``` 

Let's unpack what this means. If we were to make this a grammatical sentence it would read something like this:

"`for` every `i`ndex `in` a `range` starting after `0` until the value is equal to `dice_rolls`, do this`:`"

We would then have a set of commands it would do for every `i`. We already have the commands we want to be repeated, we just have to tell Python that by indenting them. Once they're indented, save the file and run it to get the two rolls.

## Manipulating Variables

With a `for` loop implemented, your code takes the form of this:

```python
import random
dice_rolls = 2
for i in range(0,dice_rolls):
  roll = random.randint(1,6)
  print(f'You rolled a {roll}')
```

In most game situations, rolling multiple dice is followed by adding their values together. Let's do that now. In Python, arithmetic can be performed on variables just by using the equivalent mathematical symbols. Want to add two variables together? It's as simple as: `variable_sum = variable_1 + variable_2`. Since our dice values are stored in a single updating variable instead of separate variables, however, we'll have to add the values upon themselves. First, make a variable called dice_sum above the `for` loop, and set it equal to 0:

```python
dice_sum = 0
```

We'll be adding each value of `dice_roll` we get to this `dice_sum` variable as we loop through each dice roll. In the `for` loop, right after the `roll` variable is assigned, type:

```python
dice_sum = dice_sum + roll
```

Another way we can do this in Python is using the `+=` operator:

```python
dice_sum += roll
```

It doesn't matter which version you prefer, just go with whichever way is easier for you to visualize. Finally, let's print out our final value for `dice_sum`. After the `for` loop is finished, type:
```python
print('You have rolled a total of {dice_sum}')
```
Make sure this statement is not indented (since that would include it in the for loop). Overall, your code should look like this:

```python
import random
dice_rolls = 2
dice_sum = 0
for i in range(0,dice_rolls):
  roll = random.randint(1,6)
  dice_sum += roll
  print(f'You rolled a {roll}')
print('You have rolled a total of {dice_sum}')
```
If you save and run the file, you'll now get the values of the two dice rolls and their combined sum. Now our code is developing some complexity!

*[Push your code]({{ repoUrl }}/issues/1) to GitHub to continue*