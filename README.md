# Ex No :04

# <p align="center">  Attach Rifle with character mesh and implementation bullet spawn from Rifle </p>

## Aim:
To attach Rifle with character mesh and implementation bullet spawn from Rifle 
## Software Required:
Unreal Engine.

## Procedure:
To attach a rifle to the character mesh and implement bullet spawn from the rifle in Unreal Engine, you can follow these steps:

### Import the Rifle Mesh:

In Unreal Engine, go to the Content Browser and find or import the rifle mesh you want to use.
Import the rifle mesh into your project by dragging and dropping it into the desired folder.

### Set up the Rifle Socket:

Open the character mesh Blueprint you are using.
Inside the Blueprint, locate the socket on the character's hand where the rifle will be attached. This may vary depending on the character's skeletal mesh and setup.
Add a socket to the desired location on the character's hand bone. Name the socket appropriately, such as "RifleSocket".

### Attach the Rifle to the Character Mesh:

In the character mesh Blueprint, go to the Event Graph.
Create an Event Begin Play node by right-clicking in the graph and searching for "Event Begin Play."
Drag and drop the rifle mesh from the Content Browser into the Blueprint graph.
Right-click on the rifle mesh node and choose "Create a Reference to Mesh."
Connect the output execution pin of the Event Begin Play node to the input execution pin of the rifle mesh node.
Add a "Attach to Component" node and connect it to the output execution pin of the Event Begin Play node.
Connect the output pin of the rifle mesh reference node to the input pin of the Attach to Component node.
In the Attach to Component node, specify the character mesh as the Parent and the RifleSocket as the Socket Name.

### Implement Bullet Spawn:

Create a new Blueprint class based on the Actor class and name it "Bullet" or any desired name.
Inside the Bullet Blueprint, add a static mesh component to represent the bullet's visual.
Implement logic to handle the bullet's behavior, such as movement and collision detection.
In the character mesh Blueprint, go to the Event Graph.
Create an Input Action node to trigger the bullet spawn, e.g., "Fire" or "Shoot."
Add a Spawn Actor from Class node and connect it to the output execution pin of the Input Action node.
Choose the Bullet class as the class to spawn and specify the location and rotation for the spawn.
Connect the output execution pin of the Spawn Actor from Class node to the input execution pin of the rifle mesh node to make the bullet spawn from the rifle.

### Adjust Rifle and Bullet Properties:

You can further customize the rifle and bullet properties, such as adding sound effects, particle effects, or adjusting their movement and collision settings.
Modify the rifle mesh's transform to position it correctly in the character's hand.
Adjust the bullet's speed, scale, and any other visual or behavioral aspects to suit your needs.
Remember to save and compile your Blueprints after making changes. Test the character to ensure the rifle is properly attached and that bullets spawn from the rifle when the fire action is triggered. You can also add additional functionality, like reloading or weapon switching, based on your game design.

## Output:
## Gun:
![pic1](https://github.com/durga46/Ex3.Game-programming/assets/75235704/587afc33-e65a-40a3-bc14-4aa573709130)

## GunActor:
![pic2](https://github.com/durga46/Ex3.Game-programming/assets/75235704/c64390fa-1f85-44b3-b23c-44328cc221fd)

## Gun in Hand:
![pic3](https://github.com/durga46/Ex3.Game-programming/assets/75235704/b383850b-8676-4c23-bced-251f9dc6b10e)



## Result:

Thus,attach Rifle with character mesh and implementation bullet spawn from Rifle done successfully in Unreal Engine





