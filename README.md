# IBM Cloud Stencils

Create IBM Cloud diagrams with enterprise tools using IBM Cloud Stencils.  
Refer to the [IBM Architecture Center](https://www.ibm.com/cloud/garage/architectures/edit) for complete details.

# Importing Stencil Libraries into Draw.io

This easy guide provides instructions to import stencils published in this repository (**drawio folder**) into draw.io.
Stencils/icons are added and grouped using libraries, the libraries can contain one or several stencils, these are saved and generated in XML format (.xml). To use these these custom libraries, they first must be imported in order to make them available in the draw.io utility. 

## Import Guides

<details><summary>Import using Download Zip</summary>
<p>

- To download all contents of the repository, navigate to the main [page](README.md), click the **Clone or download** button and then select **Download ZIP**.

- Go to your downloads directory and extract the ZIP file contents and access the folder called **drawio**, it should be located in the following path:

`YourDownloadsDirectory/ibm-cloud-stencils-master/drawio`

- Confirm XML file(s) you wish to import are visible inside the the drawio folder in your downloads directory:

![](/images/ConfirmXMLfiles.png)

- Open the desktop [Draw.io application](https://github.com/jgraph/drawio-desktop/releases) in your computer or open [draw.io](https://www.draw.io/) in your browser.

- Select **Create New Diagram**, then click **Create**.

- Click on **File > Open Library**, browse your drawio folder in your downloads directory and select the XML file, then click on **Open**. Repeat for every additional XML file you wish to import.

- Confirm library or libraries are visible in the left panel:

![](images/ImportedLibraries.png)

</p>
</details>


<details><summary>Import using Github Clone</summary>
<p>

### Prerequistes

- A [GitHub.com account](https://github.com/).
- Git [CLI](https://gist.github.com/derhuerst/1b15ff4652a867391f03) or [GitHub Desktop](https://desktop.github.com/).
- An [SSH Key associated](https://help.github.com/en/githubauthenticating-to-github/adding-a-new-ssh-key-to-your-github-account) to the github.com account.
 
### Instructions

- Sign into [github](https://github.com/login?return_to=%2Fibm-cloud-architecture%2Fibm-cloud-stencils).
- While in the main [page](https://github.com/ibm-cloud-architecture/ibm-cloud-stencils), click the **Clone or download** button, select on **Use SSH** if not already selected (**Use HTTPS** will be displayed) and then copy the link using the copy symbol:

![](images/UseSSH.png)

- CD to directory where you wish to clone this repository.

- Clone the repository using **git clone** syntax using the previously copied ssh link:

```
$ git clone git@github.com:ibm-cloud-architecture/ibm-cloud-stencils.git
Cloning into 'ibm-cloud-stencils'...
Enter passphrase for key '/Users/youruserid/.ssh/id_rsa': 
```
- Enter the passphrase of your SSH key.

- Confirm repository was successfully cloned, the CLI should display something like this:

```
remote: Enumerating objects: 58893, done.
remote: Total 58893 (delta 0), reused 0 (delta 0), pack-reused 58893
Receiving objects: 100% (58893/58893), 185.09 MiB | 5.01 MiB/s, done.
Resolving deltas: 100% (18944/18944), done.
$ 
```
- Optionally use GitHub Desktop to Clone. In the main [page](https://github.com/ibm-cloud-architecture/ibm-cloud-stencils), click the **Clone or download** button, select on **Open in Desktop**, wait for the prompt and select/confirm launching the link using GitHub Desktop application. Confirm directory where repository will be cloned:

  ![](images/CloningUsingGHD.png)

  Click on **Clone** and wait for process to complete.

- Open the desktop [Draw.io application](https://github.com/jgraph/drawio-desktop/releases) in your computer or open [draw.io](https://www.draw.io/) in your browser.

- Select **Create New Diagram**, then click **Create**.

- Click on **File > Open Library**, browse your drawio folder in your cloned/local  directory and select the XML file, then click on **Open**. Repeat for every additional XML file you wish to import.

- Confirm library or libraries are visible in the left panel:

![](images/ImportedLibraries.png)

</p>
</details>

# Using IBM Cloud Stencils

## Overview

IBM Cloud Diagrams are organized by boxes (rectangular borders) with deployedOn and deployedTo relationships -

### DeployedOn Boxes

Represent a deployedOn relationship for locations (logical, virtual, physical) of platforms, infrastructure, network, etc, on which services and applications are deployed.

DeployedOn boxes have the following attributes:

- A solid border.
- Implemented as diagram containers (container=1).
- Icons added to box remain with box when box is moved or replicated.
- Placement is done before deployedTo boxes have been placed.
- Cannot cross multiple box boundaries.

DeployedOn boxes include IBM Cloud, Region, Zone, VPC, Subnet, etc.

### DeployedTo Boxes

Represent a deployedTo relationship for grouping services and applications.

DeployesTo boxes have the following attributes:  
	
- A dashed border.
- Not implemented as diagram containers (container=0).
- Icons are not included with box when box is moved or replicated.
- Placement is done after deployedOn boxes have been placed.
- Can cross multiple box boundaries.

DeployedTo boxes include Account Group, Instance Group, Namespace Group, Resource Group, Security Group, etc.

### Box Example

A virtual server instance is **deployed on** a subnet and **deployed to** a security group. 

### Icons

IBM Cloud Icons consist of:
- [Architecture Icons](https://www.ibm.com/cloud/architecture/architectures/edit) which represent IBM Cloud components by background color.
- [Service Icons](https://l2fprod.github.io/myarchitecture/) which represent services available in the IBM Cloud catalog.

## Examples

<details><summary>IBM VPC Diagram</summary>
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

4. When adding icons to diagrams the default background color for text should be transparent but instead may be white.  *See open issue #1 and #2.*

5. When exporting diagrams to svg ensure that icons are included (check Embed Image) if using svg offline and ensure white space is minimal (select entire diagram then check Selection Only and Crop) if embedding in a document.

Open Issues:

1. Issue #620 where setting the icon text background to transparent doesn't work.<br/>Status: Open.  This issue happens if labelBackgroundColor=none is before the image; statement in icon style, so place the labelBackgroundColor=none to anywhere after the image; statement.<br/>

2. Issue #839 to move labelBackgroundColor=none to after image; statement for IBM icons.<br/>
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

## Standards

<details><summary>Colors</summary>

| Style | Hex Color | RGB Color |
| :--- | :--- | :--- |
| Text (Helvetica 12 pt) | #000000 | 0,0,0 |
| Connectors (1 pt and 2 pt) | #000000 | 0,0,0 |
| Blue Borders | #4376BB | 67,120,187 |
| Light Blue Fill | #CDEBF9 | 80,92,98 |
| Green Borders | #00882B | 0,136,43 |
| Light Green Fill | #E6F0E2 | 230,240,226 |
| Grey Borders | #919191 | 145,145,145 |
| Light Grey Fill | #E0E0E0 | 224,224,224 |
| Purple Borders | #B99ACD | 185,154,205 |
| Light Purple Fill | #F0E8FF | 245,232,255 |
| Red Borders | #FF0000 | 255,0,0 |
| Gold Borders | #C4982E | 196,152,46 |

</details>

<details><summary>DeployedOn Boxes</summary>

| Name | Icon | Icon Name | Style | Width | Type |
| :--- | :--- | :--- | :--- | ---: | :--- |
| IBM Cloud | <img src="/images/CloudTag.png" width=25 /> | CloudTag | Solid Blue Border | 3 pt | Container | 
| VPC | <img src="/images/VPCTag.png" width=25 /> | VPCTag | Solid Blue Border | 2 pt | Container |
| Region | <img src="/images/RegionTag.png" width=25 /> | RegionTag | Solid Grey Border | 2 pt | Container |
| Zone | <img src="/images/ZoneTag.png" width=25 /> | ZoneTag | Solid Grey Border<br/>Light Grey Fill | 1 pt | Container |
| Subnet | <img src="/images/SubnetACLTag.png" width=25 /> | SubnetTag | Solid Green Border<br>Light Green Fill | 1 pt | Container |
| Bare Metal Server | <img src="/images/BareMetalServerTag.png" width=25 /> |BareServerTag |  Solid Green Border | 2 pt | Container |
| Virtual Server | <img src="/images/VirtualServerTag.png" width=25 /> | VirtualServerTag |  Solid Green Border| 2 pt | Container |
| Classic Infrastructure | <img src="/images/ClassicTag.png" width=25 /> | ClassicTag | Solid Blue Border | 2 pt | Container | 
| Public Network | <img src="/images/PublicTag.png" width=25 /> | PublicTag | Solid Blue Border | 3 pt | Container | 
| Enterprise Network | <img src="/images/EnterpriseTag.png" width=25> | EnterpriseTag | Solid Blue Border | 3 pt | Container | 
| Cloud Services | <img src="/images/ServicesTag.png" width=25> | CloudServiceTag | Solid Blue Border | 1 pt | Container |
| Cloud Foundry | <img src="/images/FoundryTag.png" width=25> | FoundryTag | Solid Blue Border | 2 pt | Container |
| IBM Kubernetes Cluster | <img src="/images/KubeClusterTag.png" width=25> | KubeTag |  Solid Blue Border | 2 pt | Container |
| General Kubernetes Cluster | <img src="/images/GeneralClusterTag.png" width=25> | GeneralKubeTag | Solid Blue Border | 2 pt | Container |
| OpenShift Cluster | <img src="/images/OpenShiftClusterTag.png" width=25> | OpenShiftTag |  Solid Blue Border | 2 pt | Container |
| Kubernetes Service | <img src="/images/KubeServiceTag.png" width=25> | KubeServiceTag | Solid Blue Border | 2 pt | Container |
| Kubernetes Replica Set | <img src="/images/KubeRSTag.png" width=25> | KubeReplicaTag | Solid Blue Border<br/>Light Blue Fill | 2 pt | Container |
| Kubernetes Pod | <img src="/images/KubePodTag.png" width=25> | KubePodTag | Solid Purple Border<br/>Light Purple Fill | 2 pt | Container |

</details>

<details><summary>DeployedTo Boxes</summary>

| Name | Icon | Icon Name | Style | Width | Type |
| :--- | :--- | :--- | :--- | ---: | :--- |
| Kubernetes Namespace Group | <img src="/images/NamespaceGroupTag.png" width=25> | KubeGroupTag | Dashed Blue Border | 2 pt | Non-container |
| Account Group | <img src="/images/AccountGroupTag.png" width=25> | AccountGroupTag | Dashed Gold Border | 2 pt | Non-container |
| Instance Group | <img src="/images/InstanceGroupTag.png" width=25> | InstanceGroupTag | Dashed Green Border | 2 pt | Non-container |
| Resource Group | <img src="/images/ResourceGroupTag.png" width=25> | ResourceGroupTag | Dashed Grey Border | 2 pt | Non-container |
| Security Group | <img src="/images/SecurityGroupTag.png" width=25> | SecurityGroupTag | Dashed Red Border | 2 pt | Non-container |

</details>
