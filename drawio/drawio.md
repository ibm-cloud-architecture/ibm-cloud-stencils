## IBM Cloud Stencils for draw.io

Introducing IBM Virtual Private Cloud diagrams for draw.io:
![VPCSimple](/images/vpc-experience-simple.png)

The diagram version shown above for draw.io integrates the group tag with the group border and also includes a few enhancements for readability.

To update an existing diagram to the latest version for draw.io:
1. Copy VPCgroups.xml and VPCarrows.xml from drawio/stencils in this github. 
2. Backup existing diagram locally, open existing diagram in draw.io, and be sure that Format Panel is slected under View.
3. Under File select Open Library from Device... for VPCgroups.xml and VPCarrows.xml.
4. For each group in VPCgroups.xml select the group, select Copy Style (or select Edit Style, select all of the style, right click and select Copy).
5. For each group in existing diagram, delete existing group tag in upper left corner (for Subnet move the contents of ACL textbox to Subnet textbox, see example), select Paste Style (or select Edit Style if using Edit Style in previous step, select all of existing style, right click and select Delete, right click and select Paste).
6. Similarly for arrows from VPCarrows.xml if desired.
7. If Cloud Universe group was used you can replace with the Public Network and Enterprise Network groups in VPCgroups.xml

Return to [Main](/README.md)
