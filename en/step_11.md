## Move the ice

Make the ice move towards the player.

![ice sprite](images/ice-sprite.png)

You're still working on the **ice sprite**.

## Step 1
Add a second script that moves each clone left every few seconds.

```blocks3
when I start as a clone
forever
wait (3) seconds
change x by (-50)
end
```

## Now run your code

Click the **Green Flag**.
Check that the ice steps to the left every three seconds.

![The column of ice steps to the left every three seconds.](images/step-11.gif){:width="450px"}
