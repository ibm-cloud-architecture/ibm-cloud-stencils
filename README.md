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

## Updates (January 2020)

1. Separated into vpc icons, boxes, and connectors.
2. Secured tag to box in draw.io.  
3. Removed use of containers for some boxes in draw.io and leave for future consideration.
4. Added shading to boxes for zones and subnets for consumability and readability.
5. Added boxes for Resource Group and Reserved Group (actual name coming).
6. Added general boxes for Public Network, Enterprise Network, and Cloud Services.
7. Added icons for Power Instance and Transit Gateway.
8. Added additional connectors based on usage. 

## Notes

1. Connectors are provided by the IBM Cloud Stencils in addition to the connectors provided by the tool, for example, arrows can be drawn between objects directly in draw.io resulting in a single arrow connector which can be left as is or updated to a double arrow or dashed line similar to the provided connectors.

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
