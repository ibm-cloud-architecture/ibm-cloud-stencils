## IBM Cloud Stencils for draw.io

Introducing IBM Virtual Private Cloud diagrams for draw.io:
![VPCSimple](/images/vpc-experience-simple.png)

The diagram version shown above for draw.io integrates the group tag with the group border and also includes a few enhancements for readability.

To update an existing diagram to the latest version for draw.io:
1. Copy VPCgroups.xml and VPCarrows.xml from drawio/stencils in this github. 
2. Backup existing diagram locally, open existing diagram in draw.io, and select Format Panel under View.
3. Under File select Open Library from Device... for VPCgroups.xml and VPCarrows.xml.
4. For each group in VPCgroups.xml: select group, select Edit Style (see note), select all of style, right click, select Copy.
5. For each group in existing diagram: delete existing group tag (for Subnet move contents of ACL textbox to Subnet textbox, see example), select Edit Style (see note), select all of existing style, right click and select Delete, right click and select Paste.
6. Similarly for arrows from VPCarrows.xml if desired.
7. If Cloud Universe group was used you can either leave or replace with the Public Network and Enterprise Network groups in VPCgroups.xml.

Note: If you use Copy Style in step 4 and Paste Style in step 5 the style is copied but not the group tag.  You can also turn off the group tag by setting it to an invalid name in the style (e.g. CloudTag.svg to CloudTagOff.svg)

Return to [Main](/README.md)
