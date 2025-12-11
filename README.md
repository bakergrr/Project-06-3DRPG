# Project-06

# Features added
- Light system and hacking:
  - Throughout the level are spot lights which cast light in a clearly-defined circle. While enemies stand in these lights, their vision radius (represented by the red light each enemy casts towards the ground) increases dramatically. The player can "hack" a light by pointing their camera at it and holding the right-click button. A line will appear between the player's "phone" (displayed during the hacking animation) and the light, and after 3 seconds of hacking, it will be "hacked". Hacked lights are purple and cast a darker purple circle that does not increase enemy vision. After enough time, the light will return to normal.
- Enemy AI: (does this count, since it's fairly advanced?)
  - Enemies walk back and forth between two predetermined points, casting a small red circle around them to indicate their vision radius. The vision radius is barely wider than the enemy at first, but expands drastically when the enemy is under a light. If a player enters the enemy's vision radius, it will play an animation where it points at the player before running at them much more quickly than its default pacing speed. If the player can stay far enough away from it or hide using terrain (the enemies can't see the player through walls to chase after it), the enemy will "forgive" the player and return to its pedetermined route. If an enemy collides with a player, the player is teleported back to the beginning, the game resets. All enemies return to their original positions, all lights lose any hacking progress, all pick-ups reappear, and the time and score are reset.
- Scoring system: (this isn't an additional feature, but I wanted to explain how it worked):
  - Scattered throughout the level are wallets, purses, and briefcases that the player can pick up to gain points. Each model gives a different amount of score, and they're placed in locations to reward risky or more difficult maneuvers. As the player explores, a timer counts down from 5 minutes. At the end of the level, the player gains score equal to their time in seconds, which is combined with any score from pick-ups to create their total.
- Some small aesthetic touches that might count for a point if the enemy AI doesn't:
 - When a player hacks a light, the model, spot light, and line from the phone to the light all change color from white to purple to signify progress. As the light returns to normal, it slowly changes back from purple to white.
 - Holding right-click (the button used for hacking) creates a phone-shaped reticle on the screen to help with aim. The player can aim their hacking near the light and still hack it (mechanically, there's a much larger collider that the hacking raycast can hit, but the visible line is still drawn straight to the light orb, so it looks like aim assist or the player's hacking snapping to the light).
 - When gaining score, an additional textbox appears that shows the amount of points gained before slowly fading away.
 - When an enemy walks into or out of light, the red light that shows their vision radius gradually expands or contracts instead of snapping to the new vision radius.
 - To make the transition to the beginning of the level slightly less jarring after the player is hit by an enemy, their model will flicker briefly.
 - Text on the win screen appears in chunks over time, slowly revealing the final score.
 - Painting models on the walls makes the level feel a liiiittle bit more like the art museum it's meant to be? Some are placed slightly askew to convey a more humorous tone.

# References to resources used in the project
Jackie and Exo Red models, Jackie texting, Exo Red walking, pointing, idle, waving animations from [mixamo.com](https://www.mixamo.com/#/)

Phone by Quaternius (https://poly.pizza/m/k2kgBepoMU)

Wallet by Poly by Google [CC-BY] (https://creativecommons.org/licenses/by/3.0/) via Poly Pizza (https://poly.pizza/m/bN7GPQFma7_)
Briefcase by Poly by Google [CC-BY] (https://creativecommons.org/licenses/by/3.0/) via Poly Pizza (https://poly.pizza/m/cKZ9BZNK1JE)
Purse by jeremy [CC-BY] (https://creativecommons.org/licenses/by/3.0/) via Poly Pizza (https://poly.pizza/m/2dTPEuZyLyJ)

Wall painting by jeremy [CC-BY] (https://creativecommons.org/licenses/by/3.0/) via Poly Pizza (https://poly.pizza/m/62zn39CRkbG)
Painting by Jonathan Granskog [CC-BY] (https://creativecommons.org/licenses/by/3.0/) via Poly Pizza (https://poly.pizza/m/fWqUmeGBc-L)
Wall Art 06 by Jarlan Perez [CC-BY] (https://creativecommons.org/licenses/by/3.0/) via Poly Pizza (https://poly.pizza/m/1U5roiXQZAM)

Classy Art Deco Wallpaper and Laminate Wood Flooring Brown textures from freepbr.com

# Created by
Graham Baker

(I know that the Exo Red model doesn't really look like a robot? I'm hoping it'll pass as something closer to a cyborg or one of those uncanny-valley robot faces, but this was the closest thing that I could find to a robot on Mixamo.)
