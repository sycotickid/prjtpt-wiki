#ode 

### Development:
- [[Demo Area]]
### Mechanics
- [[Controls]]

### Story
- [[Title Cinematic]]
- [[Opening Sequence]]
- [[Neo-Hylian]]

## To Do
```tasks
not done
path includes Dev/Ode to the Hyrule Fantasy/Journal
```

### Daily Notes
9/22/25 Notes:
Due to several factors, development is messy and unorganized. I need to step back and focus down on one aspect of the game at a time. I put character aside to work on environment. I know OttHF is too big of a project, so I need to stay organized or else nothing will ever get done.

9/23/25
- Zelda Godot Tutorial
- Quaternions
- Rollback project to earlier commit
- Revisit Trello board
- Focus solely on player mechanics

Tasks:

Basic locomotion
- [x] Walk (WASD/Control Stick)
- [x] Jump (Space/A)
- [x] Open Menu (Esc/Start)

Interact with ENV
- [x] Pick up items (Auto)
- [x] Interact (open [[Chests]]/door) (Space?/A)
- [x] Use bomb (RMB/ X)
- [ ] Climb (Auto)

Interact with NPC
- [x] Interact (start dialogue) (Space?/A)
- [x] Choose dialogue option (WASD/Control Stick)

Interact with [[Enemies]]
- [x] Health/Damage
- [x] Attack (LMB/ B)
- [x] Target (Ctrl/ L-Trigger)

- [ ] Make focused (not selected) target the one closest to the players center of vision, not the one closest to the player 
- [ ] Dodge (Side/Back jump)

Model & Animation
- [ ] Model & Texture
- [ ] Animations for all programmed actions
- [ ] Blend Poses
- [ ] SFX (Ambience, Player actions - footstep, attacking, jumping, etc, enemies, objects - pot breaking, grass cutting, sword hits - , etc

Environment Art
- [ ] Large ENV pieces (cliffs, trees, boulders)
- [ ] Small ENV pieces (stones, foliage (grass, bushes, etc), shells, etc)
- [ ] Buildings & items (bridges, pots, doors, walls, ruins, furniture (counters, tables, beds, chairs, etc)
- [ ] Dungeon pieces (locked doors, torches, pillars, etc)
- [ ] Terrain

Events & Game Management
- [ ] Look into events like “Kill all enemies in a room” and effects like dropping a rupee from above screen instead of spawning a treasure chest?

UI Polish

- [ ] Flesh out item get dialogue with image of the got item and a background glow card

Story
 - [ ] I want to add a basic character creator where you can choose your gender.

The opening scene has you seated on a small boat, hooded with your face hidden. The ferryman asks: “What’s your name lad?” To which you respond by pulling back your hood and entering the character creator. After confirming your character, if you picked to play as a girl, the ferryman will respond “oh, er, lass. Apologies, I couldn’t tell under the hood.” And continue his dialogue.

- I think it could be fun to reimagine [[Kokiri Forest]] as a test. Re-imagine the space with more realistic foliage and borders
- after we create the character and before we begin the environment/ level design
- Think about how to handle regions, levels and entities within separate regions

- I think it would be pretty easy and good practice to model a small treasure [[Chests]] and animate it opening and add it to the dialogue logic.

- Destructible can be a component added to environment assets with a type associated to it as a collision mask type of value - where you can select multiple options (explosive, arrow glass (ballon?), sword (grass and signs), magic (barriers or something?), etc) - maybe different damage types can trigger different effects? (Swords and bombs can destroy signs, but a sword would cut the sign in half and a bomb would blow the entire thing up). There can be an additional variable for a replacement mesh? Like a broken version of the mesh per destruction type?

I want to see how the sign cutting workings in OoT.

For environment / level design. We should think of props that we can include to add interactivity in the level:
- grass to cut
- rocks to throw
- torches to pick up
- etc

12/17/2025 Notes
For next year, I want to focus on reimplementing enemies and combat systems

Then I want to do an art pass, creating models and animations for everything I’ve added, culminating in a test level in [[Kokiri Forest]] with everything included

I also want to include music and sfx (I should look into FL Studio and try to practice with Kokiri Forest like music)

Create music that starts on the same night and has the same vibe, but is fundamentally different:

- Great Deku Tree’s theme
- Navi’s flight theme?
- Kokiri Forest theme
- House theme
- Shop theme
- Lost woods
- Legend of the goddesses theme

Ode II: The Adventuresome Quest

First Playtest To Dos
- Should take place in [[Eagle Rock]]
- Finish implementing Octoroks, Stalfos, and Tektites (basic models?)
- Implement a cooldown for sword swings (.2 seconds or something)
- Animate the swing card (super quick 3-4 frame animation) and explosion flare card (just star and fade out from the middle) (Look into potentially replacing the sword swing card with just a particle effect? Maybe in polish)
- Add original Zelda music (overworld & title, etc)
- Add face to link (card like the shield)

- Create chest open state to show that a chest has already been opened (display new visual)
- Spend a little time trying to make the skybox pretty? (Use a tutorial, follow Brush’s advice)
- Add tutorial pops triggered by inactivity (only if the action has never been done before) use a timer that gets removed once the action is done (to prevent resource draw)

- Create main menu to select different demo levels (maybe implement basic options menu) Play -> Cove, Forest, etc; Options -> Game, Video, Audio; Quit

- Create graybox level of the cove (this will have to be designed, but maybe should include an intro, explore, and conclusion?

- Animated raft sailing to the coast (implement basic in-game cutscene?)
- Exploration
- Dungeon entrance?
- Create graybox level of Kokiri Forest 
- Link’s house
- Sword and shield
- Deku tree

- Build it into an executable 
- Test with Amanda and some team mates?

After demo (polish & art)

- Add particles! Footsteps, sword swing, hit, block, emit projectile, item hitting the ground, item break/queue_free, item pickup
- Add SFX
- Add text crawl on dialogue boxes
- Add key word highlighting

For level / world design, look into real life reference for cliffs (Ireland & Oregon)

![[Forest of Maze Map.png]]

Misc ideas:

Old man in dungeon is a sage, a keeper of the triforce. He is imprisoned and when you free him, he rewards you with a hint. 

Triforce as an interactable, not a pick up.

Should automatically trigger cutscene where Link picks up Triforce piece (avoids awkward collision / interact questions)

Maybe this works by making it an auto intractable or maybe adding intractable logic to pick ups?

#### 2/26/26
*From Reminders*
- [ ] Model out props for demo
- [ ]  Create improved mannequin to animate (not final, but also not naked)
- [ ]  Draw out top down layout of [[Cove]] and surrounding area for modeling and gray box

### 4/20/2026
This page should be reorganized such that the newest entries are added at the top of the file and older entries get pushed lower and lower, staying at the bottom.

- [x] Consolidate all to-do items and keep a todo list at the top of the page ✅ 2026-04-20