# IBM Cloud Visio Icons

## Legends

![Legends](/images/legends.png)

## 3-Tier Example

![3-Tier](/images/3-tier.png)

## Multizone Example

![Multizone](/images/Multizone.png)

## Visio Icon Conversion (vssx folder)

Conversion of IBM Cloud Icons from pptx to vssx for Visio 2013 and later.  Thisvversion contains additional IaaS icons plus the new IaaS containers.  Note that VPC will be removed from the published version until VPC is announced.  Need to determine whether to provide vss files for Visio 2003-2013.  

## Visio Diagram Templates (vstx folder)

Template files are in the process of being converted to Visio from other tools including reference architectures from the client success team.  Also working with draw.io support to fix problems with the export of draw.io templates to Visio. 

## User Guide

### Color Scheme
* Blue (RGB 67, 120, 187, or Hex 4378BB) - Used for outer containers, text, and lines.
* Red (RGB 255, 0, 0, or Hex FF0000) - Used for security containers and security groups.
* Green (RGB 0, 136, 43, or Hex 00882B) - Used for inner non-security groups).
* IaaS Green (RGB 141, 197, 63, or Hex 8DC53F) - Used for IaaS icons.
* Yellow (RGB 237, 193, 28, or Hex EDC11C) - Can also be used for specific lines as additional color besides blue.

### Group Overview
Group objects are provided as rectangular containers, rectangular or circular groups, or both to accomodate various uses but may change to single optio:
1. IBM Cloud - Provided as a container with optional IBM Cloud icon.
2. Virtual Private Cloud (GC and GT) - Provided as a container with optional IBM Cloud icon. To be temporarily renamed to Reserved Container until VPC is announced.
3. Region - Provided as a container with a list of regions to select from.
4. Zone - Provided as a container with a relative list of regions to select from.
5. Network ACL - Provided as a container with optional security icon. 
6. Security Group - Provided as a rectangular container, rectangular outline, or circular outline.
7. Auto Scale Group - Provided as a rectangular container, rectangular outline, or circular outline.
8. Performance Group (GT only) - Provided as a rectangular container, rectangular outline, or circular outline.  To be temporarily renamed to Reserved Group until GT is announced.

### Group Steps
1. Drag and drop the desired group/containers from the groups onto the canvas.
2. Select a single name from the provided list in the region and zone or replace with another name.
3. Optionally delete any group/container name that is not desired to save vertical space.
4. Optionally add the provided logo icons on a border or inside the respective group/containers for IBM Cloud, Virtual Private Cloud, and Network ACL.  

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
