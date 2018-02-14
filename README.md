# IBM Cloud Visio Icons

## Legends

![Legends](/images/legends.png)

## 3-Tier Example

![3-Tier](/images/3-tier.png)

## Multizone Example

![Multizone](/images/Multizone.png)

## Hybrid Example

![Hybrid](/images/Hybrid1.png)

## Visio Icon Conversion (vssx folder)

Conversion of IBM Cloud Icons from pptx to vssx for Visio 2013 and later.  Thisvversion contains additional IaaS icons plus the new IaaS containers.  Note that VPC will be removed from the published version until VPC is announced.  Need to determine whether to provide vss files for Visio 2003-2013.  

## Visio Diagram Templates (vstx folder)

Template files are in the process of being converted to Visio from other tools including reference architectures from the client success team.  Also working with draw.io support to fix problems with the export of draw.io templates to Visio. 

## User Guide

### Color Scheme

| Color | RGB | Hex | Description |
| --- | --- | --- | --- |
| Blue | 67, 120, 187 | 4378BB | Outer containers, text, and lines |
| Red | 255, 0, 0 | FF0000 | Security containers and groups |
| Green | 0, 136, 43 | 00882B | Non-security groups |
| Yellow | 237, 193, 28 | EDC11C | Alternative for lines |
| IaaS Green | 141, 197, 63 | 8DC53F | IaaS icons |

### Group Overview
Group objects are provided as rectangular containers, rectangular or circular groups, or both to accomodate various uses but may change to single option:
1. Cloud Universe + Public Network + Enterprise Network - 3 containers plug IBM Cloud container to encompass the previous 3 section container-like diagram used for hybrid diagrams but with the power of Visio containers.  Refer to Hybrid example above.
2. IBM Cloud - Provided as a container with optional IBM Cloud icon.
3. Virtual Private Cloud (GC and GT) - Provided as a container with optional IBM Cloud icon. To be temporarily renamed to Reserved Container until VPC is announced.
4. Region - Provided as a container with a list of multi-zone regions to select from.  Single-zone regions will also be included when names are available.  
5. Zone - Provided as a container with a relative list of zones to select from.
6. Network ACL - Provided as a container with optional security icon. 
7. Security Group - Provided as a rectangular container, rectangular outline, or circular outline.
8. Auto Scale Group - Provided as a rectangular container, rectangular outline, or circular outline.
9. Performance Group (GT only) - Provided as a rectangular container, rectangular outline, or circular outline.  To be temporarily renamed to Reserved Group until GT is announced.

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
9. Add lines between desired objects either shape-to-shape by clicking inside the shape or point-to-point by clicking on existing points on the border of the shape or add additional points to the object as desired.  Change line color to blue and weight to 1 1/2 pt.  Note that when objects are moved the shape-to-shape will automatically reorganize where the line attaches to the objects and point-to-point will always maintain the line at each point.
