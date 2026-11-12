## Swing the stick

Make the player swing when the puck is fired.

![player sprite](images/player-sprite.png)

## Step 1

Click on the **player sprite**.

Add a `repeat until`{:class="block3control"} loop.

```blocks3
when green flag clicked
+repeat until < >
end
```

## Step 2

Add a `mouse down?`{:class="block3sensing"} block to the loop.

```blocks3
when green flag clicked
repeat until <mouse down?>
end
```

## Step 3

Add a `switch costume to`{:class="block3looks"} block set to `costume 1`{:class="block3looks"} inside the loop.

```blocks3
when green flag clicked
repeat until <mouse down?>
switch costume to (costume 1 v)
end
```

## Step 4

Add a `wait until`{:class="block3control"} block with `not mouse down?`{:class="block3sensing"} after the loop.

```blocks3
when green flag clicked
repeat until <mouse down?>
switch costume to (costume 1 v)
end
+wait until <not <mouse down?>>
```

## Step 5

Add a `start sound`{:class="block3sound"} block set to `Tennis Hit`{:class="block3sound"}.

```blocks3
wait until <not <mouse down?>>
+start sound (Tennis Hit v)
```

## Step 6

Add a `switch costume to`{:class="block3looks"} block set to `costume 2`{:class="block3looks"}.

```blocks3
wait until <not <mouse down?>>
start sound (Tennis Hit v)
+switch costume to (costume 2 v)
```

## Step 7

Add a `wait`{:class="block3control"} block set to `0.3` seconds.

```blocks3
start sound (Tennis Hit v)
switch costume to (costume 2 v)
+wait (0.3) seconds
```

## Step 8

Add a `switch costume to`{:class="block3looks"} block set to `costume 1`{:class="block3looks"}.

```blocks3
switch costume to (costume 2 v)
wait (0.3) seconds
+switch costume to (costume 1 v)
```

## Now run your code

Click the **Green Flag**, aim, then click and release the mouse.
Check that the player swings and the sound plays.
