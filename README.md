# MG3
## Devlog

1. The default value for floats is 0. The default value for ints are also 0. The default values for bools are false. The default value for strings is an empty string.

2. The Update method gets called in the code automatically and does not need to be called manually. The Update method gets called once every frame.

3. KickWeapon is able to use the timer by checking each frame to see if the time has run out. The variable _lifetimeSeconds, stores the amount of time the kick should last which is 0.2 seconds. The method defined in Timer.cs named BeginTimer, stores that _lifetimeSeconds value into a variable used to track the time. This variable's value reduces as time goes on with each frame through the Update method in Timer.cs using Time.deltaTime. Using the Update method in KickWeapon.cs, which runs every frame, the IsFinished method is run which is defined in Timer.cs which checks if the time left is less than or equal to 0. If it is less than or equal to 0, the kick will go away.


## Open-Source assets
- [Cat fighter spritesheet](https://opengameart.org/content/cat-fighter-sprite-sheet)
- [Food sprites](https://rcpstd.itch.io/pixel-food-pack)