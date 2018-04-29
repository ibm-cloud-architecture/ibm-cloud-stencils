# IBM Cloud Visio Stencils

## User Guide

### Installation

1. Set the location of local folders for Visio:  File -> Options -> Advanced -> File Locations...
2. Create a folder named *IBM Cloud* in the local stencils folder.  
3. Copy the contents of the GitHub stencils folder (vssx files) to the local stencils folder.
4. Create a folder named *IBM Cloud* in the local templates folder. 
5. Copy the contents of the GitHub templates folder (vstx files) to the local templates folder.

### Setup

1. Select one of the template files to bring up a fully editable diagram in Visio and delete any icons that will not use along with any connection lines.

2. Go to More Shapes in Visio, find the folder containing the stencils, and select the stencils that you want to use in your diagrams.

![Shapes](/images/shapes.png)

3. Groups with Visio containers are provided and demonstrated in the templates to help organize diagrams.

![Groups](/images/groups.png)

4. Review the standard colors used in the templates.

![Colors](/images/colors.png)

### Navigating Visio

#### Groups
1. Select a group implemented as a Visio container to enable the CONTAINER TOOLS in the ribbon.
2. If an object will be placed over multiple Visio containers simultanenously the Visio containers must be locked under Membership in the CONTAINER TOOLS FORMAT, then unlocked after the object has been put into position.

![RibbonWithFormat](/images/ribbonwithformat.png)

#### Snap & Glue
1. Snap & Glue is enabled by default and helps with aligning icons and drawing lines among other things.
2. Disabling Snap & Glue allows precise icon placement when an icon won't go where you want it because of alignment.
3. To disable Snap & Glue, select Snap & Glue menu in the Quick Access Toolbar, uncheck Snap & Glue, select OK and exit Snap & Glue menu, put the icon where you want it, then go back and reenable Snap & Glue.
4. If you don't have Snap & Glue in the Quick Access Toolbar, go to File -> Options -> Quick Access Toolbar, search All Commands and add Snap & Glue to the Quick Access Toolbar.

![SnapAndGlue](/images/snapandglue.png)

#### Lines & Text
1. Lines are added between icons using the Connector under Tools.
2. Lines can have additional angles added either by holding the shift key and dragging to break out the midpoint of the line with four new right angles, or by holding the control key to create a single angle of an arbitrary degree at the midpoint.
3. Weight, color, and arrows of lines can be customized under Shape Styles.  
4. Size and color of the icon text can be customized under Font.
5. Position of the icon text can be modified by selecting the Text Block (Shift+Ctrl+4) under Tools.

![Ribbon](/images/ribbon.png)

### Adding Objects

#### Groups
1. Add a group and resize as desired.
2. You can delete the group name to save space if desired.
3. You can place a logo on the group border if desired.  

#### Icons & Lines
1. Add an icon to your diagram and resize as desired.  
2. Add text to the new icon by clicking on the icon and typing the text.
3. Customize the size and color of the text under Font.  
4. To subscript or superscript, highlight the desired part of the text and press "Ctrl =" to make the highlighted text subscript or "Ctrl Shift =" to make the highlighted text superscript. 
5. If any of the text wraps to next line, select text, select Text Block (Shift+Ctrl+4) under Tools, widen and reposition the text box.  You can also move the text to other sides of the icon out of the way of lines.  When done unselect the Text Block by selecting the Pointer Tool under Tools. 
6. Add a line from the new icon to another icon by using the Connector under Tools. 
7. Customize the weight and color of the line and add arrows under Shape Styles.
8. If a line obstructs the text, select text, right-click and select Font, select solid color of white for text background, and select Bring to Front. 
