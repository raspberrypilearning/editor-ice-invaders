## Aim the stick

Make the stick follow the mouse.

The starter project is open beside these instructions.
It has all the sprites and backdrops needed.

![stick sprite](images/stick-sprite.png)

## Step 1

Click on the **stick sprite**.

Add blocks to set the starting position.

```blocks3
when green flag clicked
go to x: (-168) y: (-51)
```

## Step 2

Add a `forever`{:class="block3control"} loop with a `point towards`{:class="block3motion"} block inside.

```blocks3
when green flag clicked
go to x: (-168) y: (-51)
+forever
point towards (mouse-pointer v)
end
```

## Now run your code

Click the **Green Flag** and move the mouse.
Check that the stick points at the mouse pointer.
