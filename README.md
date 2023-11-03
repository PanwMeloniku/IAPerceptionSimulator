# IAPerceptionSim

Its a small project, aimed at implementation of behaviors corresponding to AI (Artyficial Inteligence) perception system.

Main goals of project are to make AI able to:
* detect objects and characters nearby and interact with them
* recive sounds information from neighbourhood and try to locate thing which generate such sound
* stop current activity in some cases like threatening situation

Project developed with Unreal Engine 5



Last changes:
* New area where NPC (NonePlayerCharacter) can move [NavMeshBoundsVolume] has been added. 
* AI now can detect player
* AI start chasing player after detecting him
* When player vanish from AI view range for at least 5 second, AI will no longer chase player, instead It will go back wandering
* Behaviors of AI are no longer In main Character Class. All behaviors scripts has been moved to [Behavior_Tree]
* Animation 2d BlendSpace for walk to run has been added

Future changes:
* Item class will be created. It will have properties of object characteristics and avaible interaction options
* Equipment class will be created. It will allow AI to store Items.
* AI will be able to detect nearby items and make simple interactions with them (like add to equipment)
