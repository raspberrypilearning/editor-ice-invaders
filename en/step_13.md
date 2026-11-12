## Make new lines of ice

Make a new column of ice every few seconds.

![ice sprite](images/ice-sprite.png)

You're still working on the **ice sprite**.

## Step 1

The waiting time is needed in two places now, so store it in a variable.

Make a variable called `ice speed`{:class="block3variables"} for all sprites.

> ## Tip
>
> A **variable** stores a number that can change.

## Step 2

Add a `set ice speed to`{:class="block3variables"} block set to `3` at the top of the green flag script.

```blocks3
when green flag clicked
+set [ice speed v] to (3)
hide
go to x: (139) y: (-120)
repeat (6)
create clone of (myself v)
change y by (45)
end
```

## Step 3

Drag the `ice speed`{:class="block3variables"} variable into the `wait`{:class="block3control"} block of the clone script.

```blocks3
when I start as a clone
show
forever
wait (ice speed) seconds
change x by (-50)
end
```

## Step 4

Add a `forever`{:class="block3control"} loop to the end of the green flag script.

Add a `wait`{:class="block3control"} block with `ice speed`{:class="block3variables"} inside it.

```blocks3
repeat (6)
create clone of (myself v)
change y by (45)
end
+forever
wait (ice speed) seconds
end
```

## Step 5

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

Change the number in the `set` block to speed the ice up or slow it down.

![A new column of ice arrives every few seconds.](images/step-13.gif){:width="450px"}
