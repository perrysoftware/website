---
title: "Hexmesh"
date: 2020-07-13
draft: false
tags: ["Unity", "iOS"]
---

{{< figure src="/hex.png" alt="App Icon" width="200" >}}

Hexmesh Duo is the most recent game that I have created. It has currently been put on hold for other projects. My goal with this game was to expand my reach with Unity into a 3D game because all of my previous games are 2D. Most of the skills I had learned from previous projects were transferrable; however, there were a few key differences.

One of the biggest changes was creating 3D objects. A good portion of my UI is built into the game board. I had to create these in Blender and import them into Unity. Obviously, the positioning system was a big change as I had to place the blocks on 3 axes instead of 2. Colliders were 3D as well which did not involve much work on my end, but it is still important.

The most challenging part of building this game was the block spawner. The game board has 9 rows, and this was my focus. I kept track of the first block in each row so I would know what color was sitting there. All other blocks were kept in a list specific to that row. When a certain row is selected, it checks the block color currently there to the one it wants to spawn. If it is the same, it stacks the blocks; otherwise, it will push the block out. When the blocks are destroyed, they are removed from their rows and placed back into the list of blocks available to be spawned in.

One of the key changes I wanted to make after developing Spinny Spot was to make the levels the same each time you played. In Spinny Spot, each level had the same enemies and spawn rate, but the order was always random. This made for some frustrating moments that would trap players. My solution to this problem was to let the spawner run for a long time at a high speed, and I captured all the data in a text file. I then copies bits of this data to use for each level. It would go through the array of newly found spawning information to find the location and color of each block to spawn. This allowed each level to remain consistent without me having to write out each individual spawn.
