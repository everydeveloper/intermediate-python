{{ game }}! Wow that's a classic! You might be able to make a version of {{ game }} when we are done!

## Running a Python file

Let's look at our Python file. Inside we see a function `main` that will contain all of your commands as you create the dice roller:

```python
def main():
    #print('You rolled a die')
```

Below that, you'll see an `if` statement calling that function:

```python
`if __name__== "__main__":
    main()`
```
By doing this, the function `main` will run whenever you run the Python script. As you develop the dice roller, be sure to only manipulate the code within the `main` function; nothing else will need to be changed. 

Right now the only line in our `main` function is a `print()` function:`#print('You rolled a die')`. This will print whatever is inside the parenthesis. There's a `#` in front of it right now, which means it's a comment. Uncomment it by removing the `#` to let Python read it, and save the file.

You can run the Python script by typing `python dice_roller.py` in a terminal, provided you're in the correct directory. If not, run the script by typing `python /path/to/directory/dice_roller.py`, where `/path/to/directory` is replaced with the path to the file on your own system.

You'll see the following nifty, albeit not very useful line printed out in your terminal: "You've rolled a die". We'll make it more informative in a bit, but first, let's push those changes to GitHub. 


## Pushing your changes

Whenever you change files in your repository, you'll want to `add` and `commit` the file, which allows you to add a message detailing what you changed. Then you can `push` the updated version, along with your comments, to GitHub. 

Let's do those three steps:

1. Git Add: `git add dice_roller.py`
2. Git Commit: `git commit -m "I uncommented line 2"`
3. Git Push: `git push`