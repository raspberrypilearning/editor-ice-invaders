## Hide the sprite

The original ice block does not move. Hide this so only clones are visible.

![ice sprite](images/ice-sprite.png)

You're still working on the **ice sprite**.

## Step 1

Add a `hide`{:class="block3looks"} block under `go to x: y: `{:class="block3motion"}.

```blocks3
when green flag clicked
go to x: (139) y: (-120)
+hide
repeat (6)
create clone of (myself v)
change y by (45)
end
```

## Step 2

Add a `show`{:class="block3looks"} block under `when I start as a clone`{:class="block3control"}.

Each clone shows itself as it is made.

```blocks3
when I start as a clone
+show
forever
wait (3) seconds
change x by (-50)
end
```

## Now run your code

Click the **Green Flag**. Check that six blocks of ice move across the stage, with nothing left behind.

![The original sprite hides and the clones move across the stage.](images/step-12.gif){:width="450px"}
