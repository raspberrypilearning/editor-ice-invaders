## Place the puck

Put the puck in front of the stick.

![puck sprite](images/puck-sprite.png)

## Step 1

Click on the **puck sprite**.

Make the puck go to the stick.

```blocks3
when green flag clicked
go to (stick v)
```

## Step 2

Add a `point towards`{:class="block3motion"} block.

```blocks3
when green flag clicked
go to (stick v)
point towards (mouse-pointer v)
```

## Step 3

Add a `move steps`{:class="block3motion"} block.

```blocks3
when green flag clicked
go to (stick v)
point towards (mouse-pointer v)
move (130) steps
```

## Step 4

Put all three blocks inside a `repeat until`{:class="block3control"} loop with a `mouse down?`{:class="block3sensing"} block.

```blocks3
when green flag clicked
+repeat until <mouse down?>
go to (stick v)
point towards (mouse-pointer v)
move (130) steps
end
```

## Now run your code

Click the **Green Flag** and move the mouse.
Check that the puck stays in front of the stick as it turns.
