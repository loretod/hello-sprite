# Hello Sprite

## Welcome!
This 2 Minute Arcade tutorial will walk you through some of the most often used blocks when adding a sprite to your game.

## Predict
Take a look at the code and make a prediction on what you think this code does?

## Run
See if you were correct? Switch to the simulator tab and Press the **A** button. Was you're prediction correct?

## Investigate
Now... let's see what happens if you put the ``||sprites.create Sprite||`` at the bottom of the blocks?

**Add hint image here**

## Yikes!
Oh no! It seems that changing properties for a variable (in this case the sprite) we haven't loaded yet will throw an error.

Move the ``||sprites.create||`` block back to the top of the blocks.

## Modify
Time to change some things around. Play around with the some of the settings and see what happens.

-[] Click on the ''cat'' image and draw your own or select a different one from the library.  
-[] Change the x and y numbers in the velocity block.  
-[] Change the x and y numbers in the sprite position block.  
-[] Turn off the bounce off the wall option.  
-[] Turn off the stay on screen option.  
-[] Change what the sprite says and how long it he says it for.

## Make
Now it's your turn! From the ``||controller||`` menu, drag the ``||controller.on A Press||`` block and change the parameter to **B**.

Load a second sprite on the screen using your desired settings.

Press **B** to run your code.

```blocks
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
})

mySprite.setBounceOnWall(true)
mySprite.setStayInScreen(true)
mySprite.sayText(":)")
mySprite.setVelocity(50, 50)
mySprite.setPosition(0, 0)
let mySprite = sprites.create(img`
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    `, SpriteKind.Player)
```

## Recap
In this 2 Minute Arcade, we learned about how to load a sprite onto the game and adjust some of it's properties.

We also learned that it's pretty important to create the sprite variable ***first*** before beginning to change properties.

Nice!