## IBM Cloud Stencils for draw.io

IBM Virtual Private Cloud diagrams for draw.io:
![VPCSimple](/images/vpc-experience-simple-drawio.png)

To be used in conjuction with the IBM Cloud Stencils on draw.io, the updated styles in VPCgroups.xml and VPCarrows.xml in drawio/stencils on this github have integrated the group tag (square icon in upper left corner) with the group border and also includes a few enhancements for consumability and readability.

To update an existing diagram to the latest version for draw.io:
1. Make a local copy of VPCgroups.xml and VPCarrows.xml. 
2. Backup existing diagram, open existing diagram in draw.io, and enable Format Panel under View.
3. Under File select Open Library from Device... for VPCgroups.xml and VPCarrows.xml.
4. For each group in VPCgroups.xml: 
    1. Select group to temporarily add to canvas for extracting style.
    2. Select Edit Style (see note 1).
    3. Select all of new style, right click, select Copy.
5. For each group in existing diagram: 
    1. For Subnet, move contents of ACL textbox to Subnet textbox, see example.
    2. Delete existing group tag.
    3. Select Edit Style (see note 1).
    4. Select all of old style, right click and select Delete, right click and select Paste to insert copied new style.
6. Similarly for arrows from VPCarrows.xml if desired.
7. Remove groups that were temporarily added to canvas.
8. If Cloud Universe group was used you can either leave as is or replace with the Public Network and Enterprise Network groups in VPCgroups.xml.
9. Tweek the diagram if more space is needed in places.

Notes: 
1. Besides Edit Style draw.io also provides Copy Style and Paste Style which if used for step 4 and step 5 the style is copied but not the group tag.  
2. If desired, the group tag can be turned off by changing it to an invalid name in the style (e.g. change CloudTag.svg to CloudTagOff.svg) or removing the image settings in the style.
3. Path of group tags in first line of styles will change but current path will continue to be valid also.
4. Some group tags in VPCgroups.xml won't initially match the example above.

Return to [README](/README.md)
