## IBM VPC Stencils for draw.io

![VPCExperience](/images/ibm_vpc_architecture_drawio.png)

# Implementation Notes

1. Use draw.io with IBM Stencils enabled:  https://draw.io/?libs=ibm
2. Refer to Boxes.xml and Connectors.xml on this github. The tags (upper left corner of boxes) have some changes and the final path mentioned in the Box.xml styles on this github will change.
3. The boxes are not implemented as draw.io containers due to a potential expansion problem but grouping boxes has a similar effect as containers. 
4. Before exporting ia diagrams to svg, select the entire diagram, then check the Selection Only and Crop, and check the Embed Images if the svg will be used offline.  If the Selection Only and Crop is not done the resulting svg file may have extra white space (potentially significant) around the diagram which can also be removed by reducing the width and height in the svg itself.


# Upgrade Steps

To update an existing diagram to the latest version on this github for draw.io:
1. Make a local copy of Boxes.xml and Connectors.xml. 
2. Backup existing diagram, open existing diagram in draw.io, and enable Format Panel under View.
3. Under File select Open Library from Device... for Boxes.xml and Connectors.xml.
4. For each group in Boxes.xml: 
    1. Select group to temporarily add to canvas for extracting style.
    2. Select Edit Style (draw.io also provides Copy Style which copies the style but not the image settings).
    3. Select all of new style, right click, select Copy.
5. For each group in existing diagram: 
    1. For Subnet, move contents of ACL textbox to Subnet textbox, see example.
    2. Delete existing group tag.
    3. Select Edit Style (draw.io also provides Paste Style which along with Copy Style copies the style but not the image settings).
    4. Select all of old style, right click and select Delete, right click and select Paste to insert copied new style.
6. Similarly for connectors from Connectors.xml if desired.
7. Remove groups that were temporarily added to canvas.
8. If Cloud Universe group was used you can either leave as is or replace with the Public Network and Enterprise Network groups in Boxes.xml.
9. Tweek the diagram if more space is needed in places.

Return to [README](/README.md)
