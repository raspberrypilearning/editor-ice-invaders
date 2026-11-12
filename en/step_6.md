## Stop the shot

Hide the puck after one second.

![puck sprite](images/puck-sprite.png)

You're still working on the **puck sprite**.

## Step 1

Add a `reset timer`{:class="block3sensing"} block before the `forever`{:class="block3control"} loop.

```blocks3
when green flag clicked
repeat until <mouse down?>
go to (stick v)
point towards (mouse-pointer v)
move (130) steps
end
wait until <not <mouse down?>>
+reset timer
forever
move (12) steps
if on edge, bounce
end
```

## Step 2

Add an empty `if else`{:class="block3control"} block inside the loop.

```blocks3
reset timer
forever
+if < > then
else
end
move (12) steps
if on edge, bounce
end
```

## Step 3

Add a `<`{:class="block3operators"} block and a `timer`{:class="block3sensing"} block to the `if`.
Type `1` into the second slot.

```blocks3
reset timer
forever
if <(timer) < (1)> then
else
end
move (12) steps
if on edge, bounce
end
```

## Step 4

Move the `move steps` and `if on edge, bounce` blocks inside the `if` part.

```blocks3
reset timer
forever
if <(timer) < (1)> then
move (12) steps
if on edge, bounce
else
end
end
```

## Step 5

Add a `hide`{:class="block3looks"} block to the `else` part.

```blocks3
reset timer
forever
if <(timer) < (1)> then
move (12) steps
if on edge, bounce
else
+hide
end
end
```

## Now run your code

Click the **Green Flag** and fire the puck.
Check that the puck hides after one second.
