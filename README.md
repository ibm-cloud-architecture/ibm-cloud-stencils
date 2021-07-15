# IBM Stencils

## Overview

Create diagrams with IBM Stencils using enterprise tools:

IBM v2 Stencils (coming):
- <details><summary>diagrams.net (draw.io)</summary>
<p>

**NOTE: For IBM internal designs/diagrams, you must use the desktop application (2.) to create or edit a diagram. The draw.io/diagrams.net web application (1.) is only approved for public designs that contain no forward-looking material**

1. To use the IBM Stencils on draw.io/diagrams.net in your browser: https://draw.io/?libs=ibm

2. To use the IBM Stencils on the [draw.io desktop application](https://github.com/jgraph/drawio-desktop/releases) do the following:

   1. Open application and click on "+ More Shapes" in the bottom left panel.
   2. Scroll down to the "Networking" section and check "IBM".
   3. Click "Apply" to finish.

   IBM Stencils should now be available in the embedded categories in the left panel.
</details>

IBM v1 Stencils
- diagrams.net (draw.io)
- PowerPoint
- OmniGraffle
- Visio

## IBM v1 Stencils

### Example

<details><summary>IBM VPC Diagram using IBM v1 Stencils</summary>
<img src="/images/ibm_vpc_architecture_drawio.png">
</details>

### Notes

<details><summary>draw.io</summary>
<p>
1. Boxes are implemented as draw.io containers.

2. Folders for draw.io on this github are used for changes not on draw.io and are subject to change.

Fixed Issues:

- Issue #723 where overlaying a box across other boxes may cause underlying boxes to expand and have to be resized such as when placing a security group box across multiple subnet boxes.  This scenario is working as designed so draw.io added a new property "expand" to swimlanes for our boxes.  The current behavior is the default with expand=1 and our boxes are set to expand=0.

</p>
</details>

<details><summary>Visio</summary>
<p>

1. Boxes are implemented as Visio containers.

2. Box tags are currently separate and can optionally be placed on upper left corner of boxes.

</p>
</details>

<details><summary>Powerpoint</summary>
<p>

1. Refer to all-ibm-cloud-architecture-icons-October2019-WithVPCUpdatesFebruary2020.pptx on this github.

</p>
</details>
