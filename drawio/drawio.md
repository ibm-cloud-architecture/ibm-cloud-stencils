# IBM VPC Stencils for draw.io

## IBM VPC Architecture for Gen1/Gen2
![VPCArchitecture](/images/ibm_vpc_architecture_drawio.png)

## IBM VPC Architecture for Gen2
![VPCArchitecture](/images/ibm_vpc_architecture_gen2_drawio.png)

## Notes

1. To use the IBM Stencils with draw.io:  https://draw.io/?libs=ibm
2. Continuing to evaluate whether containers enabled on all boxes is problematic - subject to change.
3. The ibm_vpc_architecture template under Cloud is outdated and being updated.
4. To use svg when exporting a diagram, select the entire diagram, then check the Selection Only and Crop, and check the Embed Images (to include icons) if the svg will be used offline.  If the Selection Only and Crop is not done the resulting svg file may have extra white space around the diagram which can also be removed by reducing the width and height in the svg itself.

## Upgrading

To update an existing diagram to the latest version on draw.io:
1. Backup existing diagram, open existing diagram in draw.io, and enable Format Panel under View.
2. For each box in IBM / Boxes:
    1. Select box to temporarily add to canvas for extracting style.
    2. Select Edit Style (draw.io also provides Copy Style which copies the style but not the image settings).
    3. Select all of new style, right click, select Copy.
3. For each box in existing diagram: 
    1. For Subnet, move contents of ACL textbox to Subnet textbox as Subnet:ACL.
    2. Delete existing box tag.
    3. Select Edit Style (draw.io also provides Paste Style which along with Copy Style copies the style but not the image settings).
    4. Select all of old style, right click and select Delete, right click and select Paste to insert copied new style.
4. Similarly for connectors from Connectors.xml if desired.
5. Remove boxes that were temporarily added to canvas.
6. If Cloud Universe box was used either leave as is or replace with the Public Network and Enterprise Network boxes in IBM / Boxes.
7. Tweek the diagram if more space is needed in places.

Return to [README](/README.md)
