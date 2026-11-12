## Pop!

Make the ice pop when it is hit.

![ice sprite](images/ice-sprite.png)

You're still working on the **ice sprite**.

## Step 1

Add a `start sound`{:class="block3sound"} block set to `pop`{:class="block3sound"}.

```blocks3
when I start as a clone
show
wait until <touching (puck v)?>
change [score v] by (1)
+start sound (pop v)
```

## Step 2

Add a `change effect by`{:class="block3looks"} block set to `fisheye` and `200`.

```blocks3
change [score v] by (1)
start sound (pop v)
+change [fisheye v] effect by (200)
```

## Step 3

Add a `change size by`{:class="block3looks"} block set to `20`.

```blocks3
start sound (pop v)
change [fisheye v] effect by (200)
+change size by (20)
```

## Step 4

Add a `wait`{:class="block3control"} block set to `0.05` seconds.

```blocks3
change [fisheye v] effect by (200)
change size by (20)
+wait (0.05) seconds
```

## Step 5

Add a `hide`{:class="block3looks"} block and a `delete this clone`{:class="block3control"} block.

```blocks3
change size by (20)
wait (0.05) seconds
+hide
+delete this clone
```

## Now run your code

Click the **Green Flag** and fire the puck at the ice.
Check that the ice pops and disappears.
