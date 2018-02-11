# IBM Cloud Visio Icons

## Legends

![Legends](/images/legends.png)

## 3-Tier Template

![3-Tier](/images/3-tier.png)

## Visio Icon Conversion (vssx folder)

Tentative (subject to change) conversion of IBM Cloud Icons from pptx to vssx for Visio 2013 and later.  This Visio version contains additional icons as needed for IaaS plus the groups.  Need to determine whether to provide vss files for Visio 2003-2013.  

## Visio Diagram Templates (vstx folder)

Template files are in the process of being converted to Visio from other tools including reference architectures from the client success team.  Also working with draw.io support to fix problems with the export of draw.io templates to Visio. 

## User Guide

### Color Scheme
* Blue (RGB 67, 120, 187 or Hex 4378BB) - Used for outer containers, text, and lines.
* Red (RGB 255, 0, 0 or Hex FF0000) - Used for security containers and security groups.
* Green (RGB 0, 136, 43 or Hex 00882B) - Used for inner non-security groups).
* Yellow (RGB 237, 193, 28, or EDC11C) - Used for lines as additional color besides blue.

### Container Steps
1. Drag and drop the desired containers from the groups onto the canvas.
2. Select a single name from the provided list in the region and zone or replace with another name.
3. Optionally delete any container name that is not desired to save vertical space.
4. Optionally add the provided logo icons on the side border or bottom border or inside or outside the respective containers for IBM Cloud, Virtual Private Cloud, and Network ACL.  Note that adding the logo icon to the top border of the containers will break the container so it is no longer recognized as a container.

### Icon Steps
1. Drag icon from stencil to canvas.  Note that the master name is not automatically included with the icon on the canvas.
2. To add text to an icon on the canvas, select the icon and type the desired text.
3. Resize text to Calibri 10 pt if desired to fit more text than Calibri 12 pt.
4. Change text to blue color above if desired.  
5. If a line obstructs the text, select text, right-click and select Font, go to Text Block, and select solid color of white for text background.
6. If any of the text wraps to next line, select text, select Text Block (Shift+Ctrl+4) under Connection Point under HOME, widen text box and move widened text box to be in the center under icon. 
7. Add lines between desired objects either shape-to-shape by clicking inside the shape or point-to-point by clicking on points on the border of the shape.  Note that shape-to-shape will automatically reorganize where the line attaches to the objects and point-to-point will always maintain the line at each point.

## Visio Diagram Templates (vstx folder)

Template files are in the process of being converted to Visio from other tools including reference architectures from Paul Bahr.  Also working with draw.io support to fix problems with the export of draw.io templates to Visio. The list of names in the region and zone are intended to be edited to a single name by the architect.  
