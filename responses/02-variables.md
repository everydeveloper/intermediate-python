## Printing Variables

All the file is doing right now is printing the sentence "You rolled a die." But the purpose of rolling a die is to come up with a number, so let's do that now. 

We can  make a new variable named `roll`. Variables are simple to make in Python: set the variable equal to what you want it to be. Above the print function, create and set a variable called `roll` equal to 5 by writing:

```python
roll = 5
```

We'll want to print that variable, too, so let's change the print function to reflect what our `roll` variable is set to. This is done through Python's `f-string` functionality. By putting an `f` right before the quotes of the string you're printing, you can then print variables within the string. Let's replace the word 'die' in the sentence to our new `roll` variable. This changes the line to say:

```python
print(f'You rolled a {roll}')
```

Run the code again, and it should say `You rolled a 5`. Nice! Now we're getting a number. Go ahead and `push` your code with the output as the comment within `commit` to move on. 

A die that only rolls 5's isn't useful though, so let's add in the randomness that dice are used for.


## Randomizing Variables


Just like a real die, we want the number we roll to be random. We'll need to use a package to do so. Python is full of packages; think of them like tools you can use for specific situations. Just like how you need a shovel to dig a hole, you need the `random` package to get a random value in Python.

Right now, you should have a `main` function that contains this:

```python
roll = 5
print(f'You rolled a {roll}')
```

To use a package, we'll need to import it. At the top of the file, import the package `random` by writing:

```python
import random 
```

In general, it's good practice to import all packages at the beginning of the script. Now let's use that package to randomize our `roll` variable. To get a random integer with the `random` package, we'll want to use the following format:

```python
random.randint(X,Y)
```

where X and Y are the boundaries of the range you want your random integers to be in. Note that X, the beginning of the range and Y, and the end of the range, are inclusive bounds. Note that X (the beginning of the range) and Y (the end of the range), are inclusive bounds. This means the integers you put as X and Y will be part of possible values. Knowing that, try changing `roll` to equal any integer that is possible to roll on a six-sided die: 1, 2, 3, 4, 5 and 6. There's no need to change anything in the print statement, as we've already tied it to whatever our `roll` variable is. 

Now run the code and put *the number* you rolled as a comment, and then we'll keep this tutorial *rolling*!