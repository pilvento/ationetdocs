![ATIONET](Content/Images/Logo.png)

##ATIONet Native Interface API Protocol Specification##

<table>
	<tr>
		<th colspan="2" align="left">
			Document Information
		</th>
	</tr>
	<tr>
		<td>
			File:
		</td>
		<td>
			ATIONet-Native_Interface_Protocol_Spec-v1.3
		</td>
	</tr>
	<tr>
		<td>
		 Doc Version:
		</td>
		<td>
		 1.3
		</td>
	</tr>
	<tr>
		<td>
		 Release Date:
		</td>
		<td>
		 05, July 2014
		</td>
	</tr>
	<tr>
		<td>
		 Author:
		</td>
		<td>
		 ATIO International LLC
		</td>
	</tr>
</table>

<table>
	<tr>
		<th colspan="3" align="left">
			Change Log
		</th>
	</tr>
	<tr>
		<td>Ver.
		</td>
		<td>Date
		</td>
		<td>Change Summary
		</td>
	</tr>
	<tr valign="top">
		<td width="36" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western"><span lang="es-AR">1.0</span></p>
		</td>
		<td width="84" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western"><span lang="es-AR">04/Jan/2013</span></p>
		</td>
		<td width="404" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western" style="margin-bottom: 0.21cm">Initial version. 
			</p>
			<p class="western">General information	<br>Actions: Statement
			Charges (partial)	<br>	 Transactions Download</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="36" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western"><span lang="es-AR">1.1</span></p>
		</td>
		<td width="84" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western"><span lang="es-AR">07/Jan/2013</span></p>
		</td>
		<td width="404" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western" style="margin-bottom: 0.21cm">Statement
			Charges	<br>- Added Action 902 Negative Balance transfer to a
			sub-account</p>
			<p class="western" style="margin-bottom: 0.21cm">New group of
			actions: 941 &ndash; 950 Account Inquiries (partial)	<br>Actions:
			941 Sub-account Balance Enquiry	<br> 	 942 Sub-account Limit
			Enquiry</p>
			<p class="western">Transactions Downloads	<br>- Consolidated
			Classification Fields for Vehicles and Drivers	 <br>- Reorganized
			Response record, moved Classification fields after Driver Fields.</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="36" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">1.2</p>
		</td>
		<td width="84" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">30/10/2013</p>
		</td>
		<td width="404" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western" style="margin-bottom: 0.21cm">Account
			Inquiries	<br>- Added Action 943 Contract Balance Enquiry</p>
			<p class="western">New group of actions: 951 &ndash; 959 Account
			Download (partial)	<br>Actions: 951 Sub-Account Movements
			Download	<br> 	  952 Contract Movements Download</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="36" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">1.3</p>
		</td>
		<td width="84" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">05/07/2014</p>
		</td>
		<td width="404" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p style="margin-bottom: 0cm"><b>Statement Charges</b>	<br>- Added
			Action 903 Transfer balance from sub-account to a sub-account</p>
			<p style="margin-bottom: 0cm">- Added Action 904 Transfer balance
			from contract to a sub-account</p>
			<p style="margin-bottom: 0cm">- Added Action 905 Transfer balance
			from sub-account to a contract</p>
			<p class="western" style="margin-bottom: 0.21cm">- Change and
			reorganize request and response records</p>
			<p class="western" style="margin-bottom: 0.21cm"><b>Transactions
			Downloads</b>	<br>- Change and reorganize request and response
			records</p>
			<p style="margin-bottom: 0cm"><b>Account Inquiries</b>	<br>-
			Remove Action 943 Contract Balance Enquiry</p>
			<p class="western" style="margin-bottom: 0.21cm">- Change and
			reorganize request and response records</p>
			<p style="margin-bottom: 0cm"><b>Account Downloads</b>	<br>-
			Remove Action 952 Contract Movements Download</p>
			<p style="margin-bottom: 0cm">- Change Action 951 Sub-Account
			Movements Download to 951 Movements Download</p>
			<p class="western" style="margin-bottom: 0.21cm">- Change and
			reorganize request and response records</p>
			<p style="margin-bottom: 0cm"><b>Error Handling</b></p>
			<p class="western">- Include &ldquo;ResponseError&rdquo; in
			response record for actions intended to post a command            
			              
			</p>
		</td>
	</tr>
</table>

**Contents**

[1 Scope](#1--scope)

>[1.1 Scope details](#11--scope-details)

[2 System Interface API](#__RefHeading__3490_1617151515)

>[2.1 Interface API Messages](#__RefHeading__3492_1617151515)

[3 Data security](#__RefHeading__3494_1617151515)

[4 Message Structure](#__RefHeading__3496_1617151515)

[5 Error handling](#__RefHeading__3498_1617151515)

[6 Statement Charges Interface](#__RefHeading__3500_1617151515)

>[6.1 Action Codes](#__RefHeading__3502_1617151515)

>[6.2 Identification](#__RefHeading__3504_1617151515)

>[6.3 Statement Charge (POST) – Body Section Record Format](#__RefHeading__3506_1617151515)

[7 Transactions Download Interface](#__RefHeading__3508_1617151515)

>[7.1 Action Codes](#__RefHeading__3510_1617151515)

>[7.2 Transactions Download (POST) – Body Section Format Request](#__RefHeading__3512_1617151515)

>[7.3 Transactions Download (POST) – Body Section Format Response](#__RefHeading__3514_1617151515)

[8 Account Enquiries](#__RefHeading__3516_1617151515)

>[8.1 Action Codes](#__RefHeading__3518_1617151515)

>[8.2 Identification](#__RefHeading__3520_1617151515)

>[8.3 Account Enquiry (POST) – Body Section Record Format Request](#__RefHeading__3522_1617151515)

>[8.4 Account Enquiry (POST) – Body Section Record Format Response](#__RefHeading__3524_1617151515)

[9 Account Downloads](#__RefHeading__3526_1617151515)

>[9.1 Action Codes](#__RefHeading__3528_1617151515)

>[9.2 Account Download (POST) – Body Section Format Request](#__RefHeading__3530_1617151515)

>[9.3 Account Download (POST) – Body Section Format Response](#__RefHeading__3532_1617151515)

####Overview####

#####Introduction#####

This specification is intended to document ATIONet’s Native Interface
API messaging format and related features required for the systems
applying for integration with ATIONet.

The Interface API allows the The following sections provide descriptions
of the messages themselves, the expected behaviour for each supported
action type and a common ground for the functionality of each relevant
item.

#####Definitions#####

######Subscriber.######
ATIONet’s subscription owner. The person or company who
runs the service.

######Homebase.######
A type of ATIONet subscription where the subscriber owns
the site(s) but also the fleet(s) of vehicles.

######Network.######
A type of ATIONet subscription where the subscriber enrolls
Fleet Companies and retail or commercial sites to operate with its own
method-of-payment. The Network company doesn’t own the site(s) or the
vehicles.

######Retail.######
A type of ATIONet subscription where the subscriber owns the
sites and enrolls Fleet Companies to operate with its own
method-of-payment.

######Merchant.######
On a Network type subscription, the Merchant is the
company who own the sites.

######Company.######
On a Network or Retail type subscription, the Company is
the company who own the fleet.

######Terminal.######
Transaction capture device at the site.

####1 Scope####

Version 1.3 of this document covers a particular version of ATIONet’s
Host protocol. Although feature’s descriptions are generally not related
to a particular version of the protocol, some changes may apply which
would be specifically commented and identified on each feature’s
description paragraph.

#####1.1 Scope details:#####

Protocol: ATIONet Native Interface API

Version: Version 1.3

API URI: native.ationet.com/v1/interface\

####2 System Interface API####

The Interface API provide system-to-system access to certain features of
ATIONet otherwise only available via the ATIONet Console, and it’s
intended to allow direct interaction of third-party systems on
Subscribers, Merchants and fleet Companies with ATIONet.

Availability of part or all the functionality of the Interface API is
subject to the business type and contract terms of the ATIONet
subscriber.

#####2.1 Interface API Messages#####

<table>
	<thead>
		<tr valign="center">
			<th rowspan="2" align="left">Name
			</th>
			<th colspan="2" align="center">Protocol Ver.
			</th>
			<th  rowspan="2" align="left">Description
			</th>
		</tr>
  <tr valign="top">
    <th align="center">Initial
    </th>
    <th align="center">Change
    </th>
  </tr>
	</thead>
	<tbody>
		<tr valign="top">
			<td rowspan="3"  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0.21cm">Statement
				charges [HTTP POST]</p>
				<p class="western" align="left">901 to 920</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center">1.0</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center" style="margin-bottom: 0.21cm"><br><br>
				</p>
				<p class="western" align="center" style="margin-bottom: 0.21cm"><br><br>
				</p>
				<p class="western" align="center"><br>
				</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0.21cm">Commands
				ATIONet to process a movement on the account of a driver or
				vehicle, given an action type indicated on the message body. 
				</p>
				<p class="western" align="left" style="margin-bottom: 0.21cm">Availability
				of this message and the type of actions allowed depend on the
				subscriber type and its contracting terms.</p>
				<p class="western" align="left">901 - Balance transfer to a
				sub-account</p>
			</td>
		</tr>
		<tr valign="top">
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center">1.1</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center"><br>
				</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">902 - Balance withdrawal from a
				sub-account</p>
			</td>
		</tr>
		<tr valign="top">
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center"><br>
				</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center">1.3</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0.21cm">901
				- Balance transfer to a sub-account</p>
				<p class="western" align="left" style="margin-bottom: 0.21cm">902
				- Balance withdrawal from a sub-account</p>
				<p class="western" align="left" style="margin-bottom: 0.21cm">903
				- Transfer balance from sub-account to a sub-account</p>
				<p class="western" align="left" style="margin-bottom: 0.21cm">904
				- Transfer balance from contract to a sub-account</p>
				<p class="western" align="left">905 - Transfer balance from
				sub-account to a contract</p>
			</td>
		</tr>
		<tr valign="top">
			<td rowspan="3"  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0.21cm">Transactions
				Download<br>[HTTP POST]</p>
				<p class="western" align="left">931 to 940</p>
			</td>
			<td rowspan="2"  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center">1.0</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center"><br>
				</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0.21cm">Returns
				a list of completed transactions from ATIONet host, between two
				dates, for a given Subscriber, Merchant or fleet Company</p>
				<p class="western" align="left" style="margin-bottom: 0.21cm">931
				- Transactions Download</p>
				<p class="western" align="left">932 - Transactions Download for
				Merchants</p>
			</td>
		</tr>
		<tr valign="top">
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center">1.1</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0.21cm">931
				- Transactions Download</p>
				<p class="western" align="left">932 - Transactions Download for
				Merchants</p>
			</td>
		</tr>
		<tr valign="top">
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center"><br>
				</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center">1.3</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0.21cm">931
				- Transactions Download</p>
				<p class="western" align="left">932 - Transactions Download for
				Merchants</p>
			</td>
		</tr>
		<tr valign="top">
			<td rowspan="3"  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0.21cm">Account
				Enquiries<br>[HTTP POST]</p>
				<p class="western" align="left">941 to 950</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center">1.1</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center"><br>
				</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0.21cm">Returns
				specific values of a Contract or Sub-account.</p>
				<p class="western" align="left" style="margin-bottom: 0.21cm">941
				- Sub-account Balance Enquiry	</p>
				<p class="western" align="left">942 - Sub-Account Limit Enquiry</p>
			</td>
		</tr>
		<tr valign="top">
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center">1.2</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center"><br>
				</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">943 - Contract Balance Enquiry</p>
			</td>
		</tr>
		<tr valign="top">
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center"><br>
				</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center">1.3</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0.21cm">941
				- Sub-account Balance Enquiry	</p>
				<p class="western" align="left" style="margin-bottom: 0.21cm">942
				- Sub-Account Limit Enquiry</p>
				<p class="western" align="left"><font color="#ff0000"><strike>943
				- Contract Balance Enquiry</strike></font></p>
			</td>
		</tr>
		<tr valign="top">
			<td rowspan="2"  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0.21cm">Account
				Downloads<br>[HTTP POST]</p>
				<p class="western" align="left">951 to 960</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center">1.2</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center"><br>
				</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0.21cm">951
				- Sub-Account Movements Download 
				</p>
				<p class="western" align="left">952 - Contract Movements
				Download<br><br>
				</p>
			</td>
		</tr>
		<tr valign="top">
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center"><br>
				</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="center">1.3</p>
			</td>
			<td  style="border: 1px solid #000001; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0.21cm">951
				- Movements Download 
				</p>
				<p class="western" align="left" style="margin-bottom: 0.21cm"><font color="#ff0000"><strike>951
				- Sub-Account Movements Download</strike></font></p>
				<p class="western" align="left"><font color="#ff0000"><strike>952
				- Contract Movements Download</strike></font><font color="#ff0000">
				</font>
				</p>
			</td>
		</tr>
	</tbody>
</table>

####3 Data security####

The Interface API requires an SSL connection between both parties. The
SSL connection is established for each request/response pair, using a
certificate property of ATIONet, meaning that each request must include
a system-type user and password on the Header. The user will be matched
against the related ATIONet actor for each message. (for example: when a
Transactions Download request is received, the Interface will first
check whether the company of the authenticated user matches with the
Company code in the request).

Users to be used on the Interface API messaging will be created by
authorized users via ATIONet Console, with the role “Interface API”.

At this time there is no provisioning to distribute or update
certificates or thumbprint thru a system interface. This information
will be provided at request of the Subscriber.

####4 Message Structure####

All Interface API messages share the same structure, what change from
message to message are the Action Code, which indicates the actual
interface function, the value fields sent and received, and the HTTP
action (POST, GET, REQUEST) which changes depending on the Action Code.

Both, requests and responses use a JSON format.

Only one request is accepted on each message, although some requests and
many responses will contain multiple records.

#####Request Format#####

*Header:*

Accept-Encoding: gzip

Authorization: Basic user:password

*Body:*

{“ActionCode”:”nnn”,”FieldName”:”StringValue”,”FieldName”:Value}

#####Response#####

*Header:*

Content-Type: application/json; charset=utf-8

*Body:*

[{“Fieldname”:”StringValue”,”FieldName”:”StringValue”,”FieldName”:Value},
{“Fieldname”:”StringValue”,”FieldName”:”StringValue”,”FieldName”:Value}]


Note: Some Action Codes returns a single response row, for example the
Statement charges.

Note: Alphanumeric fields, stated as Type “A/N” in record format tables
below show the maximum possible length as the Size, although in
JSON-formatted strings they will be represented with trailing spaces
trimmed.

####5 Error handling#####

Success/failure exits on the Interface API will be handled via HTTP
status codes.

Successful request will get a HTTP 200 and the resulting response.

Actions intended to return data, for example the Transactions Downloads
group may return many records, just a single record or even no records
at all and even though will be considered successful if the requests met
the validation criteria. These Actions will always return a
JSON-formatted list of records, enclosed in curly brackets “[…]”. An
empty response will contain [] as body.

Actions intended to post a command, for example the Statement Charges
group will return a single JSON-formatted item with the “ResponseCode”,
“ResponseMessage” and “ResponseError” fields. The body of these
responses will never be empty.

Failure to process the request will be indicated by an HTTP 400’s range
status code. The body will contain a single JSON-formatted item with the
“ResponseCode”, “ResponseMessage” and “ResponseError” fields.

####6 Statement Charges Interface####

The Statement Charge message sends an instruction to ATIONet to apply a
well-defined action on the current account subsystem, the subject of the
action will be a sub-account of a contract, lets say a Vehicle or a
Driver account.

Depending on the type of charge, this message might be used by one or
the other party of the contract (the subscriber or the fleet company).

#####6.1 Action Codes#####

The Action Code specifies the type of accounting transactions requested
by a Statement Charge Message. The submitted code must match one of the
pre-defined operation types. Not all operation types are available for
all subscribers and/or fleet companies, availability depends on
subscription types but also on contract terms with ATIONet.

<table>
	<tr valign="top">
		<th align="left">Action Code
		</th>
		<th colspan="2" align="left">Description
		</th>
	</tr>
	<tr valign="top">
		<td rowspan="3" width="41" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">901</p>
		</td>
		<td width="145" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Title:</p>
		</td>
		<td width="338" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Balance transfer to a sub-account</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="145" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Function:</p>
		</td>
		<td width="338" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western" style="margin-bottom: 0.21cm">Transfers a given
			value from the global balance of the Contract to the sub-account
			related to the Vehicle or Driver.</p>
			<p class="western">Contract Balance must have enough funds (or
			product volume) to allow the transfer; otherwise the action will
			be rejected by the current accounts subsystem.</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="145" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Observations</p>
		</td>
		<td width="338" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">The action will first trigger a Deposit action
			on the Contract and the Contract to sub-account transfer.</p>
		</td>
	</tr>
	<tr valign="top">
		<td rowspan="2" width="41" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">902</p>
		</td>
		<td width="145" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Title:</p>
		</td>
		<td width="338" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Balance withdrawal from a sub-account</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="145" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Function:</p>
		</td>
		<td width="338" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western" style="margin-bottom: 0.21cm">Withdraws a given
			value from the sub-account related to the Vehicle or Driver.</p>
			<p class="western">Sub-account Balance must have enough funds (or
			product volume) to allow the withdrawal; otherwise the action will
			be rejected by the current accounts subsystem.</p>
		</td>
	</tr>
	<tr valign="top">
		<td rowspan="2" width="41" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">903</p>
		</td>
		<td width="145" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Title:</p>
		</td>
		<td width="338" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Balance transfer from sub-account to
			sub-account</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="145" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Function:</p>
		</td>
		<td width="338" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western" style="margin-bottom: 0.21cm">Transfers a given
			value from the original sub-account (related to the Original
			Vehicle or Driver) to the sub-account related to the Vehicle or
			Driver.</p>
			<p class="western">Original sub-account balance must have enough
			funds (or product volume) to allow the transfer; otherwise the
			action will be rejected by the current accounts subsystem.</p>
		</td>
	</tr>
	<tr valign="top">
		<td rowspan="2" width="41" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">904</p>
		</td>
		<td width="145" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Title:</p>
		</td>
		<td width="338" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Balance transfer from contract to sub-account</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="145" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Function:</p>
		</td>
		<td width="338" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western" style="margin-bottom: 0.21cm">Transfers a given
			value from the contract to the sub-account related to the Vehicle
			or Driver.</p>
			<p class="western">Contract balance must have enough funds (or
			product volume) to allow the transfer; otherwise the action will
			be rejected by the current accounts subsystem.</p>
		</td>
	</tr>
	<tr valign="top">
		<td rowspan="2" width="41" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">905</p>
		</td>
		<td width="145" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Title:</p>
		</td>
		<td width="338" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Balance transfer from sub-account to contract</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="145" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Function:</p>
		</td>
		<td width="338" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western" style="margin-bottom: 0.21cm">Transfers a given
			value from the sub-account related to the Vehicle or Driver to the
			contract.</p>
			<p class="western">Sub-account Balance must have enough funds (or
			product volume) to allow the withdrawal; otherwise the action will
			be rejected by the current accounts subsystem.</p>
		</td>
	</tr>
</table>

#####6.2 Identification#####

When a Statement Charge is received, ATIONet will try to identify the
Subscriber, the Species (Currency Code or Master Fuel Code) and the
Identifier of the sub-account (Vehicle or Driver), this can be performed
thru several combinations of the Identification Fields on the body of
the message:

1.  Any Identifier field (Identifier, Driver Code, Vehicle Code, Vehicle
    Plate, SubAccount External Code and SubAccount Id) only. Only
    accepted for Home-base subscriptions.

2.  Company Code + Identifier.

3.  Company Code + Contract Code + (Driver Code or Vehicle Code or
    Vehicle Plate)

#####6.3 Statement Charge (POST) – Body Section Record Format#####

<table>
	<thead>
		<tr valign="top">
			<th align="left">Field Name
			</th>
			<th align="left">Size
			</th>
			<th align="left">Type
			</th>
			<th align="left">Condition
			</th>
			<th align="left">Descriptions/Field Value(s)
			</th>
		</tr>
	</thead>
	<tbody>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">SubscriberCode</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">3</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Required</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Fixed. To be assigned by ATIONet</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">ActionCode</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">3</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Required</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Operation type code. <br>See
				Action Code Section.</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">CompanyCode</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">30</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">ContractCode</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">20</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">DriverCode</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">VehicleCode</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">VehiclePlate</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">SubAccountExternalCode</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">SubAccountId</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">36</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Identifier</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0cm">Public
				ID of the identification device (chipkey ID, account number on a
				mag card, RFID serial number, etc.)</p>
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">DriverCodeOrigin</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">VehicleCodeOrigin</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">VehiclePlateOrigin</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">SubAccountExternalCodeOrigin</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">SubAccountIdOrigin</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">36</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">IdentifierOrigin</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0cm">Public
				ID of the identification device (chipkey ID, account number on a
				mag card, RFID serial number, etc.)</p>
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">MasterFuelCode</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Conditional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Required if Charge Volume is
				specified</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">CurrencyCode 
				</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Conditional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Required if Charge Amount is
				specified</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Amount</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">10</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Required</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Charge Amount or Charge Volume 
				</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="186" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Description</p>
			</td>
			<td width="30" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">1000</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="168" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A description for the current
				account movement</p>
			</td>
		</tr>
	</tbody>
</table>

####7 Transactions Download Interface####

The Transactions Download Interface are POST actions to recover all the
payment transactions processed by ATIONet for a given Terminal, Contract
Code or Company Code depending on the particular Action Code.

The Action Code is validated against the type of company of the
authenticated user. Request not passing this validation will be
rejected.

The download will be limited by dates (from and to), which must be
included in the request

#####7.1 Action Codes#####

The Action Code specifies the type of record transaction to be
retrieved; this differentiation is based on the different roles on an
ATIONet operation (Fleet Company, Merchant, Network, Home-base), which
also mandates different ways to identify the requester and scope of
transactions to download.

<table>
	<tr valign="top">
		<th align="left">Action Code
		</th>
		<th colspan="2" align="left">Description
		</th>
	</tr>
	<tr valign="top">
		<td rowspan="4" width="54" height="20" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">931</p>
		</td>
		<td width="84" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Title:</p>
		</td>
		<td width="374" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Transactions Download 
			</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="84" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Function:</p>
		</td>
		<td width="374" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Download complete transactions records</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="84" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Allowed for:</p>
		</td>
		<td width="374" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Subscribers and Fleet Companies</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="84" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Identification:</p>
		</td>
		<td width="374" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western" style="margin-bottom: 0.21cm">Subscriber Code</p>
			<p class="western" style="margin-bottom: 0.21cm">Merchant Code
			(Optional, if included will act as a filter)</p>
			<p class="western" style="margin-bottom: 0.21cm">Company Code
			(Optional, if included will act as a filter)</p>
			<p class="western" style="margin-bottom: 0.21cm">Terminal
			Code(Optional, if included will act as a filter)</p>
			<p class="western">Contract Code (Optional, if included will act
			as a filter)</p>
		</td>
	</tr>
	<tr valign="top">
		<td rowspan="4" width="54" height="19" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">932</p>
		</td>
		<td width="84" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Title:</p>
		</td>
		<td width="374" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Transactions Download for Merchants</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="84" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Function:</p>
		</td>
		<td width="374" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Download transactions records (fueling details
			subset)</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="84" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Allowed for:</p>
		</td>
		<td width="374" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Merchants on a three-layer subscription model</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="84" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Identification:</p>
		</td>
		<td width="374" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western" style="margin-bottom: 0.21cm">Subscriber Code</p>
			<p class="western" style="margin-bottom: 0.21cm">Merchant Code 
			</p>
			<p class="western">Terminal Code (Optional, if included will act
			as a filter)</p>
		</td>
	</tr>
</table>

#####7.2 Transactions Download (POST) – Body Section Format *Request*#####

<table>
	<thead>
		<tr valign="top">
			<th align="left">Field Name
			</th>
			<th align="left">Size
			</th>
			<th align="left">Type
			</th>
			<th align="left">Condition
			</th>
			<th align="left">Descriptions/Field Value(s)
			</th>
		</tr>
	</thead>
	<tbody>
		<tr valign="top">
			<td width="100" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">SubscriberCode</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">3</p>
			</td>
			<td width="37" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="76" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Required</p>
			</td>
			<td width="239" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Fixed. To be assigned by ATIONet</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="100" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">ActionCode</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">3</p>
			</td>
			<td width="37" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">N</p>
			</td>
			<td width="76" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Required</p>
			</td>
			<td width="239" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Action Codes section above</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="100" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">MerchantCode</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">30</p>
			</td>
			<td width="37" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="76" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Conditional</p>
			</td>
			<td width="239" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Action Codes section above</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="100" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">CompanyCode</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">30</p>
			</td>
			<td width="37" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="76" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Conditional</p>
			</td>
			<td width="239" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Action Codes section above</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="100" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">ContractCode</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">20</p>
			</td>
			<td width="37" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="76" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="239" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Action Codes section above</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="100" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">TerminalCode</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="37" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="76" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="239" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Action Codes section above</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="100" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">DateFrom</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">19</p>
			</td>
			<td width="37" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="76" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Required</p>
			</td>
			<td width="239" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0cm">From
				date to filter transactions</p>
				<p class="western" align="left">&ldquo;yyyy/MM/dd hh:mm:ss&rdquo;</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="100" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">DateTo</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">19</p>
			</td>
			<td width="37" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="76" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="239" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0cm">To
				date to filter transactions</p>
				<p class="western" align="left">&ldquo;yyyy/MM/dd hh:mm:ss&rdquo;</p>
			</td>
		</tr>
	</tbody>
</table>

#####7.3 Transactions Download (POST) – Body Section Format *Response*#####

<table>
	<thead>
		<tr valign="top">
			<th align="left">Field Name
			</th>
			<th align="left">Size
			</th>
			<th align="left">Type
			</th>
			<th align="left">Descriptions/Field Value(s)
			</th>
		</tr>
	</thead>
	<tbody>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">TransactionID</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">36</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Transaction&rsquo;s UID</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubscriberCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">3</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Code of the subscriber who owns the
				transaction</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">TransactionSequenceNumber</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Transaction ID as received from the site&rsquo;s
				controller system. Usually a transaction counter. Site-based,
				might repeat from site to site.</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">AuthorizationCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Authorization Code</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">ResponseCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">5</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Host response code sent to the terminal</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">ResponseMessage</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Host response text sent to the terminal</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Status</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">1</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">2- &ldquo;Completed&rdquo;, 3- &ldquo;Confirmed&rdquo;</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">StatusDescription</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">&ldquo;Completed&rdquo;
				or &ldquo;Confirmed&rdquo;</p>
				<p class="western" style="margin-bottom: 0.21cm">A transaction is
				Completed when the completion message sent from the site&rsquo;s
				terminal is processed and approved by ATIONet, meaning that the
				sale or delivery transaction was successfully performed at the
				site.</p>
				<p class="western" style="margin-bottom: 0.21cm">A transaction is
				Confirmed when the site&rsquo;s terminal receives an acknowledge
				message of the successful processing of completion message from
				ATIONet.</p>
				<p class="western">Thus, Confirmed or Completed transactions are
				considered valid records of a successful transaction at the site.
				But, a transaction that is only Completed (not confirmed) might
				indicate that the site&rsquo;s terminal is not aware of ATIONet
				status. Depending on the site&rsquo;s system, this could lead to
				differences between site&rsquo;s and ATIONet sales totals.</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">HostDateTime</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">19</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">ATIONet&rsquo;s
				transaction datetime &ldquo;yyyy/mm/dd hh:mm:ss&rdquo;. 
				</p>
				<p class="western">ATIONet Host date time is UCT</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubscriberDateTime</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">19</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">Subscriber
				transaction datetime &ldquo;yyyy/mm/dd hh:mm:ss&rdquo;.</p>
				<p class="western">Subscriber date time is Subscriber TimeZone</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubscriberTimeZone</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">TimeZone code of the subscriber (abbreviation)</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SiteDateTime</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">19</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0.21cm">Site
				transaction datetime &ldquo;yyyy/mm/dd hh:mm:ss&rdquo;.</p>
				<p class="western">Site date time is Site TimeZone</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SiteTimeZone</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">TimeZone code of the site
				(abbreviation)</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">DateTime</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">19</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Site&rsquo;s transaction date &ldquo;yyyy/mm/dd
				hh:mm:ss&rdquo;.</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">MerchantCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">30</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">Code of the
				company who owns the site</p>
				<p class="western">N/A to Homebase subscribers</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">MerchantName</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">250</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">Name of the
				company who owns the site</p>
				<p class="western">N/A to Homebase subscriber</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SiteCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Site Code</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SiteName</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">100</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Name of the Site</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">TerminalCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">Site&rsquo;s
				Terminal identification code.</p>
				<p class="western">A Terminal is the device or system that
				captures the transaction at the site, depending on the controller
				(system) type at the site, it may be the actual terminal (for
				example the specific OPT) or the whole system (several OPTs
				served by a single controller).</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubAccountId</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">36</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubAccount&rsquo;s UID</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubAccountExternalCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubAccount&rsquo;s external code</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">AccountTypeDescription</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">&ldquo;Driver&rdquo;
				or &ldquo;Vehicle&rdquo;</p>
				<p class="western" style="margin-bottom: 0.21cm">This field
				indicates whether the sub-account charged with the transaction is
				a Vehicle or a Driver.</p>
				<p class="western">NOTE: The rest of the fields related to
				Vehicle or Driver in the transaction will be populated or not
				depending on this value and should be evaluated accordingly.</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">VehicleCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Vehicle Code</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">DriverCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Driver Code</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">ProductAmountRequested</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">Amount (money)
				requested on a single-product pre-authorization. 
				</p>
				<p class="western" style="margin-bottom: 0.21cm">xxxxxxx.xx</p>
				<p class="western">NOTE: ATIONet Native Transaction Protocol
				allows for one product to be included directly on the message
				body. More products could be included in the Product Data
				structure, therefore &ldquo;Product&rdquo; figures might be
				different (lesser) than &ldquo;Transaction&rdquo; figures, which
				always represents total values. On most situations (just one
				fueling per transaction, without dry products), &ldquo;Product&rdquo;
				and &ldquo;Transaction&rdquo; value-fields would have the same
				values.</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">ProductVolumeRequested</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Volume requested on a single-product
				pre-authorization. xxxxxxx.xx</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">ProductVolumeAuthorized</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Volume authorized. xxxxxxx.xx</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">ProductAmountAuthorized</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Amount authorized. xxxxxxx.xx</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">ProductVolumeDispensed</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Actual fueling volume (adjusted by the
				completion message). xxxxxxx.xx</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">ProductAmountDispensed</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Actual fueling amount (adjusted by the
				completion message). xxxxxxx.xx</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">ProductUnitPrice</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">PUP on a
				single-product transaction.</p>
				<p class="western">xxx.xxx</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">TransactionAmountRequested</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Transaction amount requested on the
				pre-authorization. xxxxxxx.xx</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">TransactionAmountAuthorized</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Transaction amount authorized.	 <br>xxxxxxx.xx</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">TransactionAmountDispensed</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Actual amount fueled. xxxxxxx.xx</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">MeasurementUnitCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Unit of measuring for the volume fields,
				according to site&rsquo;s configuration.</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">CurrencyCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Currency of the amount fields, according to
				site&rsquo;s configuration</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">FuelCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Site&rsquo;s product code</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">FuelMasterCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Standardized product code. Helps to identify a
				fuel product category across multiple Merchant brands and site&rsquo;s
				product codes</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">FuelMasterDescription</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">100</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Standardized product description. Helps to
				identify a fuel product category across multiple Merchant brands
				and site&rsquo;s product codes</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">InvoiceNumber</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Number assigned by the Terminal to the
				document issued for the transaction. May be empty.</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">BatchNumber</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">11</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Batch Identification. Informed by the site&rsquo;s
				controller. Persisted on ATIONet for information purposes only.
				May be empty</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">ShiftNumber</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Shift (or Date+Shift) Identification. Informed
				by the site&rsquo;s controller. Persisted on ATIONet for
				information purposes only. May be empty</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">PumpNumer</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">2</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Fueling position number. Informed by the
				terminal.</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">EntryMethod</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">1</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0cm">1 =
				Manual Entry</p>
				<p class="western" align="left" style="margin-bottom: 0cm">2 =
				Magnetic Card Swipe</p>
				<p class="western" align="left" style="margin-bottom: 0cm">3 =
				Smart Card</p>
				<p class="western">4 = AVI</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">CompanyCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">30</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">Company code</p>
				<p class="western">Not meaningful for Homebase subscribers</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">CompanyName</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">250</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">Company name</p>
				<p class="western">Not meaningful for Homebase subscribers</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">ClassificationLabel1</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">200</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">Classifications</p>
				<p class="western">ATIONet allows for up to four user-defined
				classification field for Vehicles or Drivers.</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">ClassificationLabel2</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">200</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western"><br>
				</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">ClassificationLabel3</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">200</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western"><br>
				</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">ClassificationLabel4</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">200</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western"><br>
				</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">ContractCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">20</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">Contract code</p>
				<p class="western">Not meaningful for Homebase subscribers</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubContractCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">SubContract code</p>
				<p class="western">Not meaningful for Homebase subscribers</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">PrimaryIdentificationLabel</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Public ID of the primary
				identification device (chipkey ID, account number on a mag card,
				RFID serial number, etc.)</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SecondaryIdentificationLabel</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Public ID of the secondary identification
				device (chipkey ID, account number on a mag card, RFID serial
				number, etc.)</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">FleetCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Fleet Code</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">FleetName</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Fleet Name</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">VehiclePlate</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Licence plate</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">VehicleClassDescription</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Vehicle Class</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">VehicleClassificationValue1</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western"><br>
				</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">VehicleClassificationValue2</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western"><br>
				</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">VehicleClassificationValue3</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western"><br>
				</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">VehicleClassificationValue4</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western"><br>
				</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">DriverName</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">100</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Name of Driver</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">DriverLicenceState</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Driver licence jurisdiction</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">DriverLicenceNumber</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Driver licence</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">DriverID</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">DriverID prompt result</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">DriverClassificationValue1</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western"><br>
				</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">DriverClassificationValue2</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western"><br>
				</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">DriverClassificationValue3</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western"><br>
				</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">DriverClassificationValue4</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western"><br>
				</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">EngineHours</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Engine hours prompt result</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Odometer</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Odometer prompt result</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">LastOdometer</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Previous odometer value</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">LastEngineHours</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Previous engine hours value</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">TrailerHourMeterReading</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Trailer hours prompt result</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">TruckUnitNumber</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Truck Unit ID prompt result</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">TrailerNumber</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Trailer ID prompt result</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">TripNumber</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Trip/Guide/Route prompt result</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">PurchaseOrderNumber</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">PO prompt result</p>
			</td>
		</tr>
	</tbody>
</table>

####8 Account Enquiries####

The Account Enquiries messages retrieve data from ATIONet, specific to a
Contract or Sub-Account (Vehicle or Driver types).

Depending on the type of enquiry, this message might be used by one or
the other party of the contract (the subscriber or the fleet company).

#####8.1 Action Codes#####

The Action Code specifies the type of enquiry requested. The submitted
code must match one of the pre-defined operation types. Not all
operation types are available for all subscribers and/or fleet
companies; availability depends on subscription types but also on
contract terms with ATIONet.

<table>
	<tr valign="top">
		<th align="left">Action Code
		</th>
		<th colspan="2" align="left">Description
		</th>
	</tr>
	<tr valign="top">
		<td rowspan="2" width="41" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">941</p>
		</td>
		<td width="145" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Title:</p>
		</td>
		<td width="338" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Sub-account Balance Enquiry	</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="145" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Function:</p>
		</td>
		<td width="338" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western" style="margin-bottom: 0.21cm">Retrieves the
			total Balance for a given Sub-Account (Vehicle or Driver). Works
			with product or money based current accounts. On a product
			account, it returns the volume balance and the master product
			code. May return up to two product-volume pair when the vehicle is
			a dual-product unit.</p>
			<p class="western">This message only retrieves information from
			ATIONet&rsquo;s Current Account subsystem, without considering any
			other business rule that may apply to the Site, Vehicle and/or
			Driver, which may potentially impact on the amount or limit that
			would be authorized at transaction time.</p>
		</td>
	</tr>
</table>

#####8.2 Identification#####

When an Account Enquiry is received, ATIONet will try to identify the
Company and the Identifier of the sub-account (Vehicle or Driver), this
can be performed thru several combinations of the Identification Fields
on the body of the message:

1.  Any Identifier field (Identifier, Driver Code, Vehicle Code, Vehicle
    Plate, SubAccount External Code and SubAccount Id) only. Only
    accepted for Home-base subscriptions.

2.  Company Code + Identifier.

3.  Company Code + Contract Code + (Driver Code or Vehicle Code or
    Vehicle Plate)

#####8.3 Account Enquiry (POST) – Body Section Record Format *Request*#####

<table>
	<thead>
		<tr valign="top">
			<th align="left">Field Name
			</th>
			<th align="left">Size
			</th>
			<th align="left">Type
			</th>
			<th align="left">Condition
			</th>
			<th align="left">Descriptions/Field Value(s)
			</th>
		</tr>
	</thead>
	<tbody>
		<tr valign="top">
			<td width="151" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">SubscriberCode</p>
			</td>
			<td width="24" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">3</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Required</p>
			</td>
			<td width="209" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Fixed. To be assigned by
				ATIONet</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="151" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">ActionCode</p>
			</td>
			<td width="24" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">3</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Required</p>
			</td>
			<td width="209" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Operation type code. <br>See
				Action Code Section.</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="151" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">CompanyCode</p>
			</td>
			<td width="24" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">30</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="209" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="151" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">ContractCode</p>
			</td>
			<td width="24" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">20</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="209" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="151" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">DriverCode</p>
			</td>
			<td width="24" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="209" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="151" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">VehicleCode</p>
			</td>
			<td width="24" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="209" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="151" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">VehiclePlate</p>
			</td>
			<td width="24" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="209" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="151" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">SubAccountExternalCode</p>
			</td>
			<td width="24" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="209" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="151" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">SubAccountId</p>
			</td>
			<td width="24" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">36</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="209" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="151" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Identifier</p>
			</td>
			<td width="24" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="29" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="70" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="209" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0cm">Public
				ID of the identification device (chipkey ID, account number on
				a mag card, RFID serial number, etc.)</p>
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
	</tbody>
</table>

#####8.4 Account Enquiry (POST) – Body Section Record Format *Response*#####

<table>
	<thead>
		<tr valign="top">
			<th align="left">Field Name
			</th>
			<th align="left">Size
			</th>
			<th align="left">Type
			</th>
			<th align="left">Descriptions/Field Value(s)
			</th>
		</tr>
	</thead>
	<tbody>
		<tr valign="top">
			<td width="180" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">SubscriberCode</p>
			</td>
			<td width="38" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">3</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="248" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Fixed. To be assigned by ATIONet</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="180" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">CompanyCode</p>
			</td>
			<td width="38" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">30</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="248" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Company identification. Should be
				ignored on Homebase subscribers.</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="180" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">CompanyName</p>
			</td>
			<td width="38" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">250</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="248" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Company name. Should be ignored
				on Homebase subscribers.</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="180" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">ContractCode</p>
			</td>
			<td width="38" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">20</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="248" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Contract identification. Should
				be ignored on Homebase subscribers.</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="180" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubContractCode</p>
			</td>
			<td width="38" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="248" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">SubContract code</p>
				<p class="western">Not meaningful for Homebase subscribers</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="180" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubAccountId</p>
			</td>
			<td width="38" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">36</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="248" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubAccount&rsquo;s UID</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="180" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubAccountExternalCode</p>
			</td>
			<td width="38" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="248" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubAccount&rsquo;s external code</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="180" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">DriverCode</p>
			</td>
			<td width="38" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="248" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="180" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">VehicleCode</p>
			</td>
			<td width="38" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="248" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="180" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">VehiclePlate</p>
			</td>
			<td width="38" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="248" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Identification section</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="180" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Identifier</p>
			</td>
			<td width="38" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">250</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="248" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Identifications related to
				subaccount</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="180" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">FuelMasterCode</p>
			</td>
			<td width="38" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="248" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Standardized product code. Helps to identify a
				fuel product category across multiple Merchant brands and site&rsquo;s
				product codes</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="180" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">FuelMasterDescription</p>
			</td>
			<td width="38" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">100</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="248" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Standardized product description. Helps to
				identify a fuel product category across multiple Merchant brands
				and site&rsquo;s product codes</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="180" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">CurrencyCode</p>
			</td>
			<td width="38" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A</p>
			</td>
			<td width="248" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Currency configured for the
				Contract</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="180" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Amount</p>
			</td>
			<td width="38" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">N</p>
			</td>
			<td width="248" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0cm">Amount
				balance for the sub-account. 
				</p>
				<p class="western" align="left">xxxxxxx.xx</p>
			</td>
		</tr>
	</tbody>
</table>

####9 Account Downloads####

The Account Download messages are POST actions to recover all the
currents accounts movements processed by ATIONet for a given Company
Code depending on the particular Action Code.

The Action Code is validated against the type of company of the
authenticated user. Request not passing this validation will be
rejected.

The download will be limited by dates (from and to), which must be
included in the request

#####9.1 Action Codes#####

The Action Code specifies the type of record transaction to be
retrieved; this differentiation is based on the different roles on an
ATIONet operation (Fleet Company, Merchant, Network, Home-base), which
also mandates different ways to identify the requester and scope of
transactions to download.

<table>
	<tr valign="top">
		<th align="left">Action Code
		</th>
		<th colspan="2" align="left">Description
		</th>
	</tr>
	<tr valign="top">
		<td rowspan="4" width="54" height="19" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">951</p>
		</td>
		<td width="84" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Title:</p>
		</td>
		<td width="374" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Movements Download 
			</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="84" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Function:</p>
		</td>
		<td width="374" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Download complete current account movements
			records</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="84" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Allowed for:</p>
		</td>
		<td width="374" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Subscribers and Fleet Companies</p>
		</td>
	</tr>
	<tr valign="top">
		<td width="84" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western">Identification:</p>
		</td>
		<td width="374" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
			<p class="western" style="margin-bottom: 0.21cm">Subscriber Code</p>
			<p class="western">Company Code (Optional, if included will act as
			a filter)</p>
		</td>
	</tr>
</table>

#####9.2 Account Download (POST) – Body Section Format *Request*#####

<table>
	<thead>
		<tr valign="top">
			<th align="left">Field Name
			</th>
			<th align="left">Size
			</th>
			<th align="left">Type
			</th>
			<th align="left">Condition
			</th>
			<th align="left">Descriptions/Field Value(s)
			</th>
		</tr>
	</thead>
	<tbody>
		<tr valign="top">
			<td width="100" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">SubscriberCode</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">3</p>
			</td>
			<td width="37" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="76" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Required</p>
			</td>
			<td width="239" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Fixed. To be assigned by ATIONet</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="100" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">ActionCode</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">3</p>
			</td>
			<td width="37" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">N</p>
			</td>
			<td width="76" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Required</p>
			</td>
			<td width="239" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Action Codes section above</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="100" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">CompanyCode</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">30</p>
			</td>
			<td width="37" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="76" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Conditional</p>
			</td>
			<td width="239" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">See Action Codes section above</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="100" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">DateFrom</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">19</p>
			</td>
			<td width="37" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="76" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Required</p>
			</td>
			<td width="239" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0cm">From
				date to filter movements</p>
				<p class="western" align="left">&ldquo;yyyy/MM/dd hh:mm:ss&rdquo;</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="100" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">DateTo</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">19</p>
			</td>
			<td width="37" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">A/N</p>
			</td>
			<td width="76" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Optional</p>
			</td>
			<td width="239" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0cm">To
				date to filter movements</p>
				<p class="western" align="left">&ldquo;yyyy/MM/dd hh:mm:ss&rdquo;</p>
			</td>
		</tr>
	</tbody>
</table>

#####9.3 Account Download (POST) – Body Section Format *Response*#####

<table>
	<thead>
		<tr valign="top">
			<th align="left">Field Name
			</th>
			<th align="left">Size
			</th>
			<th align="left">Type
			</th>
			<th align="left">Descriptions/Field Value(s)
			</th>
		</tr>
	</thead>
	<tbody>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Id</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">36</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Current account&rsquo;s UID</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">MovementId</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">36</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Movements&rsquo;s UID</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubscriberCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">3</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Code of the subscriber who owns the
				transaction</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">HostDateTime</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">19</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">ATIONet&rsquo;s
				transaction date time &ldquo;yyyy/mm/dd hh:mm:ss&rdquo;. 
				</p>
				<p class="western">ATIONet Host date time is UCT</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">DateTime</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">19</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">movement date
				expressed in subscriber time zone 
				</p>
				<p class="western">&ldquo;yyyy/mm/dd hh:mm:ss&rdquo;.</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubscriberTimeZone</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">TimeZone code of the subscriber (abbreviation)</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Type</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">1</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Internal ATIOnet movement type
				code</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">TypeDescription</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Movement type description</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Origin</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">1</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Internal ATIOnet code for the origin of the
				movement</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">OriginDescription</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Description for the origin of the movement</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Description</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">1000</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Movement description</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubAccountId</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">36</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubAccount&rsquo;s UID</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubAccountExternalCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubAccount&rsquo;s external code</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">CompanyCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">30</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">Company code</p>
				<p class="western">Not meaningful for Homebase subscribers</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">CompanyName</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">250</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">Company name</p>
				<p class="western">Not meaningful for Homebase subscribers</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">ContractCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">20</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">Contract code</p>
				<p class="western">Not meaningful for Homebase subscribers</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">SubContractCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">SubContract code</p>
				<p class="western">Not meaningful for Homebase subscribers</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">IsDebit</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">1</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" style="margin-bottom: 0.21cm">Indicates that&rsquo;s
				a debit or credit movement</p>
				<p class="western">1 = &ldquo;True&rdquo;, 2= &ldquo;False&rdquo;</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">FuelMasterCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Standardized product code. Helps to identify a
				fuel product category across multiple Merchant brands and site&rsquo;s
				product codes</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">FuelMasterDescription</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">100</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Standardized product description. Helps to
				identify a fuel product category across multiple Merchant brands
				and site&rsquo;s product codes</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">CurrencyCode</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">50</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">A/N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western">Currency of the amount fields</p>
			</td>
		</tr>
		<tr valign="top">
			<td width="191" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">Amount</p>
			</td>
			<td width="43" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">10</p>
			</td>
			<td width="31" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left">N</p>
			</td>
			<td width="232" style="border: 1px solid #00000a; padding-top: 0cm; padding-bottom: 0cm; padding-left: 0.2cm; padding-right: 0.19cm">
				<p class="western" align="left" style="margin-bottom: 0cm">Amount
				balance for the sub-account. 
				</p>
				<p class="western" align="left">xxxxxxx.xx</p>
			</td>
		</tr>
	</tbody>
</table>
