## Make new lines of ice

Make a new column of ice every few seconds.

![ice sprite](images/ice-sprite.png){:width="80px"}

You're still working on the **ice sprite**.

## Step 1

Put the `repeat`{:class="block3control"} loop inside a `forever`{:class="block3control"} loop.

```blocks3
when green flag clicked
hide
set [ice speed v] to (3)
go to x: (139) y: (-120)
+forever
repeat (6)
create clone of (myself v)
change y by (45)
end
+end
```

## Step 2

Add a `go to x: y:`{:class="block3motion"} block and a `wait`{:class="block3control"} block with `ice speed`{:class="block3variables"} to the bottom of the `forever`{:class="block3control"} loop.

```blocks3
when green flag clicked
hide
set [ice speed v] to (3)
go to x: (139) y: (-120)
forever
repeat (6)
create clone of (myself v)
change y by (45)
end
+go to x: (139) y: (-120)
+wait (ice speed) seconds
end
```

## Now run your code

Click the **Green Flag**. Check that a new column of **ice** arrives every few seconds.

![A new column of ice arrives every few seconds.](images/step-15.gif){:width="450px"}
