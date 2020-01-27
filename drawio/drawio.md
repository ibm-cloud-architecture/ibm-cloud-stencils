## IBM VPC Stencils for draw.io

![VPCExperience](/images/ibm_vpc_architecture_drawio.png)

# Notes

1. To use the IBM Stencils with draw.io:  https://draw.io/?libs=ibm
2. Use the temporary Boxes.xml and Connectors.xml on this github in conjunction with the IBM VPC Stencils on draw.io. The Boxes.xml on this github has some differences including path in the final version.
3. To enable container-like use of the boxes, grouping boxes will create a similar effect as containers.  The draw.io container property is not enabled due to a potential problem. 
4. To use svg when exporting a diagram, select the entire diagram, then check the Selection Only and Crop, and check the Embed Images (to include icons) if the svg will be used offline.  If the Selection Only and Crop is not done the resulting svg file may have extra white space around the diagram which can also be removed by reducing the width and height in the svg itself.


# Upgrading

To update an existing diagram to the latest version on this github for draw.io:
1. Make a local copy of Boxes.xml and Connectors.xml. 
2. Backup existing diagram, open existing diagram in draw.io, and enable Format Panel under View.
3. Under File select Open Library from Device... for Boxes.xml and Connectors.xml.
4. For each box in Boxes.xml: 
    1. Select box to temporarily add to canvas for extracting style.
    2. Select Edit Style (draw.io also provides Copy Style which copies the style but not the image settings).
    3. Select all of new style, right click, select Copy.
5. For each box in existing diagram: 
    1. For Subnet, move contents of ACL textbox to Subnet textbox, see example.
    2. Delete existing box tag.
    3. Select Edit Style (draw.io also provides Paste Style which along with Copy Style copies the style but not the image settings).
    4. Select all of old style, right click and select Delete, right click and select Paste to insert copied new style.
6. Similarly for connectors from Connectors.xml if desired.
7. Remove boxes that were temporarily added to canvas.
8. If Cloud Universe box was used either leave as is or replace with the Public Network and Enterprise Network boxes in Boxes.xml.
9. Tweek the diagram if more space is needed in places.

Return to [README](/README.md)
