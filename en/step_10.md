## Line up the ice

Repeat six blocks of ice in a line.

![ice sprite](images/ice-sprite.png)

## Step 1

Click on the **ice sprite**.

Add a green flag and set its `x` and `y` starting positions.

```blocks3
when green flag clicked
go to x: (139) y: (-120)
```

## Step 2

Add a `create clone of myself`{:class="block3control"} block and a `change y by`{:class="block3motion"} block set to `45`.

You may need to play with the number to suit your sprite.

```blocks3
when green flag clicked
go to x: (139) y: (-120)
+create clone of (myself v)
+change y by (45)
```

> ## Tip
>
> A **clone** is a copy of a sprite.

## Step 3

Put the two blocks inside a `repeat`{:class="block3control"} loop set to `6`.

```blocks3
when green flag clicked
go to x: (139) y: (-120)
+repeat (6)
create clone of (myself v)
change y by (45)
end
```

> ## Tip
>
> Experiment with the number in the `repeat`{:class="block3control"} loop to make a longer or shorter line of ice.

## Now run your code

Click the **Green Flag**. Check that a line of six blocks of ice appears.

![The blocks that make a column of six clones of the ice sprite.](images/step-10.gif){:width="450px"}
