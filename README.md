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

# IBM Cloud Stencils for VPC

## Overview

IBM VPC diagrams are designed to organize a VPC solution to visually show the functionality and availability of the IBM VPC platform.    

![VPCArchitecture](/images/ibm_vpc_architecture_power_drawio.png)

To automate creation of Terraform for IBM Virtual Private Cloud refer to [Terraformer](https://github.com/ibm-cloud-architecture/terraformer).

## General Notes

1. Instance Group feature is not currently available. 
2. IBM VPC has a single subnet type Subnet.
3. Subnet:ACL denotes a Subnet with an associated ACL which can be customized such as SubnetName:ACLName, SubnetCIDR:ACLName, split to 2 lines, etc.
4. Diagram containers if available in a tool (draw.io and Visio) are used for primary boxes but not secondary boxes.  Secondary boxes are Instance Group, Resource Group, and Security Group.  
5. To migrate existing boxes to latest boxes, apply box styles from new boxes to existing diagram.  For draw.io, updating styles in existing containerless diagrams won't take advantage of containerized styles but using the grouping feature creates container-like behavior if desired.

## draw.io Notes

1. To use the IBM Stencils on draw.io in your browser: https://draw.io/?libs=ibm
2. To use the IBM Stencils on the [draw.io desktop application](https://github.com/jgraph/drawio-desktop/releases) do the following:

   1. Open application and click on "+ More Shapes" in the bottom left panel.
   2. Scroll down to the "Networking" section and check "IBM".
   3. Click "Apply" to finish.

   IBM Stencils should now be available in the embedded categories in the left panel.
3. Template named ibm_vpc_architecture under Cloud on draw.io is currently outdated.
4. Folders for draw.io on this github are used for changes not on draw.io.
5. Primary boxes are containers (container=1) and secondary boxes are not containers (container=0).  Secondary boxes are Instance Group, Resource Group, and Security Group.  Temporary step to set container=0 (in style or uncheck property) for the secondary boxes.  *See open issue #2.*
6. Changing box border color will also change tag color allowing customization with other preferred colors, but note that deviating from standards below might conflict with boxes/colors added to the stencils in the future.
7. Changing box border color to white on white background makes the box appear invisible, so for example if used for Public Network and Enterprise Network boxes to hide borders while still taking advantage of their containers.
8. When adding icons to diagrams the default background color for text should be transparent but instead may be white.  *See open issue #1.*
9. When exporting diagrams to svg ensure that icons are included (check Embed Image) if using svg offline and ensure white space is minimal (select entire diagram then check Selection Only and Crop) if embedding in a document.


### draw.io Issues

Open Issues:
1. Issue #620 where setting the icon text background to transparent doesn't work.  Status: Found that this previously worked, so provided example in issue of a working style and a non-working style.
2. Issue #748 to remove container setting for 3 secondary boxes.  Status: Open.

Fixed Issues:
1. Issue #724 where icons dropped onto a container would not stay in the container when the container is moved.  The problem was only on FF browser.
2. Issue #723 where overlaying a box across other boxes may cause underlying boxes to expand and have to be resized such as when placing a security group box across multiple subnet boxes.  This scenario is working as designed so draw.io added a new property "expand" to swimlanes for our boxes.  The current behavior is the default with expand=1 and our boxes are set to expand=0.

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
| Subnet | Solid Green Border (a)<br>Light Green Fill | 1 pt | Container |
| Cloud Services | Solid Blue Border | 1 pt | Container |
| Instance Group | Dashed Green Border | 2 pt | Non-container |
| Resource Group | Dashed Grey Border | 2 pt | Non-container |
| Security Group | Dashed Red Border | 2 pt | Non-container |

Notes:

a. Subnet can optionally be changed to Solid Red Border to highlight exposed resources.
