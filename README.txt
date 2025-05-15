UI:
The UI consists in a main canvas including all the widgets. The HUD blueprint acts as an interface between
the player character and the UI.

Dialogue System:
A DialogueActor was created with the hability to send a dialogues array to the player who, in time, displays
them in the UI.

Inventory System:
The Item Actors store a data struct (ItemData) with different variables needed along the system, such as
the icon to display in the inventory widget, and either they are a 3D item, also some data needed for the
3d items. When the player picks up an item, that data is sent to the player, and much like the dialogues 
system, the player sends that data along the UI in order to be displayed correctly.

Testing:
The game plays as a top-down Diablo-like game. A few items are located in the map (a glass statue and
a white pipe). When clicking on them, they must be collected and loaded in the inventory. The inventory
screen opens with the Esc key and closes either with Esc or the close button on the top right corner. The
inventory screen must display icons for the items collected and the icons must be able to be dragged and
dropped into the viewport slot. If the item is 3D, the viewport should display a 3D icon, able to be 
rotated with the mouse, else the same icon 2D will be displayed (in this test map the statue is set to be
a 3D item and the pipe a 2D item).
In the map there's also a dialogue actor (represented as a big blue box). When clicking on it its dialogues
must be displayed, letter by letter. Pressing the Space Bar, the current dialogue will finish displaying 
and when pressing it again the next dialogue will start displaying, if there is another one, else the 
dialogue screen will just close.