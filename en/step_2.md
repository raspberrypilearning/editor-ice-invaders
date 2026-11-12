## Freeze the aim

Stop the stick turning when the mouse is clicked.

![stick sprite](images/stick-sprite.png)

You're still working on the **stick sprite**.

## Step 1

Swap the `forever`{:class="block3control"} loop for a `repeat until`{:class="block3control"} loop.

```blocks3
when green flag clicked
go to x: (-168) y: (-51)
+repeat until < >
point towards (mouse-pointer v)
end
```

## Step 2

Add a `mouse down?`{:class="block3sensing"} block to the loop.

```blocks3
when green flag clicked
go to x: (-168) y: (-51)
repeat until <mouse down?>
point towards (mouse-pointer v)
end
```

## Now run your code

Click the **Green Flag** and move the mouse.
Click the mouse and check that the stick stops turning.
