## IBM Cloud Stencils for draw.io

![VPCSimple](/images/vpc-experience-simple-drawio.png)

# Implementation Notes

1. VPC stencils consists of VPC (on draw.io), VPC Groups (VPCgroups.xml on this github), and VPC Arrows (VPCarrows.xml on this github).
2. VPC Groups integrates the group tag (square icon in upper left corner) with the group border and also includes a few enhancements for consumability and readability.
3. Group name (e.g. IBM Cloud) could be deleted in some cases if desired since the group tag designates what the group is or vice versa.
4. Group tag can be turned off by changing it to an invalid name in the style (e.g. change CloudTag.svg to CloudTagOff.svg) or removing the image settings in the style.
5. Path of group tags at beginning of styles will change but current path will continue to be valid also.
6. Some group tags in VPC Groups won't initially match the example above.
7. All groups are implemented as containers except Security Group is not a container since it can span other groups. Containers are advantageous in that the contents are moved/copied along with the container.
8. All borders and lines are 2 pt to be visible with limited space - can be customized as desired.
9. All text and lines are black to distinguish from borders and icons, and text is Helvetica 12 pt - can be customized as desired.

# Upgrade Steps

To update an existing diagram to the latest version on this github for draw.io:
1. Make a local copy of VPCgroups.xml and VPCarrows.xml. 
2. Backup existing diagram, open existing diagram in draw.io, and enable Format Panel under View.
3. Under File select Open Library from Device... for VPCgroups.xml and VPCarrows.xml.
4. For each group in VPCgroups.xml: 
    1. Select group to temporarily add to canvas for extracting style.
    2. Select Edit Style (draw.io also provides Copy Style which copies the style but not the image settings).
    3. Select all of new style, right click, select Copy.
5. For each group in existing diagram: 
    1. For Subnet, move contents of ACL textbox to Subnet textbox, see example.
    2. Delete existing group tag.
    3. Select Edit Style (draw.io also provides Paste Style which along with Copy Style copies the style but not the image settings).
    4. Select all of old style, right click and select Delete, right click and select Paste to insert copied new style.
6. Similarly for arrows from VPCarrows.xml if desired.
7. Remove groups that were temporarily added to canvas.
8. If Cloud Universe group was used you can either leave as is or replace with the Public Network and Enterprise Network groups in VPCgroups.xml.
9. Tweek the diagram if more space is needed in places.
1. Besides Edit Style draw.io also provides Copy Style and Paste Style which if used for step 4 and step 5 the style is copied but not the group tag.  

Return to [README](/README.md)
