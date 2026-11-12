## Hit the ice

Add a point when the puck hits a piece of ice.

![ice sprite](images/ice-sprite.png)

## Step 1

Click on the **ice sprite**.

Add an empty `wait until`{:class="block3control"} block to the `show` script.

```blocks3
when I start as a clone
show
+wait until < >
```

## Step 2

Add a `touching`{:class="block3sensing"} block set to `puck`.

```blocks3
when I start as a clone
show
wait until <touching (puck v)?>
```

## Step 3

Add a `change score by`{:class="block3variables"} block set to `1`.

```blocks3
when I start as a clone
show
wait until <touching (puck v)?>
+change [score v] by (1)
```

## Now run your code

Click the **Green Flag** and fire the puck at the ice.
Check that the score goes up when the puck hits the ice.
