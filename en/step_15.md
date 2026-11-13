## Burst effect

Make the ice burst as it disappears.

![ice sprite](images/ice-sprite.png){:width="150px"}

You're still working on the **ice sprite**.

## Step 1

Add a `change effect by`{:class="block3looks"} block set to `fisheye` and `200` under the `start sound`{:class="block3sound"} block.

```blocks3
when I start as a clone
show
wait until <touching (puck v)?>
start sound (pop v)
+change [fisheye v] effect by (200)
delete this clone
```

## Step 2

Add a `change size by`{:class="block3looks"} block set to `20`.

```blocks3
wait until <touching (puck v)?>
start sound (pop v)
change [fisheye v] effect by (200)
+change size by (20)
delete this clone
```

## Step 3

Add a `wait`{:class="block3control"} block set to `0.05` seconds, so the burst can be seen.

```blocks3
change [fisheye v] effect by (200)
change size by (20)
+wait (0.05) seconds
delete this clone
```

## Now run your code

Click the **Green Flag** and shoot the puck at the ice.
Check that the ice swells and bursts before it disappears.

![The ice swells and bursts when the puck hits it.](images/step-15.gif){:width="450px"}
