## IBM Cloud Stencils for draw.io

Introducing IBM Virtual Private Cloud diagrams for draw.io:
![VPCSimple](/images/vpc-experience-simple.png)

The updated styles in VPCgroups.xml and VPCarrows.xml in drawio/stencils on this github have integrated the group tag (upper left corner) with the group border and also includes a few enhancements for consumability and readability.

To update an existing diagram to the latest version for draw.io:
1. Copy VPCgroups.xml and VPCarrows.xml. 
2. Backup existing diagram locally, open existing diagram in draw.io, and enable Format Panel under View.
3. Under File select Open Library from Device... for VPCgroups.xml and VPCarrows.xml.
4. For each group in VPCgroups.xml: select group, select Edit Style (see note 1), select all of style, right click, select Copy.
5. For each group in existing diagram: delete existing group tag (for Subnet move contents of ACL textbox to Subnet textbox, see example), select Edit Style (see note 1), select all of existing style, right click and select Delete, right click and select Paste.
6. Similarly for arrows from VPCarrows.xml if desired.
7. If Cloud Universe group was used you can either leave as is or replace with the Public Network and Enterprise Network groups in VPCgroups.xml.

Notes: 
1. If you use Copy Style for step 4 and Paste Style for step 5 the style is copied but not the group tag.  
2. You can also turn off the group tag by changing it to an invalid name in the style (e.g. change CloudTag.svg to CloudTagOff.svg)
3. The path of group tags in first line of styles may change but current path will continue to be valid also.

Return to [Main](/README.md)
