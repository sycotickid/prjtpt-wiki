[[Journal]]

Notes from BotW:

Camera vertical movement is inverse

Camera has a ray cast that detects if the camera will obscure the player and it lerps the camera to the point before the ray collision smoothly.

  

Also, link’s target range for Guardians is massive! I wonder if targeting is different per enemy and their ranges are actually determined by a target radius attached to the enemy itself? Maybe you can both target each other if your target shapes intersect?

  

When beginning to move. There is a half second or so of slower movement that acts as kind of an anticipation. Link kind of ramping up to move

  

Notes from YT:

Flying enemies can use nav agent to navigate and a regular impulse / force to keep them in the air? Like a bouncing (impulse, fall, impulse, fall, etc)