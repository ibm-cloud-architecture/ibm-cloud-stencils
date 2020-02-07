# IBM Cloud Stencils

Create IBM Cloud diagrams with enterprise tools using IBM Cloud Stencils.  
Refer to the [IBM Architecture Center](https://www.ibm.com/cloud/garage/architectures/edit) for complete details.

# IBM Cloud Stencils for VPC

## Overview

Use enterprise tools to create IBM VPC diagrams that are designed to organize a VPC solution to visually show the functionality and availability of the IBM VPC platform.    

![VPCArchitecture](/images/ibm_vpc_architecture_power_drawio.png)

## General Notes

1. Instance Group feature is not currently available. 
2. IBM VPC has a single subnet type Subnet.
3. Subnet:ACL denotes a Subnet with an associated ACL which can be customized such as SubnetName:ACLName, SubnetCIDR:ACLName, split to 2 lines, etc.
4. Diagram containers if available in a tool (draw.io and Visio) are used for primary boxes but not secondary boxes (Instance Group, Resource Group, and Security Group).  
5. To migrate existing diagrams to latest version (February 2020) of stencils:
   1. Apply box styles from new boxes to existing diagram and delete existing box tags.  For draw.io, updating styles in existing containerless diagrams won't take advantage of containerized styles but using the grouping feature creates container-like behavior if desired.
   2. Apply connector styles from new connectors to existing diagram if desired.
   3. ACL is now specified as Subnet:ACL in Subnet title that can be customized as desired.
   4. Cloud Universe now consists of 3 boxes for Public Network + IBM Cloud + Enterprise Network.
   5. Tweek the diagram if more or less space is needed in places.

## draw.io Notes

1. To use the IBM Stencils on draw.io: https://draw.io/?libs=ibm
2. Template named ibm_vpc_architecture under Cloud is currently outdated.
3. Folders for draw.io on this github are used for changes not on draw.io.
4. Primary boxes are implemented as containers:  
   1. Temporary step to set container=0 (in style or uncheck property) for the 3 secondary boxes (Instance Group, Resource Group, Security Group), or leave as is.  See issue #2.
   2. Temporary step to resize underlying primary boxes when secondary boxes are placed across multiple primary boxes.  See issue #3.
   3. Temporary step to ensure icons remain with a primary box by adding icons to standalone primary boxes before nesting primary boxes, or group nested primary boxes.  See issue #4.
5. Changing box border color will also change tag color allowing customization with other preferred colors, but note that deviating from standards below might conflict with boxes/colors added to the stencils in the future.
6. Changing box border color to white on white background makes the box appear invisible, so for example if used for Public Network and Enterprise Network boxes to hide borders while still taking advantage of their containers.
7. When adding icons to diagrams the default white background color for text can be unchecked if desired so text has background color of shaded boxes.  
   1. Temporary step if this doesn't work is to replace a non-working style with a working style in each icon in shaded areas (will post example here soon), or leave with text background color of white.  See issue #1.
8. When exporting diagrams to svg ensure that icons are included (check Embed Image) if using svg offline and ensure white space is minimal (select entire diagram then check Selection Only and Crop) if embedding in a document.

### draw.io Issues

1. Issue #620 where setting the icon text background from white to nothing doesn't work.  Status: Found that this previously worked, so provided example in issue of a working style and a non-working style.
2. Issue #748 to remove container setting for 3 secondary boxes.  Status: Opened.
3. Issue #723 when overlaying a box on multiple boxes which may cause underlying boxes to expand and have to be resized. Status: Working as designed but an option is being discussed to disable the auto-resizing.  
4. Issue #724 when adding an icon to a container the icon doesn't remain with the container.  Status: Found that this scenario doesn't work with nested boxes but does work with icons added to standalone containers.

## Visio Notes

1. Primary boxes are implemented as containers.
2. Box tags are currently separate and can optionally be placed on upper left corner of boxes.

## PowerPoint Notes

1. Refer to all-ibm-cloud-architecture-icons-October2019-WithVPCUpdatesFebruary2020.pptx on this github.

## Color Standards

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

## Box Standards

| Box | Style | Width | Type (if available) |
| :--- | :--- | ---: | :--- |
| IBM Cloud | Solid Blue Border | 3 pt | Container | 
| Public Network | Solid Blue Border | 3 pt | Container | 
| Enterprise Network | Solid Blue Border | 3 pt | Container | 
| VPC | Solid Blue Border | 2 pt | Container |
| Region | Solid Grey Border | 2 pt | Container |
| Zone | Solid Grey Border<br/>Light Grey Fill | 1 pt | Container |
| Subnet | Solid Green Border<br>(or Solid Red Border)<br>Light Green Fill | 1 pt | Container |
| Cloud Services | Solid Blue Border | 1 pt | Container |
| Instance Group | Dashed Green Border | 2 pt | Non-container |
| Resource Group | Dashed Grey Border | 2 pt | Non-container |
| Security Group | Dashed Red Border | 2 pt | Non-container |
