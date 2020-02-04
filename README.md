# IBM Cloud Stencils

Create IBM Cloud diagrams with enterprise tools using IBM Cloud Stencils.  
Refer to the [IBM Architecture Center](https://www.ibm.com/cloud/garage/architectures/edit) for complete details.

# IBM Cloud Stencils for VPC

## Overview

Use enterprise tools to create IBM VPC diagrams that are designed to organize a VPC solution to visually show the functionality and availability of the IBM VPC platform.    

![VPCArchitecture](/images/ibm_vpc_architecture_power_drawio.png)

## Updates (February 2020)

1. Organized into vpc icons, boxes, and connectors.
2. Added box type with integrated tags on draw.io.
3. Added shading to boxes for zones and subnets.
4. Added width variation on boxes.
5. Added boxes for Instance Group, Resource Group, Cloud Services, Public Network, and Enterprise Network.
6. Added icons for Power Instance and Transit Gateway.

## General Notes

1. Instance Group feature is not currently available. 
2. To migrate existing diagrams to latest version of stencils:
   1. Apply box styles from new boxes to existing diagram and delete existing box tags.  For draw.io, updating styles in existing containerless diagrams won't take advantage of containerized styles but using the grouping feature creates container-like behavior if desired.
   2. Apply connector styles from new connectors to existing diagram if desired.
   3. ACL is now specified as Subnet:ACL in Subnet title that can be customize as desired.
   4. Cloud Universe now consists of 3 boxes for Public Network + IBM Cloud + Enterprise Network.
   5. Tweek the diagram if more or less space is needed in places.

## draw.io Notes

1. To use the IBM Stencils: https://draw.io/?libs=ibm
2. Template named ibm_vpc_architecture under Cloud is currently outdated.
3. Folders on this github are used for changes not on draw.io.
4. Nongroup boxes are implemented as containers.  Temporary step to set container=0 (in style or uncheck property) for group boxes only.  There is a potential issue being investigated when overlaying groups on multiple boxes which may cause underlying boxes to expand and have to be resized.
5. Box tag can be removed if desired by removing shape and prType properties in style.
6. Box tag and border can change color if desired by changing border color which would deviate from the standards below but can be useful to make the border and tag invisible on white background by changing border color to white, for example to advantage of containers for Public Network and Enterprise Network but making their border and tag white.
7. When adding icons to diagrams the default white background color for text can be unchecked if desired so text has background color of shaded boxes.  There is a potential issue being investigated with the unchecking sometimes not sticking.
8. When exporting diagrams to svg ensure that icons are included and white space is mimimal.  Icons use a web reference and are not included in the svg by default so if the svg will be used offline check Embed Images when exporting the svg. To minimize white space select the entire diagram first then check the Selection Only and Crop when exporting the svg.

## Visio Notes

1. Nongroup boxes are implemented as containers.
2. Box tags are currently separate and can optionally be placed on upper left corner of boxes.

## PowerPoint Notes

1. Refer to all-ibm-cloud-architecture-icons-October2019-WithVPCUpdatesFebruary2020.pptx on this github.

## Diagram Standards

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
| Light Red Fill | #FFE4E1 | 255,228,225 |

## VPC Boxes

| Box | Style | Width |
| :--- | :--- | ---: |
| IBM Cloud<br/>Public Network<br/>Enterprise Network | Solid Blue Border | 3 pt |
| VPC | Solid Blue Border | 2 pt |
| Region | Solid Grey Border | 2 pt |
| Zone | Solid Grey Border<br/>Light Grey Fill | 1 pt |
| Subnet | Solid Green Border<br>Light Green Fill | 1 pt |
| Instance Group | Dashed Green Border | 2 pt |
| Resource Group | Dashed Grey Border | 2 pt |
| Security Group | Dashed Red Border | 2 pt |
| Cloud Services | Solid Blue Border | 1 pt |
| (reserved) | Solid Red Border<br>Light Red Fill | 1 pt |
