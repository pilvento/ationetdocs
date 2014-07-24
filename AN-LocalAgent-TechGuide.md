![ATIONET](/Content/Images/ATIOnetLogo_250x70.png) 

***

# ATIOnet Local Agent Technical Guide

> **About:** This document provides setup and service instructions and background for the ATIOnet Local Agent, software-only version.    	

</br>

<table>
	<thead>
		<tr>
			<td colspan="2" class="tablehead">Document Information</td>
		</tr>
	</thead>
	<tfoot>
		<td colspan="2"> </td>
	</tfoot>
	<tbody>
		<tr>
			<td width="20%" class="rowhead" align="right">File:</td>
			<td>AN-LocalAgent-TechGuide.md</td>
		</tr>
		<tr>
			<td align="right">Doc. Version:</td>
			<td>1.0</td>
		</tr>
		<tr>
			<td align="right">Release Date:</td>
			<td>25/Jul/2014</td>
		</tr>
		<tr>
			<td align="right">Author:</td>
			<td>ATIO International LLC</td>
		</tr>
	</tbody>
</table>

<table>
     <thead>
          <tr>
          	<td colspan="3">Change Log</td>
          </tr>
     </thead>
     <tfoot>
          <td colspan="3"> </td>
     </tfoot>
     <tbody>
        <tr>
          	<td>Ver.</td>
            <td>Date</td>
            <td>Change summary</td>
        </tr>
        <!-- Insert a table row like this for each version -->
        <tr>
          	<td>1.0</td>
          	<td>25/Jul/2014</td>
          	<td>Initial version. Software-only product</td>
        </tr>
        <!-- End of version table row -->
     </tbody>
</table>
</br>

<!-- ###Table of Content -->


<!-- Optional Terms & Definition section -->
        
### Definitions	

<dl>
  <dt>Term</dt>
  <dd>Term's definition</dd>
</dl>

<!-- Content starts here -->
##Introduction

ATIOnet Local Agent is a gateway component that enables communication between a range of certified Capture Systems and ATIOnet Host, distributed by ATIO International as a software-only gateway or as a bundled software and hardware unit. 

The Local Agent provides the following services to the Capture System (CS):

- **Gateway service to ATIOnet Host with protocol conversion**. The CS connects to the Local Agent on a local or remote private network via a TCP/IP socket and the Local Agent forwards the messages to ATIOnet, including protocol conversion to ATIOnet Native Transaction Protocol.
- **Offline authorization**. In the case of a communication failure between the Local Agent and the ATIOnet Host, the Local Agent will continue to authorize and store transactions with the CS. Once the link is restablished, a re-synchronization is performed automatically and the on-line service is resumed.

> This document covers the software part of the ATIOnet Local Agent. Hardware setup and support topics for the bundled version are not included.

###Audience
This document is intended for technical support staff including the following:

- Field support technicians
- IT staff of Merchants with supported CS affiliated to ATIOnet
- IT staff of ATIOnet subscribers

###Scope
This document provides the following information about ATIOnet Local Agent software gateway

- Deployment scenarios
- Systems requirements
- Software download instructions
- Setup instructions
- Troubleshooting
- Problem reporting requirements

##Deployment scenarios
explicar que se puede instalar local en el sitio o en un servidor central y que puede atender a una o más terminales

##Systems requirements
| Requirement          | Description        |
| -------------------- | ------------       |
| Operating System     | Windows 7 or later - Windows server 2012 or later - |
| ...                      |                    |

##Software download instructions

##Setup instructions

##Troubleshooting
detección de problemas
donde están los logs
como reinstalo

##Problem reporting requirements
qué datos hay que mandar, logs etc. para reportar un problema
