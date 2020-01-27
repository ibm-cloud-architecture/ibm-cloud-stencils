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
2. Ensure tag remains in position with box during diagram creation in draw.io.  
3. Removed use of containers for some boxes in draw.io and leave for future consideration.
4. Added shading to boxes for zones and subnets for consumability and readability.
5. Added boxes for Resource Group and Reserved Group (actual name coming).
6. Added general boxes for Public Network and Enterprise Network.
7. Added icons for Power Instance and Transit Gateway.
8. Added additional connectors based on usage. 

## Notes

1. Connectors are provided by the IBM Cloud Stencils as a convenience in addition to the connectors provided by the tool, for example, arrows can be drawn between objects directly in draw.io resulting in a single arrow connector with 1 pt width which can be left as is or updated to a double arrow or dashed line with 2 pt width similar to the provided connectors.
2. Box tags, box titles, and box colors are provided as a visual reference but rather than have both a box tag and box title for IBM Cloud, for example, the box would still be recognizable with one or the other.

## Styles

| Style | Hex Color | RGB Color | Font/Width |
| :--- | :--- | :--- | ---: |
| Text | #000000 | 0,0,0 | Helvetica 12 pt |
| Lines / Arrows | #000000 | 0,0,0 | 2 pt |
| Blue Borders | #4376BB | 67,120,187 | 2 pt |
| Green Borders | #00882B | 0,136,43 | 2 pt |
| Light Green Fill | #E6F0E2 | 230,240,226 | |
| Grey Borders | #919191 | 145,145,145 | 2 pt |
| Light Grey Fill | #E0E0E0 | 224,224,224 | |
| Red Borders | #FF0000 | 255,0,0 | 2 pt |
| Light Red Fill (reserved) | #FFE4E1 | 255,228,225 | |

## Groups

| Group | Style |
| :--- | :--- |
| VPC<br/>IBM Cloud<br/>Public Network<br/>Enterprise Network | Solid Blue Border |
| Region | Solid Grey Border |
| Zone | Solid Grey Border<br/>Light Grey Fill |
| Subnet | Solid Green Border<br>Light Green Fill |
| Security Group | Dashed Red Border |
| Reserved Group | Dashed Green Border |
| Resource Group | Dashed Grey Border |
| (reserved) | Solid Red Border<br>Light Red Fill |
