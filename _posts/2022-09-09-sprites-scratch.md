---
title: Sprites
author: Nikky Leone
date: 2022-09-09 20:55:00 +0800
categories: [Year 7, Microbits]
tags: [sprites]
---

**In computer graphics, a sprite is a two-dimensional bitmap that is part of a larger scene (e.g., a 2D video game). Sprites can be static images or animated graphics.**

**Sprites were the standard way to integrate graphics into video games in the 1980s and 1990s. Every character and object in the game was represented by a sprite that the game’s designer created.** In modern times, 2D sprites have been replaced by 3D polygons because of the superior graphics rendering power that is available.

**Sprites are also used to represent icons as part of a user interface.**

# Scratch

**Every Scratch program is made up of sprites and the scripts (instructions) that control them. Scripts are programmed to make the sprites do things.**  Sprites can be made to **move around, change their appearance, react when they touch things, and be controlled by the player.** Sprites can also be programmed **to talk in speech bubbles and play sounds and music.** A project can have lots of sprites, and each sprite can have lots of scripts. **Games are more exciting when there are more sprites to hit, dodge, or chase each other.**

# Bonus: creating a sprite in Python

**Now we’re ready to make our first sprite. In `Pygame`, sprites are objects. If you haven’t worked with objects in Python before, they are a convenient way of grouping data and code into a single entity.** It may be a little confusing at first, but fortunately, Pygame sprites are a good way to practice with objects and get used to how they work.

We start by defining our new sprite:

```python
class Player(pygame.sprite.Sprite):
```
 
**class tells Python we’re defining a new object, which is going to be our player sprite, and its type is `pygame.sprite.Sprite`, which means it will be based on `Pygame`’s pre-defined Sprite class.**

**The first bit of code we need in a class definition, is the special `__init__()` function, which defines what code will run whenever a new object of this type is created.** There are also two properties that every Pygame sprite must have: an image and a rect:

```python
class Player(pygame.sprite.Sprite):
    def __init__(self):
        pygame.sprite.Sprite.__init__(self)
        self.image = pygame.Surface((50, 50))
        self.image.fill(GREEN)
        self.rect = self.image.get_rect()
``` 
 
**The first line, `pygame.sprite.Sprite.__init__(self)` is required by `Pygame`** - it runs the built-in `Sprite` classes initializer. **Next, we define the image property - in this case, we’re just creating a simple 50 x 50 square and filling it with the color `GREEN`.** in a future post we’ll learn how to make the sprite’s image be something fancier, like a character or spaceship, but a solid square is good enough for now. **To move a sprite, we can use `x, y, z` coordinates that are implemented in Python.**

> You don't have to know everything that I mentioned in this post, understanding the concept of sprites is our goal. :)
{: .prompt-tip }




