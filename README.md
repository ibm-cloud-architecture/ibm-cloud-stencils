# IBM Cloud Visio Icons

## Visio Icon Conversion (vssx folder)

Conversion of IBM Cloud Icons from pptx to vssx for Visio 2013 and later.  
TODO: Need to determine whether to provide vss files for Visio 2003-2013.  

### Icons

The proposed icons in Visio that are different from other tools are shown below.  

This includes additional icons and some redesigns from VPC design team experiences (original and redesign are both available).  The redesigned icons are Firewall (Security), Gateway (Security), Load Balancer (IaaS), and VPN (IaaS and Security).  

Icons pulled in from bluemix portal or elsewhere can contain color which may not look good when placed on top of the IaaS green in the IBM Cloud Icons.  Therefore some icons are black-and-whited or similar process to make the icons look good with the rest of the IBM Cloud Icons. A new icon can also be created from scratch if needed.

![Icons](/images/icons.png)

### Groups

The proposed groups in Visio are shown below.

The existing 3-section rectangle is accomplished with Cloud Universe + IBM Cloud + Other Networks in order to take advantage of containers for Visio power users and to bridge the former with the new containers.

The user has a choice of the outermost container being Cloud Universe or IBM Cloud or VPC.  Each group is provided as either a container or non-container.  The provided logos can be added to the border if desired or the provided group name can be used or deleted to reclaim space.  The groups have initial sizes that vary to allow an inner group to be dropped on top of an outer group.  

![Groups](/images/groups.png)

## Visio Diagram Templates (vstx folder)

Template files are in the process of being converted to Visio from other tools including reference architectures from the client success team.  Also working with draw.io support to fix problems with the export of draw.io templates to Visio. 

## User Guide

### Legends

![Legends](/images/legends.png)


### Color Scheme

| Color | RGB | Hex | Description |
| :--- | :--- | :--- | :--- |
| Blue | 67, 120, 187 | 4378BB | Outer containers, text, and lines |
| Red | 255, 0, 0 | FF0000 | Security containers and groups |
| Green | 0, 136, 43 | 00882B | Non-security groups |
| Yellow | 237, 193, 28 | EDC11C | Alternative for lines |
| IaaS Green | 141, 197, 63 | 8DC53F | IaaS icons |

### Group Steps
1. Drag and drop the desired group/container from the groups onto the canvas.
2. Select a single name from the provided list in the region and zone or replace with another name.
3. Optionally delete any group/container name that is not desired to save vertical space.
4. Optionally add the provided logo icons on a border or inside the respective group/container for IBM Cloud, Virtual Private Cloud, and Network ACL.  
5. Before a group can be placed over multiple containers the containers must be locked under FORMAT then unlocked after the group has been placed.

### Icon Steps
1. Drag icon from stencil to canvas.  Note that the master name is not automatically included with the icon on the canvas.
2. If an icon does not go exactly where you want it (e.g. Visio tries to align the icon with other icons on the canvas), go to Snap & Glue and uncheck Snap and Glue, put the icon where you want it, then go back and recheck Snap and Glue if you prefer to have it turned on.  If you don't have Snap & Glue in the Quick Access Toolbar at the top of Visio, go to File -> Options -> Quick Access Toolbar, search All Commands and add Snap & Glue to the Quick Access Toolbar.
3. To add text to an icon on the canvas, select the icon and type the desired text.
4. Resize text to Calibri 10 pt if desired to fit more text than Calibri 12 pt.
5. Change text to blue color if desired.  
6. If a line obstructs the text, select text, right-click and select Font, go to Text Block, and select solid color of white for text background.
7. If any of the text wraps to next line, select text, select Text Block (Shift+Ctrl+4) under Connection Point under HOME, widen text box and move widened text box to be in the center under icon. 
8. If subscript or superscript of the text or parts of the text is desired, highlight the desired text and press CTRL+= to make the highlighted text subscript or CTRL+SHIFT+= to make the highlighted text superscript. 
9. Add lines between desired objects either object-to-object by clicking inside the objects or point-to-point by clicking on existing points on the border of the objects or add additional points to the objects as desired.  Change line color to blue and weight to 3 pt to allow the lines to standout from the groups.  Note that when objects are moved the shape-to-shape will automatically reorganize where the line attaches to the objects and point-to-point will always maintain the line at each point.

## Examples

Notes:
1. The public gateway needs to be instantiated in each zone and can be attached to one or more subnets.


### 3-Tier Multizone Security Group 

![3-TierMultizoneSG](/images/MultizoneSG.png)

### Existing Hybrid Example Using Containers

![Hybrid](/images/Hybrid1.png)


