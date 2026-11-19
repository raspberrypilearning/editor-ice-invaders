## Shoot the puck

Send the puck flying when the mouse is released.

![puck sprite](images/puck-sprite.png){:width="80px"}

You're still working on the **puck sprite**.

## Step 1

Make the **puck** wait until the mouse is released by adding a `wait until`{:class="block3control"} block with a `not`{:class="block3operators"} and a `mouse down?`{:class="block3sensing"} inside.

```blocks3
when I receive [reset v]
set rotation style [don't rotate v]
set drag mode [not draggable v]
repeat until <mouse down?>
go to (stick v)
point towards (mouse-pointer v)
move (130) steps
end
+wait until <not <mouse down?>>
```

## Step 2

Add a `forever`{:class="block3control"} loop with a `move steps`{:class="block3motion"} block inside.


```blocks3
wait until <not <mouse down?>>
+forever
move (10) steps
end
```

## Step 3

Add an `if on edge, bounce`{:class="block3motion"} block inside the `forever`{:class="block3control"} loop.

```blocks3
wait until <not <mouse down?>>
forever
move (10) steps
+if on edge, bounce
end
```

> [!TIP]
>
> Make the **puck** move faster or slower by experimenting with different numbers in the `move`{:class="block3motion"} block.

## Now run your code

Click the **Green Flag** and then click. Check that the **puck** flies off in the direction you aimed at.

![The puck flies off in the direction aimed when the mouse is released.](images/step-5.gif){:width="450px"}
 