## Hit the ice

Make a block of ice disappear when the puck hits it.

![ice sprite](images/ice-sprite.png)

You're still working on the **ice sprite**.

## Step 1

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

Add a `delete this clone`{:class="block3control"} block.

```blocks3
when I start as a clone
show
wait until <touching (puck v)?>
+delete this clone
```

## Now run your code

Click the **Green Flag** and shoot the puck at the ice.
Check that the block of ice disappears when the puck hits it.

![A block of ice disappears when the puck hits it.](images/step-14.gif){:width="450px"}
