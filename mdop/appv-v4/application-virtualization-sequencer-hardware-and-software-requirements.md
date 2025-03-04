---
title: Application Virtualization Sequencer Hardware and Software Requirements
description: Application Virtualization Sequencer Hardware and Software Requirements
author: dansimp
ms.assetid: c88a1b5b-23e1-4460-afa9-a5f37e32eb05
ms.reviewer: 
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop, appcompat, virtualization
ms.mktglfcycl: deploy
ms.sitesec: library
ms.prod: w8
ms.date: 06/16/2016
---


# Application Virtualization Sequencer Hardware and Software Requirements


This topic describes the minimum recommended hardware and software requirements for the computer running the Microsoft Application Virtualization (App-V) Sequencer.

**Important**  
You must run the App-V sequencer (**SFTSequencer.exe**) using an account that has administrator privileges because of the changes the sequencer makes to the local system. These changes can include writing files to the **C:\\Program Files** directory, making registry changes, starting and stopping services, updating security descriptors for files, and changing permissions.

 

Before you install the Sequencer and after you sequence each application, you must restore a clean operating system image to the sequencing computer. You can use one of the following methods to restore the computer running the Sequencer:

-   Reformat the hard drive and reinstall the operating system.

-   Restore the hard drive on the computer running the Sequencer image by using another disk-imaging software.

-   Revert a virtual operating system image such as a Microsoft Virtual PC image. Using a virtual machine allows for clean sequencing environments to be easily reused with minimal administration.

The following list outlines the recommended hardware requirements for running the App-V Sequencer.

The requirements are listed first for Microsoft Application Virtualization (App-V) 4.6 SP2, followed by the requirements for versions that preceded App-V 4.6 SP2.

### <a href="" id="hardware-requirements-"></a>Hardware Requirements

-   Processor—Intel Pentium III, 1 GHz (32-bit or 64-bit). The sequencing process is a single-threaded process and does not take advantage of dual processors.

-   Memory—1 GB or above, 2 GB recommended.

-   Hard disk—40 gigabyte (GB) hard disk space with a minimum of 15 GB available hard disk space. We recommend that you have at least three times the hard disk space that the application you are sequencing requires.

    **Note**  
    Sequencing requires heavy disk usage. A fast disk speed can decrease the sequencing time.

     

### Software Requirements for App-V 4.6 SP2

The following list outlines the supported operating systems for running the App-V 4.6 SP2 Sequencer.

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Operating System</th>
<th align="left">Edition</th>
<th align="left">Service Pack</th>
<th align="left">System Architecture</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Windows XP</p></td>
<td align="left"><p>Professional</p></td>
<td align="left"><p>SP3</p></td>
<td align="left"><p>x86</p></td>
</tr>
<tr class="even">
<td align="left"><p>Windows Vista</p></td>
<td align="left"><p>Business, Enterprise, or Ultimate</p></td>
<td align="left"><p>SP2</p></td>
<td align="left"><p>x86</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Windows 7</p></td>
<td align="left"><p>Professional, Enterprise, or Ultimate</p></td>
<td align="left"><p>No service pack or SP1</p></td>
<td align="left"><p>x86 and x64</p></td>
</tr>
<tr class="even">
<td align="left"><p>Windows 8</p></td>
<td align="left"><p>Pro or Enterprise Edition</p></td>
<td align="left"><p></p></td>
<td align="left"><p>x86 and x64</p></td>
</tr>
</tbody>
</table>

 

**Note**  
The Application Virtualization (App-V) 4.6 SP2 Sequencer supports 32-bit and 64-bit versions of these operating systems.

 

You should configure computers running the Sequencer with the same applications that are installed on targeted computers.

### Software Requirements for Versions that Precede App-V 4.6 SP2

The following list outlines the supported operating systems for running the Sequencer for versions that precede App-V 4.6 SP2.

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Operating System</th>
<th align="left">Edition</th>
<th align="left">Service Pack</th>
<th align="left">System Architecture</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Windows XP</p></td>
<td align="left"><p>Professional</p></td>
<td align="left"><p>SP2 or SP3</p></td>
<td align="left"><p>x86</p></td>
</tr>
<tr class="even">
<td align="left"><p>Windows Vista</p></td>
<td align="left"><p>Business, Enterprise, or Ultimate</p></td>
<td align="left"><p>No service pack, SP1, or SP2</p></td>
<td align="left"><p>x86</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Windows 7¹</p></td>
<td align="left"><p>Professional, Enterprise, or Ultimate</p></td>
<td align="left"><p></p></td>
<td align="left"><p>x86</p></td>
</tr>
</tbody>
</table>

 

¹Supported for App-V 4.5 with SP1 or SP2, and App-V 4.6 only

**Note**  
The Application Virtualization (App-V) 4.6 Sequencer supports 32-bit and 64-bit versions of these operating systems.

 

You should configure computers running the Sequencer with the same applications that are installed on targeted computers.

### Software Requirements for Remote Desktop Services for App-V 4.6 SP2

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Operating System</th>
<th align="left">Edition</th>
<th align="left">Service Pack</th>
<th align="left">System Architecture</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Windows Server 2003 R2</p></td>
<td align="left"><p>Standard Edition, Enterprise Edition, or Datacenter Edition</p></td>
<td align="left"><p>SP2</p></td>
<td align="left"><p>x86</p></td>
</tr>
<tr class="even">
<td align="left"><p>Windows Server 2008</p></td>
<td align="left"><p>Standard, Enterprise, or Datacenter Edition</p></td>
<td align="left"><p>SP2</p></td>
<td align="left"><p>x86</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Windows Server 2008 R2</p></td>
<td align="left"><p>Standard, Enterprise, or Datacenter Edition</p></td>
<td align="left"><p>No service pack or SP1</p></td>
<td align="left"><p>x64</p></td>
</tr>
<tr class="even">
<td align="left"><p>Windows Server 2012</p></td>
<td align="left"><p>Standard, Enterprise, or Datacenter Edition</p></td>
<td align="left"><p></p></td>
<td align="left"><p>x86 or x64</p></td>
</tr>
</tbody>
</table>

 

**Note**  
Application Virtualization (App-V) 4.6 SP2 for Remote Desktop Services supports 32-bit and 64-bit versions of these operating systems.

 

### Software Requirements for Remote Desktop Services for Versions that Precede App-V 4.6 SP2

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Operating System</th>
<th align="left">Edition</th>
<th align="left">Service Pack</th>
<th align="left">System Architecture</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Windows Server 2003</p></td>
<td align="left"><p>Standard Edition, Enterprise Edition, or Datacenter Edition</p></td>
<td align="left"><p>SP1 or SP2</p></td>
<td align="left"><p>x86</p></td>
</tr>
<tr class="even">
<td align="left"><p>Windows Server 2003 R2</p></td>
<td align="left"><p>Standard Edition, Enterprise Edition, or Datacenter Edition</p></td>
<td align="left"><p>No service pack or SP2</p></td>
<td align="left"><p>x86</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Windows Server 2008</p></td>
<td align="left"><p>Standard, Enterprise, or Datacenter Edition</p></td>
<td align="left"><p>SP1 or SP2</p></td>
<td align="left"><p>x86</p></td>
</tr>
<tr class="even">
<td align="left"><p>Windows Server 2008 R2</p></td>
<td align="left"><p>Standard, Enterprise, or Datacenter Edition</p></td>
<td align="left"><p>No service pack or SP1</p></td>
<td align="left"><p>x64</p></td>
</tr>
</tbody>
</table>

 

**Note**  
Application Virtualization (App-V) 4.6 SP2 for Remote Desktop Services supports 32-bit and 64-bit versions of these operating systems.

 

## Related topics


[Application Virtualization Client Hardware and Software Requirements](application-virtualization-client-hardware-and-software-requirements.md)

[Application Virtualization System Requirements](application-virtualization-system-requirements.md)

[How to Install the Application Virtualization Sequencer](how-to-install-the-application-virtualization-sequencer.md)

[How to Upgrade the Application Virtualization Sequencer](how-to-upgrade-the-application-virtualization-sequencer.md)

 

 





