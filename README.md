# IBM v1 Stencils

Create IBM Cloud diagrams with enterprise tools using IBM Cloud Stencils.  
Refer to the [IBM Architecture Center](https://www.ibm.com/cloud/garage/architectures/edit) for complete details.

## Overview

IBM Diagrams are comprised of boxes that group icons:
- [Architecture Icons](https://www.ibm.com/cloud/architecture/architectures/edit) which represent IBM Cloud components.
- [Service Icons](https://l2fprod.github.io/myarchitecture/) which represent services available in the IBM Cloud catalog.

## Example

<details><summary>IBM VPC Diagram using IBM v1 Stencils</summary>
<img src="/images/ibm_vpc_architecture_drawio.png">
</details>

## Notes

<details><summary>General</summary>
<p>

1. Floating IP icon is an arrow with a closed circle that represents a NIC pointing outwards from an instance. 

2. IBM VPC has a single subnet type Subnet where Subnet:ACL denotes a Subnet with an associated ACL which can be customized such as SubnetName:ACLName, SubnetCIDR:ACLName, split to 2 lines, etc.

3. Diagram containers if available in a tool (draw.io and Visio) are used as mentioned in the Overview.

4. To migrate existing boxes and groups to latest if desired, apply styles from new boxes and groups to existing diagram.  For draw.io, updating styles in existing boxes that are not yet containers won't make existing contents of a box part of the container.

</p>
</details>

<details><summary>draw.io</summary>
<p>

**NOTE: For IBM internal designs/diagrams, you must use the desktop application (2.) to create or edit a diagram. The draw.io/diagrams.net web application (1.) is only approved for public designs that contain no forward-looking material**

1. To use the IBM Stencils on draw.io in your browser: https://draw.io/?libs=ibm

2. To use the IBM Stencils on the [draw.io desktop application](https://github.com/jgraph/drawio-desktop/releases) do the following:

   1. Open application and click on "+ More Shapes" in the bottom left panel.
   2. Scroll down to the "Networking" section and check "IBM".
   3. Click "Apply" to finish.

   IBM Stencils should now be available in the embedded categories in the left panel.

3. Folders for draw.io on this github are used for changes not on draw.io and are subject to change.

4. When adding icons to diagrams the default background color for text should be transparent but instead may be white.  *See open issue #1 below for a workaround.*

5. When exporting diagrams to svg ensure that icons are included (check Embed Image) if using svg offline and ensure white space is minimal (select entire diagram then check Selection Only and Crop) if embedding in a document.

Open Issues:

1. Issue #620 where setting the icon text background to transparent doesn't work.<br/>Status: Open.  This issue happens if labelBackgroundColor=none is before the image; statement in icon style, so place the labelBackgroundColor=none to anywhere after the image; statement.<br/>
Status: Open.

Fixed Issues:

1. Issue #724 where icons dropped onto container in FF would not stay in container when container is moved.

2. Issue #723 where overlaying a box across other boxes may cause underlying boxes to expand and have to be resized such as when placing a security group box across multiple subnet boxes.  This scenario is working as designed so draw.io added a new property "expand" to swimlanes for our boxes.  The current behavior is the default with expand=1 and our boxes are set to expand=0.

3. Issue #748 to set container=0 for deployedTo boxes as mentioned in Overview.

</p>
</details>

<details><summary>Visio</summary>
<p>

1. Boxes are implemented as containers.

2. Box tags are currently separate and can optionally be placed on upper left corner of boxes.

</p>
</details>

<details><summary>Powerpoint</summary>
<p>

1. Refer to all-ibm-cloud-architecture-icons-October2019-WithVPCUpdatesFebruary2020.pptx on this github.

</p>
</details>
