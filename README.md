# character customiation game

![](https://i.imgur.com/PDR7Zxd.jpg)

## What you'll learn

-  Managing states and prop drilling (passing props)
-  Dynamic styles with template literals
-  Managing layers with `z-index`

### User Story

1. User sees a pre-selected avatar.
2. User sees lists of parts for body, clothing (3 layers), eyebrows, eyes, hair, and mouths. Note: Nose is pre-set as there is only one variation.
3. User can select a different part and the avatar will reflect the change when the user clicks on a different item.
4. App MUST be responsive.

### Optional Feature

1. User can choose hats and glasses as well.
2. User can click a `RANDOMIZE` button to generate a new character with random features.
3. Style the webpage to your heart's content!


### Working with layers
The avatar that we are going to make consists of several different layers: 
![](https://i.imgur.com/BNg5EYe.gif)

We know that the element in the layer above will cover the element in the layer below. For example, your glasses layer should be on top of your body layer, otherwise the body would cover the glasses and you wouldn't see the glasses.

Here's a general idea of which layer should be on top of which.

![](https://i.imgur.com/G4HfkZo.jpg)

You don't have to follow this reference. Use your own judgement to decide which layer to use and sometimes you can put several things on the same layer too!

On a web page, you can use the CSS property z-index (default 0) to represent the layer index. Note that you can only use this property with a positioned element (absolute, relative, fixed, sticky) or a flex child. The higher the number, the higher the layer. For example, an element with a z-index of 2 will sit on top of everything with a z-index of 1 or less.
