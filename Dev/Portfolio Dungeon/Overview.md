Portfolio Dungeon is a Zelda-style dungeon made up of five rectangular rooms that represent pages on a website ([javiergonzalez.dev](https://javiergonzalez.dev)). Each room should roughly take up the width and height of the viewport. This can be achieved either by scaling the size of the room to the viewport or implementing a zoom in feature that prevents the screen from bleeding over the edge of a room, either by zooming in or otherwise constraining the camera

### Timeline

#### Phase One - Information Dungeon
When someone first visits the website, a graphic akin to the original Legend of Zelda title screen can display as the loading screen: 

The Legend of Javier
A Link to the Portfolio
-)============>

Loading... => Start

On start, display dungeon with UI elements for hearts, coins (rupees), two item slots (sword and blank) and a mini-map? (A tooltip on the top left / right corner can remind the player "Press Esc to open the menu").
> Explore icone.js game icons for UI assets

Pressing Esc can display a small menu for configuring the game or shortcuts?
Resume
Pages
- About
- Portfolio
- Contact
- Home (greyed out until you complete the secret dungeon)
Settings
Exit

##### Character:
Moves with WASD (and / or Arrow Keys)
Interacts with E (to talk with NPC, pick up objects, activate levers, etc)
LMB to use first item (sword)
RMB to use second item (bombs)
Shift to roll?
Esc to pause

##### Animations:
1. Walk
2. Attack
3. Push
4. Open container
5. Roll
6. Wave / Talk
7. Hurt
8. Die
9. Item Get
10. Throw
11. Pickup
12. Idle

##### Map:
Center -> Landing page
> Mostly empty room lit by a sky spot light with a grate texture, so it looks like we are under a grate. Doors leading north, east and west with a cracked wall on the southern wall (or a closed door that requires a level?)
> UI elements: Javier Gonzalez | Software Engineer
> Title and subtitle can fade in on load and fade out when the player moves, fading back in when the player stops moving? (Maybe it is always there or engraved onto the floor?)

North -> Portfolio
> Houses paintings with plaques that detail each project. How would linking to the project work? I want it to be diegetic and intuitive. Maybe for portals a la Minish Cap or ALttP. Before we have projects to add to the room, we can have a construction character stand in the room and complain about how I haven't accomplished enough yet?

East -> Contact
> A room with a desk containing a paper and quill that deposits a contact form on interact. (On submit, the player can do an animation of folding the form and putting it into a mail slot?) There can also be  pickup-able buttons that display social media icons that can be thrown to visit the link? How can this be communicated effectively and un-intrusively?

West -> About
> On enter, the room can have an old man who will talk about me when spoken to (or maybe when you enter the room). // Insert self-glorifying copy here
> Maybe if you speak to him multiple times, he gives you a key to a room where the level for the southern door is? Or maybe there's a chest in the corner (or behind a puzzle) with the key.

South -> Secret Dungeon Entrance
> For Phase One, the southern room can just be a playground containing some monsters and / or a puzzle.

#### Phase Two - Secret Dungeon
The southern room, only accessible via bomb or level, is the start of the dungeon (to be designed) which can involve fighting monsters, solving puzzles and defeating a boss to gain access to a secret area (and enable the "Home" button on the menu).

Browser cookies can be used to store save data so a user can continue the dungeon on subsequent visits.
Items:
- Bow and Arrow (or Bombs if not already obtained in the Info Dungeon)
- Dungeon Map
- Compass
- Boss Key

When the player defeats the boss, the receive the Triforce and a thank you message (maybe a shortcut portal appears to the contact page?)

#### Phase Three - Escaping the Dungeon
After defeating the boss of the Secret Dungeon, a path can open up to the overworld where they can explore a small map with a village and wilderness area? This could be where the Home button takes you, after unlocking it?

Ideas can be incorporated to show other interests?
- Crafting (Minecraft)
- Farming (Stardew Valley)
- Survival (Don't Starve)
- City Building (Banished)
- etc