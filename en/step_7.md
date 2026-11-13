## Reload the puck

Bring the puck back to the stick for the next shot.

![puck sprite](images/puck-sprite.png){:width="150px"}

You're still working on the **puck sprite**.

## Step 1

Add a `hide`{:class="block3looks"} block to the `else`{:class="block3control"} part.

Then add a `broadcast`{:class="block3events"} block under it, and choose `reset`{:class="block3events"} from the drop-down.

```blocks3
reset timer
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

## Step 2

Add a `show`{:class="block3looks"} block to the top of the script, so the puck comes back for the next shot.

```blocks3
when I receive [reset v]
+show
set rotation style [don't rotate v]
set drag mode [not draggable v]
repeat until <mouse down?>
go to (stick v)
point towards (mouse-pointer v)
move (130) steps
end
```

## Now run your code

Click the **Green Flag** and shoot the puck.
Check that the puck disappears, then reappears on the stick ready for the next shot.

![The puck hides one second after it is shot, then comes back to the stick.](images/step-7.gif){:width="450px"}
