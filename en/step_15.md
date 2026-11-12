## Pop!

Make the ice pop as it disappears.

![ice sprite](images/ice-sprite.png)

You're still working on the **ice sprite**.

## Step 1

Add a `start sound`{:class="block3sound"} block set to `pop`{:class="block3sound"} above the `delete this clone`{:class="block3control"} block.

```blocks3
when I start as a clone
show
wait until <touching (puck v)?>
+start sound (pop v)
delete this clone
```

## Step 2

Add a `change effect by`{:class="block3looks"} block set to `fisheye` and `200`.

```blocks3
wait until <touching (puck v)?>
start sound (pop v)
+change [fisheye v] effect by (200)
delete this clone
```

## Step 3

Add a `change size by`{:class="block3looks"} block set to `20`.

```blocks3
start sound (pop v)
change [fisheye v] effect by (200)
+change size by (20)
delete this clone
```

## Step 4

Add a `wait`{:class="block3control"} block set to `0.05` seconds, so the pop can be seen.

```blocks3
change [fisheye v] effect by (200)
change size by (20)
+wait (0.05) seconds
delete this clone
```

## Now run your code

Click the **Green Flag** and shoot the puck at the ice.
Check that the ice swells and pops before it disappears.

![The ice squashes, pops and disappears when the puck hits it.](images/step-15.gif){:width="450px"}
