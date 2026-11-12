## Keep them coming

Make a new column of ice every few seconds.

![ice sprite](images/ice-sprite.png)

You're still working on the **ice sprite**.

## Step 1

Add a `forever`{:class="block3control"} loop to the end of the green flag script.
Add a `wait`{:class="block3control"} block with `ice speed`{:class="block3variables"} inside it.

```blocks3
when green flag clicked
set [ice speed v] to (3)
hide
go to x: (139) y: (-120)
repeat (6)
create clone of (myself v)
change y by (45)
end
+forever
wait (ice speed) seconds
end
```

## Step 2

Duplicate the `go to` block and the `repeat` loop.
Put the copies inside the `forever` loop.

```blocks3
forever
wait (ice speed) seconds
go to x: (139) y: (-120)
repeat (6)
create clone of (myself v)
change y by (45)
end
end
```

## Now run your code

Click the **Green Flag**.
Check that a new column of ice arrives every few seconds.
