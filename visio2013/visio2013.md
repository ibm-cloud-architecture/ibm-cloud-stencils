## IBM VPC Stencils for Visio 2013

![VPCExperience](/images/ibm_vpc_architecture_visio.png)

# Upgrade Steps

To update an existing diagram to the latest version on this github for Visio 2013:
1. Make a local copy of VPC Groups.vssx, VPC Arrows.vssx, and VPC.vssx in your My Shapes folder.
2. Backup existing diagram and open existing diagram in Visio 2013.
3. Under More Shapes go to My Shapes folder and select VPC Groups.vssx, VPC Arrows.vssx, and VPC.vxxs.
4. For each Security Group: 
    1. Select border.
    2. Change to dash used in VPC Groups.
    3. Change to 2 pt width.
5. For all other groups:
    1. For Subnet, move contents of ACL textbox to Subnet textbox, see example.
    2. Delete existing group tag.
    3. Select border.
    3. Change to solid line if not already.
    4. Change to 2 pt width.
    5. Change to same color used in VPC Groups.
6. Change arrows and lines to 2 pt width if desired.
7. If Cloud Universe group was used you can either leave as is or replace with the Public Network and Enterprise Network groups in VPC Groups.
8. Tweek the diagram if more space is needed in places.

Return to [README](/README.md)
