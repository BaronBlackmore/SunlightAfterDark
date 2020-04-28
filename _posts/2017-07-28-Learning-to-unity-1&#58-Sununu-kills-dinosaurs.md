---
layout: post
---
So, I've been learning Unity this year, in order to make the games of my dreams. With the help of some friends, and a whole ton of youtube tutorials, I got to work making the simplest game I could think of, an endless runner. If you're looking to start learning unity, I recommend [Games Plus James](https://www.youtube.com/user/gamesplusjames), his tutorials are simple and clear to follow.

After getting to grips with the interface, which was a bit overwhelming, I got to work on making sprites and concepts for the runner. And who would be a great running protagonist other than Sununu, the lovable scamp swinging fire at dinosaurs. 

[Prehestoric pixel art](/images/2017-07-28-Learning-to-unity-1&-58-Sununu-kills-dinosaurs.png)

![Run animation](/images/sununu-run.gif)

It's a one hit kill and you have to make it as far as possible, avoid the lava and get back to the future. Who's trying to stop you, but a swarm of dinosaurs controlled by your arch enemy Ben! 

![Character faces](/images/sununu-ben.png)

Unity is pretty good. if you're looking to make something simple or using common game mechanics, it takes care of a lot of things for you; things like gravity or collision detection. Though, most of the work needed to be done in code, and Unity works with C# and javascript. I chose to learn C# and will break down how that panned out in the next post. For now i'll just say it was hard. I needed to follow the tutorials meticulously, constantly repeating individual coding tasks in the tutorials up until the miraculous moment where it all just clicked.

I wrote scripts for two types of enemy, a passive and active one. As you run right they both move left, but when the pterodactyl sees you it dive bombs. Then I added in the oil mechanic: Killing dinosaurs adds to your oil-meter in the top left, which you can use up to boost. 

![Gameplay gif](/images/dinorun-1.gif)

It was fine to come up with neat mechanics, but the biggest challenge was one I had not considered: did it feel good to play? I spent days just trying to figure out how to make him jump in a satisfying way. The feeling of playing is so particular, the screen needs to move at a pace which isn't too slow/fast. The enemies hitboxes needed to feel fair/like a challenge. These difference in leaning too far one way or the other in any of these feels microscopic, and vary person to person. I can really appreciate how much work and playtesting must go into games that feel good to play, it sure isn't easy to get right.

The last addition was the cutscene. After playing for 10 seconds straight without dying, Ben shows up on a drone and you throw quips at each other. After the chat is over, semi-homing buzz-saw drones fly towards you. 

![Gameplay gif](/images/dinorun-2.gif)

Looking back, I remember how much of this had to be told to the program, nothing exists until you make it exist. Which platforms are generated next, the way the enemies turn red then disappear, what "jump" means...

