# IBM Cloud Visio Stencils and Templates

## User Guide

### Legend

![Legend](/images/legend.png)

### Colors

![Colors](/images/colors.png

### Install

1. Create a stencils folder: My Documents \ My Shapes \ IBM_Cloud_Visio_Stencils
2. Copy the Stencils (vssx files) from the GitHub Stencils folder or zip to this folder.
3. Create a templates folder: My Documents \ My Shapes \ IBM_Cloud_Visio_Stencils\Templates 
4. Copy the Templates (vstx files) from the GitHub Templates folder or zip to this folder.

### Setup
1. Select one of the teamplate files to bring up a fully editable diagram in Visio.
2. Delete any icons and connecting lines that are not needed. 
3. Go to More Shapes to the folder you created and select the stencils that you want to use in your diagrams.

 
### Containers and Groups
1. Drag and drop the desired group/container from the groups onto the canvas.
2. Select a single name from the provided list in the region and zone or replace with another name.
3. Optionally delete any group/container name that is not desired to save vertical space.
4. Optionally add the provided logo icons on a border or inside the respective group/container for IBM Cloud, Virtual Private Cloud, and Network ACL.  
5. Before a group can be placed over multiple containers the containers must be locked under FORMAT then unlocked after the group has been placed.

### Icons
1. Drag icon from stencil to canvas.  Note that the master name is not automatically included with the icon on the canvas.
2. If an icon does not go exactly where you want it (e.g. Visio tries to align the icon with other icons on the canvas), go to Snap & Glue and uncheck Snap and Glue, put the icon where you want it, then go back and recheck Snap and Glue if you prefer to have it turned on.  If you don't have Snap & Glue in the Quick Access Toolbar at the top of Visio, go to File -> Options -> Quick Access Toolbar, search All Commands and add Snap & Glue to the Quick Access Toolbar.
3. To add text to an icon on the canvas, select the icon and type the desired text.
4. Resize text to Calibri 10 pt if desired to fit more text than Calibri 12 pt.
5. Change text to blue color if desired.  
6. If a line obstructs the text, select text, right-click and select Font, go to Text Block, and select solid color of white for text background.
7. If any of the text wraps to next line, select text, select Text Block (Shift+Ctrl+4) under Connection Point under HOME, widen text box and move widened text box to be in the center under icon.  While in Text Block mode you can also move the text to other sides of the icon out of the way of lines as desired.  
8. If subscript or superscript of the text or parts of the text is desired, highlight the desired text and press CTRL+= to make the highlighted text subscript or CTRL+SHIFT+= to make the highlighted text superscript. 
9. Add lines between desired objects either object-to-object by clicking inside the objects or point-to-point by clicking on existing points on the border of the objects or add additional points to the objects as desired.  Change line color to blue and weight to 3 pt to allow the lines to standout from the groups.  Note that when objects are moved the shape-to-shape will automatically reorganize where the line attaches to the objects and point-to-point will always maintain the line at each point.

## Examples

Notes:
1. The public gateway needs to be instantiated in each zone and can be attached to one or more subnets.


### VPC with Single Zone Security Groups

![VPCwithSinglezoneSG](/images/VPCwithSinglezoneSG.png)

### VPC with Multi Zone Security Groups

![VPCwithMultizoneSG](/images/VPCwithMultizoneSG.png)

### VPC with Classic Network

![VPCwithClassicNetwork](/images/VPCwithClassicNetwork.png)

### Existing Hybrid Example Using Containers

![Hybrid](/images/Hybrid1.png)


