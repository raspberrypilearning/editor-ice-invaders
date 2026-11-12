## Bounce off the walls

Keep the puck on the screen.

![puck sprite](images/puck-sprite.png)

You're still working on the **puck sprite**.

Add an `if on edge, bounce`{:class="block3motion"} block inside the `forever`{:class="block3control"} loop.

```blocks3
when green flag clicked
repeat until <mouse down?>
go to (stick v)
point towards (mouse-pointer v)
move (130) steps
end
wait until <not <mouse down?>>
forever
move (12) steps
+if on edge, bounce
end
```

## Now run your code

Click the **Green Flag** and fire the puck.
Check that the puck bounces off the edges.
