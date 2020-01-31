# IBM VPC Stencils for Visio 2010

## IBM VPC Architecture for Gen1/Gen2
![VPCExperience](/images/ibm_vpc_architecture_visio.png)

## Notes

1. Additional work is needed on securing the tags.

## Upgrading

To update an existing diagram to the latest version on this github for Visio 2010:
1. Make a local copy of Boxes.vss, Connectors.vss, and VPC.vss in your My Shapes folder.
2. Backup existing diagram and open existing diagram in Visio 2010.
3. Under More Shapes go to My Shapes folder and select Boxes, Connectors, and VPC.
4. For each Security Group: 
    1. Select border.
    2. Change to dash used in Boxes.
    3. Change to 2 pt width.
5. For all other groups:
    1. For Subnet, move contents of ACL textbox to Subnet textbox, see example.
    2. Delete existing group tag.
    3. Select border.
    4. Change to solid line if not already.
    5. Change to same width used in Boxes.
    6. Change to same color used in Boxes.
    7. Add group tag from Boxes.
6. Use 1 pt width for connectors or as desired.
7. If Cloud Universe group was used you can either leave as is or replace with the Public Network and Enterprise Network groups in Boxes.
8. Tweek the diagram if more space is needed in places.

Return to [README](/README.md)
