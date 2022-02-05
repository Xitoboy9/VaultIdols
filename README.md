# VaultIdols
How to get your skin in (somewhat advanced)

First, get a copy of your skin's texture. Use something like NameMC for this. Then, go into the resource pack and under assets>the_vault>textures>item you can insert the skin file. Do the same under assets>minecraft>textures>item. That folder is for the vanilla items, in this case just the totem of undying.

Standard, the folder (assets>the_vault) is filled with 8 files: 4 textures and 4 mcmeta files. These textures are copies of my skin stacked on top of eachother and the mcmeta file basically tells it how to cycle through them. It can be hard to tell which vault god's totem you have, so having something like eyes blinking with their color can be useful. If you don't care about that, drop in 4 copies of your skin, and rename them to:

idol_benevolent

idol_malevolence

idol_omniscient

idol_timekeeper

(for easy copypasting, looking at you male- mane- mal- ugh)

Also, delete the mcmeta files if you don't care about animating them.

I would advise atleast somewhat changing the 4 copies, so you can see the difference. You can use online pixel art creators like PixilArt, or one of the many skin creators. Just change some color to the god's respective colors. For reference, here are their colors:

Benevolent: green

Malevolence: red

Omniscient: blue

Timekeeper: orange

Remember to do the same in the vanilla files! That one isn't animated for me, since I don't really have a use for vanilla totems, but you could animate it too. Just replace the filename with totem_of_undying instead of the idol names.

How to get your skin in, animated (advanced)

To animate your skin, use a pixelart editor like PixilArt (mentioned earlier), and change the canvas size to 64 pixels wide, and a certain amount of pixel high. The height is decided by the amount of "frames" you want. I chose 5. So the height becomes 64*5 = 320. Then, import the texture of your skin, and copy paste it however many time you want. Make your changes, and you're done.

Next, export all 4 of your stacked textures, and get them in the pack.

For the final step, it's on to those mcmeta files. Open them with any text editor and you'll be greeted by a .json file. There's 2 important things here:

First, the frametime. How many in-game ticks should be between each frame? 20 ticks is a second.

Second, is the frames. Here, you choose the order of the frames. Remember, the list starts at 0! So if you have 3 frames, you have frame 0, frame 1, and frame 2. Not frame 3! You can extend certain frames by repeating their number in the list, or remove frames entirely. I'd advise 0,1,2,3,2,1. Note the last 0 is not there. Since after the last 1, it loops to the beginning which is 0 already. Putting it their doubles it up. That example of numbers is based on 4 frames.

You can do the same step for the vanilla texture of a totem of undying.
