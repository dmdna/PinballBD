# Pinball

By: Benjamin Blas Maristany, Diego Medina Molina

## Overview

Pinball is a classic and timeless table game. We have made a simple version in Unreal Engine 5 to demonstrate physics interactions within both world objects and backend data like player score. We have multiple paddles, bumpers, and speed panels that showcase a wide range of physics interactions.

## Physics Interactions

We have included several physics interactions in our project.

Firstly, we have included some bumpers that launch the ball at certain velocities, allowing for added momentum to keep the pinball going. This naturally adds the possible interaction of being launched into another bumper, which brings about that classic pinball feel.

We also added some speed panels, where the ball will receive an added force in the direction the arrows are pointing at. This will give a ball a "nudge" effect as it is travelling through the table. This will naturally increase the ball's speed in one direction, which will also slow it down if it happens to be travelling in the other direction.

On top of that, we included an orange frictionless pad that slightly modifies the ball's behavior, which will hopefully add a touch of surprise for the player in terms of how they expect the ball to move.

Lastly, we inserted a ball resizer hut. When the ball ends up inside this rainbow structure, the ball's size changes to a random size within reasonable scale.

## Effects

We have added simple effects that appear when the physics of the ball are changing.

When a bumper is hit, it will show a simple particle explosion, indicating that the ball is receiving an impulse by hitting it. The bumper itself is also animated to showcase this physics interaction.

When the resizer is activated, another particle effect will be temporarily activated. As it is a rainbow hut, multicolored streams of energy will spew from the top.

## Player Input

There are 3 simple controls:
1. The left and right paddles are controlled by pressing the **Left and Right Arrow Keys**, respectively. The additional paddle on the top right is also controlled by the right arrow key.
2. The ball launcher is controlled by pressing and holding the **Bottom Arrow Key** to charge the plunger and later releasing it to launch.

## Scoring

To show how physics interactions can interact with backend game data, we have added a simple scoring system displayed by a number on the player's HUD.

- Hit a Big Bumper = 100 points
- Hit a Small Bumper = 500 points
- Hit a Golden Bumper = 1250 points
- Activate the Ball Resizer = 3000 points

The game will also track the player's High Score during their play session, incentivizing them to keep playing to keep getting the highest score possible. When a ball is reset, the score resets as well, but the high score will be updated if the player just surpassed it this round.

## Resources

Everything we used for this project was either part of or derived from the default assets provided by Unreal Engine 5. This includes Static Meshes, Materials, Particle Effects