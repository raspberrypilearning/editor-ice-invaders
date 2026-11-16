## Stop the puck

Stop the puck one second after it is shot.

![puck sprite](images/puck-sprite.png){:width="150px"}

You're still working on the **puck sprite**.

## Step 1

Add an `if else`{:class="block3control"} block inside the loop.

Hover over the `move`{:class="block3motion"} and `on edge`{:class="block3motion"} blocks so that they snap into place.

![Adding an if else block, then dragging the move and if on edge blocks inside the if part.](images/step-6-if.gif){:width="450px"}

## Step 2

Time less than one second by adding a `less than`{:class="block3operators"} block with `timer`{:class="block3sensing"} in the first box.

Then type `1` into the second box.

```blocks3
wait until <not <mouse down?>>
forever
+if <(timer) < (1)> then
move (10) steps
if on edge, bounce
else
end
end
```

> [!TIP]
>
> Change the number next to `timer`{:class="block3sensing"} to make the puck slide for longer.

## Step 3

Add a `reset timer`{:class="block3sensing"} block before the `forever`{:class="block3control"} loop.

```blocks3
wait until <not <mouse down?>>
+reset timer
forever
if <(timer) < (1)> then
move (10) steps
if on edge, bounce
else
end
end
```

## Now run your code

Click the **Green Flag** and shoot the puck. Check that the puck stops after `1` second.

![The puck stops one second after it is shot.](images/step-6.gif){:width="450px"}
