# VRC-Avatar-PVP
An optimized easy to edit World based Avatar PVP system


--Setup--
install the Layer and Collision setup
Under tools click on it
go to a game object to see if the layers have been created

install the Avatar PVP
add the prefab to your scene
set the respawn point in the PVP manager
done!

all the defalts work fine

--Refreced Prefabs--
the anchor is just an empty game object that spawns per bone (Legs Arms Chest Head) and and gets re proportioned
this is done so theres only 10 objects having there position updated no matter how many layers are configured
half of the anchors get there position updated each frame

the coliders prefabs have been set up to ignore colision with they Colider Layer by setting the Collision Override on the colider set to Everything
this stops the coliders from collision testing everything killing performance
yet Particals can still colide
any mesh can be used as a colider but the more polygons the more performance it eats when you get hit

the Downed VRC station is a chair with a downed animation that when the player gets downed gets teleported to the players location and on the next frame the player is forced into it
Note if your in a chair and you get downed your tracking breaks due to how anomalous the VRC station script is
(you can't eject player from all chairs only referenced ones)

--Zone Prefabs--
the fire zone fires tics on an interval on the fire layer (31)

the water zone makes player immune from fire (31) and cancels effect on that layer
