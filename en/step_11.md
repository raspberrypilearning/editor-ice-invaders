## Set the ice speed

Store the ice speed in a variable.

![ice sprite](images/ice-sprite.png)

> ## Tip
>
> A **variable** stores a number that can change.

You're still working on the **ice sprite**.

## Step 1

Make a variable called `ice speed`{:class="block3variables"} for all sprites.

## Step 2

Add a `set ice speed to`{:class="block3variables"} block set to `3` at the top of the green flag script.

```blocks3
when green flag clicked
+set [ice speed v] to (3)
hide
go to x: (139) y: (-120)
```

## Step 3

Put the `ice speed`{:class="block3variables"} variable in the `wait`{:class="block3control"} block of the clone script.

```blocks3
when I start as a clone
forever
wait (ice speed) seconds
change x by (-50)
end
```

The ice moves at the same speed for now.
Try a different number in the `set` block to change it.
