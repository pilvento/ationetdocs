![ATIONET](Content/Images/ATIOnetLogo_250x70.png) 

***

# ATIOnet Identification Scenarios
> **About:** This document describes the different possible combination of steps and data request procedures to identify a cardholder that can be implemented on ATIOnet.
These capabilities may vary according to the capture device, protocol and susbscription model.  		

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
			<td>AN-Identification_Scenarios-TechGuide.en</td>
		</tr>
		<tr>
			<td align="right">Doc. Version:</td>
			<td>1.0</td>
		</tr>
		<tr>
			<td align="right">Release Date:</td>
			<td>20, July 2014</td>
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
          	<td>20/July/2014</td>
          	<td>Change description</td>
        </tr>
        <!-- End of version table row -->
     </tbody>
</table>
</br>

<!-- ###Table of Content -->


<!-- Optional Terms & Definition section -->
        
### Definitions	

<dl>
  <dt>Terminal</dt>
  <dd>Te device or system in charge of handling the interaction with the cardholder and/or the attendant</dd>
  <dt>Carholder</dt>
  <dd>The person, vehilce or unit who is identified as the subject of the transaction</dd>
  <dt>Sub-account</dt>
  <dd>A particular account whithin a Contract with an assigned balance</dd>
  <dt>Identification</dt>
  <dd>Device, media support or piece of information presented to a capture device in order to identify a cardholder</dd>

</dl>

<!-- Content starts here -->
## Overview ##
Every transaction on ATIOnet start with a secure identification of a sub-account to be debited or credit by the transaction. A sub-account can be a Vehicle -or broadly a Unit- or a Driver -broadly a Person.
On ATIOnet, every transaction impact to a one sub-account and one sub-account only, it is called a sub-account because it is always part of a Contrat (its parent account), but it is common to request two Identifications on the same transaction, usually to identify the Vehicle and the Driver or viceversa.

On ATIOnet Native Transaction Protocol, there are two Identification set of fields, a Primary ID and a Secondary ID, is up to the Terminal to decide which one is Primary or Secondary but the common practice is to send the ID presented first as the Primary. Most of the Terminals have the capability to capture a second ID and send it as a prompt on the authorization request, ATIOnet is capable of taking such prompt and processing it as a the secondary Identification.

It is important to only the sub-account linked to the Primary Identification will have their balance impacted for the transaction, the Secondary Identification will be used to perform a two-fold identification capture and may have the related entity affected on its statistics and counters, like quotas or mileage calculation but the money or volume sold will accounted to the Primary sub-account only.

## Relevant Configuration ##

### Prompting Rules ###
Some prompts when enforced via Rules can help with the Identification.
Terminals supporting re-prompt functionality can activate prompts of missing information dinamically reacting to specific decline codes received from the Host.

<dl>
  <dt>Truck Number</dt>
  <dd>Vehicle ID (Unit Code)</dd>
  <dt>Vehicle PIN</dt>
  <dd>Secure numeric value associated to the Vehicle</dd>
  <dt>Driver ID</dt>
  <dd>Driver Identification number, must match the Driver Code on the system</dd>
  <dt>Driver PIN</dt>
  <dd>Secure number associated to the Driver</dd>
</dl>

> Note about Vehicle and Driver ID data-type. ATIOnet supports alphanumeric values in Vehicles and Drivers, but if you plan to use them as IDs, take into consideration that most capture terminals doesn't accept string input at these prompts, so numeric-only values might be used instead.

### Terminal / Controller Configuration ###
The flag ```Use Driver Id as Driver Card Track``` parameter forces the system to pass the Driver ID prompt as a Secondary Track (secondary identification), instead of taking it as an information-only prompt. This is useful to implement a two-fold authentication on terminals that doesn't accept dual card-swipe.

### Enforced Vehicle-Driver relation ###
Vehicle can be linked to one or more Drivers and viceversa from the Vehicle and Driver administration tools. When the Primary sub-account is linked to another, ATIOnet will automatically enforce a two-fold authentication, meaning that both the Vehicle and the Driver should be identified successfully at capture time and the relation must be satisfied in order to the the transaction approved.

## Use of PINs ##
PINs are not an identification per-se, they are supporting mechanisms to validate that the individual present at capture time is rightfully in posession of the Vehicle and/or Driver ID numbers. Meaning that the actual data to be used as the record locators are the Vehicle ID or the Driver ID, the PINs only add a security layer on top of a solely manual entry.
Although the parameter is ```Vehicle PIN``` or ```Driver PIN```, the PIN is actually tied to the Identification (the card, hard-key, token, manual-entry etc.) and not directly to the Vehicle or Driver

## Scenarios ##

|Expected Identification behavior                     | Description / Configuration strategy                        |
|-----------------------------------------------------|------------------------------------------------------------|
|Single Vehicle                                       | Assign at least one Identification to a Vehicle-type sub-account|
|Single Driver| Idem to a Driver-type sub-account|
|Dual ID, Vehicle(s) enabled for a/some Driver(s)|Configure a relation between the Vehicle(s) and the Driver(s). The Vehicle balances, cummmulators, counters and mileage will be impacted; to the Drivers, only their cummulators will be affected|
|Dual ID, Driver(s) authorized for a/some Vehicle(s)|Configure a relation between the Drivers(s) and the Vehicles(s). The Driver(s) balances, cummmulators and counters will be impacted; to the Vehicles, only their cummulators and mileage will be modified. Only applies to Terminals with dual swipe capability|
|Single Vehicle card with Driver ID manual prompt|Transaction is completed against Vehicle's sub-account, Driver ID is informative|
Dual ID, Vehicle card with Driver ID manual prompt|If Terminal is configured to pass Driver ID as a secondary track, functions as a full dual ID scenario, validating the Vehicle ID and the Driver ID, if there are Vehicle/Driver relations configured those will be enforced.|
|Vehicle ID or Vehicle card plus Vehicle PIN|PIN entry used as an entry validation, must match the PIN for the Identification presented for the Vehicle. On a single Driver Identification scenario where the Vehicle ID is not required, if the Vehicle ID prompt is active the content of the field is ignored, as there is no Vehicle ID to validate.|
|Driver ID or Driver card plus Driver PIN|Same as Vehicle case above, but referred to Driver ID|






 

