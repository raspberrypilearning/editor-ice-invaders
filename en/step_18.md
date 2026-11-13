## Keep score

Count the ice blocks that get hit.

![ice sprite](images/ice-sprite.png){:width="150px"}

You're still working on the **ice sprite**.

## Step 1

Make a variable called `score`{:class="block3variables"} for all sprites.

![The Make a Variable button in Scratch.](images/make-a-variable.png){:width="250px"}

## Step 2

Add a `set score to`{:class="block3variables"} block set to `0` at the top of the green flag script.

```blocks3
when green flag clicked
+set [score v] to (0)
set [ice speed v] to (3)
hide
go to x: (139) y: (-120)
```

## Step 3

Add a `change score by`{:class="block3variables"} block set to `1` under the `wait until`{:class="block3control"} block.

```blocks3
when I start as a clone
show
wait until <touching (puck v)?>
+change [score v] by (1)
start sound (pop v)
change [fisheye v] effect by (200)
change size by (20)
wait (0.05) seconds
delete this clone
```

## Now run your code

Click the **Green Flag** and shoot the puck at the ice.
Check that the score goes up by one for every block of ice hit.

![The score goes up by 1 when the puck hits a piece of ice.](images/step-18.gif){:width="450px"}
