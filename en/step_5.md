## Hide the puck

Hide the puck after one second.

![puck sprite](images/puck-sprite.png){:width="150px"}

You're still working on the **puck sprite**.

## Step 1

Add an empty `if else`{:class="block3control"} block inside the loop.

```blocks3
wait until <not <mouse down?>>
forever
+if < > then
else
end
move (12) steps
if on edge, bounce
end
```

## Step 2

Drag the `move`{:class="block3motion"} and `if on edge`{:class="block3motion"} blocks inside the `if`{:class="block3control"} part.

![Dragging the move and if on edge blocks inside the if part.](images/step-5-drag.gif){:width="450px"}

## Step 3

Add a `less than`{:class="block3operators"} block and a `timer`{:class="block3sensing"} block to the `if`{:class="block3control"}.

Type `1` into the second box.

```blocks3
wait until <not <mouse down?>>
forever
+if <(timer) < (1)> then
move (12) steps
if on edge, bounce
else
end
end
```

## Step 4

Add a `hide`{:class="block3looks"} block to the `else`{:class="block3control"} part.

Then add a `broadcast`{:class="block3events"} block under it, and choose `reset`{:class="block3events"} from the drop-down.

Add a `show`{:class="block3looks"} block to the top of the script, so the puck comes back for the next shot.

```blocks3
when I receive (reset v)
+show
repeat until <mouse down?>
go to (stick v)
point towards (mouse-pointer v)
move (130) steps
end
wait until <not <mouse down?>>
forever
if <(timer) < (1)> then
move (12) steps
if on edge, bounce
else
+hide
+broadcast (reset v)
end
end
```

## Step 5

Add a `reset timer`{:class="block3sensing"} block before the `forever`{:class="block3control"} loop.

```blocks3
wait until <not <mouse down?>>
+reset timer
forever
if <(timer) < (1)> then
move (12) steps
if on edge, bounce
else
hide
end
end
```

## Now run your code

Click the **Green Flag** and shoot the puck.
Check that the puck hides after one second.

> [!TIP]
>
> Change the number next to `timer` to make the puck stop sooner or later.

![The puck hides one second after it is shot.](images/step-5.gif){:width="450px"}
