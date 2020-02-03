# IBM Cloud Stencils

Create IBM Cloud diagrams with enterprise tools using IBM Cloud Stencils.  
Refer to the [IBM Architecture Center](https://www.ibm.com/cloud/garage/architectures/edit) for complete details.

# IBM Cloud Stencils for VPC

## Overview

Use enterprise tools to create IBM VPC diagrams that are designed to organize a VPC solution to visually show the functionality and availability of the IBM VPC platform.    

## Tools

[draw.io](/drawio/drawio.md)

[PowerPoint](/powerpoint/powerpoint.md)

[Visio2013](/visio2013/visio2013.md)

[Visio2010](/visio2010/visio2010.md)

## Updates (February 2020)

1. Organized into vpc icons, boxes, and connectors.
2. Added box type with integrated tags and boxes on draw.io.
3. Added shading to boxes for zones and subnets.
4. Added width variation on all boxes.
5. Added boxes for Instance Group, Resource Group, Cloud Services, Public Network, and Enterprise Network.
6. Added icons for Power Instance and Transit Gateway.

## Notes

1. To migrate existing diagrams to latest version of stencils:
   1. Apply box styles from new boxes to existing diagram and delete existing box tags.
   2. Apply connector styles from new connectors to existing diagram if desired.
   3. ACL is now specified as Subnet:ACL in Subnet title that can be customize as desired.
   4. Cloud Universe now consists of 3 boxes for Public Network + IBM Cloud + Enterprise Network.
   5. Tweek the diagram if more or less space is needed in places.

## Styles

| Style | Hex Color | RGB Color |
| :--- | :--- | :--- |
| Text (Helvetica 12 pt) | #000000 | 0,0,0 |
| Connectors (1 pt) | #000000 | 0,0,0 |
| Blue Borders | #4376BB | 67,120,187 |
| Green Borders | #00882B | 0,136,43 |
| Light Green Fill | #E6F0E2 | 230,240,226 |
| Grey Borders | #919191 | 145,145,145 |
| Light Grey Fill | #E0E0E0 | 224,224,224 |
| Red Borders | #FF0000 | 255,0,0 |
| Light Red Fill (reserved) | #FFE4E1 | 255,228,225 |

## Boxes

| Box | Style | Width |
| :--- | :--- | ---: |
| IBM Cloud<br/>Public Network<br/>Enterprise Network | Solid Blue Border | 3 pt |
| VPC | Solid Blue Border | 2 pt |
| Region | Solid Grey Border | 2 pt |
| Zone | Solid Grey Border<br/>Light Grey Fill | 1 pt |
| Subnet | Solid Green Border<br>Light Green Fill | 1 pt |
| Security Group | Dashed Red Border | 2 pt |
| Reserved Group | Dashed Green Border | 2 pt |
| Resource Group | Dashed Grey Border | 2 pt |
| Cloud Services | Solid Blue Border | 1 pt |
| (reserved) | Solid Red Border<br>Light Red Fill | 1 pt |
