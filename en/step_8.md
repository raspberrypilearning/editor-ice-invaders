## Make a column of ice

Make six pieces of ice in a line.

![ice sprite](images/ice-sprite.png)

> ## Tip
>
> A **clone** is a copy of a sprite.

## Step 1

Click on the **ice sprite**.

Add blocks to hide the ice and set its starting position.

```blocks3
when green flag clicked
hide
go to x: (139) y: (-120)
```

## Step 2

Add an empty `repeat`{:class="block3control"} loop set to `6`.

```blocks3
when green flag clicked
hide
go to x: (139) y: (-120)
+repeat (6)
end
```

## Step 3

Add a `create clone of myself`{:class="block3control"} block inside the loop.

```blocks3
when green flag clicked
hide
go to x: (139) y: (-120)
repeat (6)
+create clone of (myself v)
end
```

## Step 4

Add a `change y by`{:class="block3motion"} block set to `45`.

```blocks3
when green flag clicked
hide
go to x: (139) y: (-120)
repeat (6)
create clone of (myself v)
+change y by (45)
end
```

The clones appear in the next step.
