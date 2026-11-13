## Animate player

Make the player swing their arm when the puck is shot.

![player sprite](images/player-sprite.png){:width="150px"}

Click on the **player sprite**.

## Step 1

Add a `repeat until`{:class="block3control"} loop, with a `mouse down?`{:class="block3sensing"} block.

```blocks3
when I receive (reset v)
go to x: (-159) y: (-58)
set drag mode [not draggable v]
+ repeat until <mouse down?>
end
```

## Step 2

Add a `switch costume`{:class="block3looks"} block and set to `costume 1`{:class="block3looks"}.

```blocks3
when I receive (reset v)
go to x: (-159) y: (-58)
set drag mode [not draggable v]
repeat until <mouse down?>
switch costume to (costume 1 v)
end
```

## Step 3

Add a `wait until`{:class="block3control"} block with `not mouse down?`{:class="block3sensing"} after the loop.

```blocks3
when I receive (reset v)
go to x: (-159) y: (-58)
set drag mode [not draggable v]
repeat until <mouse down?>
switch costume to (costume 1 v)
end
+wait until <not <mouse down?>>
```

## Step 4

Add another `switch costume to`{:class="block3looks"} block, but set to `costume 2`{:class="block3looks"}. 

Then add a `wait`{:class="block3control"} and  `switch costume`{:class="block3looks"} back.

```blocks3
wait until <not <mouse down?>>
+switch costume to (costume 2 v)
+wait (0.3) seconds
+switch costume to (costume 1 v)
```

## Now run your code

Click the **Green Flag**. Shoot the puck and check that the player animates.

![The player swings the stick when the mouse is released.](images/step-6.gif){:width="450px"}
