![ATIONET](C:\Users\fhart\Desktop\Logo.png)

##ATIONet Native Interface API Protocol Specification##


<table>
	<tr>
		<td colspan="2">
			<b>Document Information<b>
		</td>
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
		<td colspan="3">
			<b>Change Log<b>
		</td>
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

\
\

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

**Homebase.** A type of ATIONet subscription where the subscriber owns
the site(s) but also the fleet(s) of vehicles.

**Network.** A type of ATIONet subscription where the subscriber enrolls
Fleet Companies and retail or commercial sites to operate with its own
method-of-payment. The Network company doesn’t own the site(s) or the
vehicles.

**Retail.** A type of ATIONet subscription where the subscriber owns the
sites and enrolls Fleet Companies to operate with its own
method-of-payment.

**Merchant.** On a Network type subscription, the Merchant is the
company who own the sites.

**Company.** On a Network or Retail type subscription, the Company is
the company who own the fleet.

**Terminal.** Transaction capture device at the site.

\

\
\

\
\

\

####1.  Scope####
    =====

Version 1.3 of this document covers a particular version of ATIONet’s
Host protocol. Although feature’s descriptions are generally not related
to a particular version of the protocol, some changes may apply which
would be specifically commented and identified on each feature’s
description paragraph.

#####1.1  Scope details:#####
    --------------

Protocol: ATIONet Native Interface API

Version: Version 1.3

API URI: native.ationet.com/v1/interface\
\
\

####2.  System Interface API####
    ====================

The Interface API provide system-to-system access to certain features of
ATIONet otherwise only available via the ATIONet Console, and it’s
intended to allow direct interaction of third-party systems on
Subscribers, Merchants and fleet Companies with ATIONet.

Availability of part or all the functionality of the Interface API is
subject to the business type and contract terms of the ATIONet
subscriber.

#####2.1  Interface API Messages#####
    ----------------------

**Name**

**Protocol Ver.\
Initial Change**

**Description**

Statement charges [HTTP POST]

901 to 920

1.0

\
\

\
\

\

Commands ATIONet to process a movement on the account of a driver or
vehicle, given an action type indicated on the message body.

Availability of this message and the type of actions allowed depend on
the subscriber type and its contracting terms.

901 - Balance transfer to a sub-account

1.1

\

902 - Balance withdrawal from a sub-account

\

1.3

901 - Balance transfer to a sub-account

902 - Balance withdrawal from a sub-account

903 - Transfer balance from sub-account to a sub-account

904 - Transfer balance from contract to a sub-account

905 - Transfer balance from sub-account to a contract

Transactions Download\
[HTTP POST]

931 to 940

1.0

\

Returns a list of completed transactions from ATIONet host, between two
dates, for a given Subscriber, Merchant or fleet Company

931 - Transactions Download

932 - Transactions Download for Merchants

1.1

931 - Transactions Download

932 - Transactions Download for Merchants

\

1.3

931 - Transactions Download

932 - Transactions Download for Merchants

Account Enquiries\
[HTTP POST]

941 to 950

1.1

\

Returns specific values of a Contract or Sub-account.

941 - Sub-account Balance Enquiry

942 - Sub-Account Limit Enquiry

1.2

\

943 - Contract Balance Enquiry

\

1.3

941 - Sub-account Balance Enquiry

942 - Sub-Account Limit Enquiry

~~943 - Contract Balance Enquiry~~

Account Downloads\
[HTTP POST]

951 to 960

1.2

\

951 - Sub-Account Movements Download

952 - Contract Movements Download\
\

\

1.3

951 - Movements Download

~~951 - Sub-Account Movements Download~~

~~952 - Contract Movements Download~~

####3.  Data security####
    =============

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

4.  Message Structure {.western}
    =================

All Interface API messages share the same structure, what change from
message to message are the Action Code, which indicates the actual
interface function, the value fields sent and received, and the HTTP
action (POST, GET, REQUEST) which changes depending on the Action Code.

Both, requests and responses use a JSON format.

Only one request is accepted on each message, although some requests and
many responses will contain multiple records.

#### Request Format {.western}

###### Header: {.western}

Accept-Encoding: gzip

Authorization: Basic user:password

###### Body: {.western}

{“ActionCode”:”nnn”,”FieldName”:”StringValue”,”FieldName”:Value}

\

#### Response {.western}

###### Header: {.western}

Content-Type: application/json; charset=utf-8

###### Body: {.western}

[{“Fieldname”:”StringValue”,”FieldName”:”StringValue”,”FieldName”:Value},\
{“Fieldname”:”StringValue”,”FieldName”:”StringValue”,”FieldName”:Value}]

\

Note: Some Action Codes returns a single response row, for example the
Statement charges.

Note: Alphanumeric fields, stated as Type “A/N” in record format tables
below show the maximum possible length as the Size, although in
JSON-formatted strings they will be represented with trailing spaces
trimmed.

5.  Error handling {.western}
    ==============

Success/failure exits on the Interface API will be handled via HTTP
status codes.

\

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

\

Failure to process the request will be indicated by an HTTP 400’s range
status code. The body will contain a single JSON-formatted item with the
“ResponseCode”, “ResponseMessage” and “ResponseError” fields.

6.  Statement Charges Interface {.western}
    ===========================

The Statement Charge message sends an instruction to ATIONet to apply a
well-defined action on the current account subsystem, the subject of the
action will be a sub-account of a contract, lets say a Vehicle or a
Driver account.

Depending on the type of charge, this message might be used by one or
the other party of the contract (the subscriber or the fleet company).

3.  Action Codes {.western}
    ------------

The Action Code specifies the type of accounting transactions requested
by a Statement Charge Message. The submitted code must match one of the
pre-defined operation types. Not all operation types are available for
all subscribers and/or fleet companies, availability depends on
subscription types but also on contract terms with ATIONet.

Action Code

Description

901

Title:

Balance transfer to a sub-account

Function:

Transfers a given value from the global balance of the Contract to the
sub-account related to the Vehicle or Driver.

Contract Balance must have enough funds (or product volume) to allow the
transfer; otherwise the action will be rejected by the current accounts
subsystem.

Observations

The action will first trigger a Deposit action on the Contract and the
Contract to sub-account transfer.

902

Title:

Balance withdrawal from a sub-account

Function:

Withdraws a given value from the sub-account related to the Vehicle or
Driver.

Sub-account Balance must have enough funds (or product volume) to allow
the withdrawal; otherwise the action will be rejected by the current
accounts subsystem.

903

Title:

Balance transfer from sub-account to sub-account

Function:

Transfers a given value from the original sub-account (related to the
Original Vehicle or Driver) to the sub-account related to the Vehicle or
Driver.

Original sub-account balance must have enough funds (or product volume)
to allow the transfer; otherwise the action will be rejected by the
current accounts subsystem.

904

Title:

Balance transfer from contract to sub-account

Function:

Transfers a given value from the contract to the sub-account related to
the Vehicle or Driver.

Contract balance must have enough funds (or product volume) to allow the
transfer; otherwise the action will be rejected by the current accounts
subsystem.

905

Title:

Balance transfer from sub-account to contract

Function:

Transfers a given value from the sub-account related to the Vehicle or
Driver to the contract.

Sub-account Balance must have enough funds (or product volume) to allow
the withdrawal; otherwise the action will be rejected by the current
accounts subsystem.

\
\

4.  Identification {.western}
    --------------

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

1.  Statement Charge (POST) – Body Section Record Format {.western}
    ----------------------------------------------------

Field Name

Size

Type

Condition

Descriptions/Field Value(s)

SubscriberCode

3

A/N

Required

Fixed. To be assigned by ATIONet

ActionCode

3

N

Required

Operation type code.\
See Action Code Section.

CompanyCode

30

A/N

Optional

See Identification section

ContractCode

20

A/N

Optional

See Identification section

DriverCode

50

A/N

Optional

See Identification section

VehicleCode

50

A/N

Optional

See Identification section

VehiclePlate

50

A/N

Optional

See Identification section

SubAccountExternalCode

50

A/N

Optional

See Identification section

SubAccountId

36

A/N

Optional

See Identification section

Identifier

50

A/N

Optional

Public ID of the identification device (chipkey ID, account number on a
mag card, RFID serial number, etc.)

See Identification section

DriverCodeOrigin

50

A/N

Optional

See Identification section

VehicleCodeOrigin

50

A/N

Optional

See Identification section

VehiclePlateOrigin

50

A/N

Optional

See Identification section

SubAccountExternalCodeOrigin

50

A/N

Optional

See Identification section

SubAccountIdOrigin

36

A/N

Optional

See Identification section

IdentifierOrigin

50

A/N

Optional

Public ID of the identification device (chipkey ID, account number on a
mag card, RFID serial number, etc.)

See Identification section

MasterFuelCode

50

A/N

Conditional

Required if Charge Volume is specified

CurrencyCode

50

A

Conditional

Required if Charge Amount is specified

Amount

10

N

Required

Charge Amount or Charge Volume

Description

1000

A/N

Optional

A description for the current account movement

7.  Transactions Download Interface {.western}
    ===============================

The Transactions Download Interface are POST actions to recover all the
payment transactions processed by ATIONet for a given Terminal, Contract
Code or Company Code depending on the particular Action Code.

The Action Code is validated against the type of company of the
authenticated user. Request not passing this validation will be
rejected.

The download will be limited by dates (from and to), which must be
included in the request

6.  Action Codes {.western}
    ------------

The Action Code specifies the type of record transaction to be
retrieved; this differentiation is based on the different roles on an
ATIONet operation (Fleet Company, Merchant, Network, Home-base), which
also mandates different ways to identify the requester and scope of
transactions to download.

Action Code

Description

931

Title:

Transactions Download

Function:

Download complete transactions records

Allowed for:

Subscribers and Fleet Companies

Identification:

Subscriber Code

Merchant Code (Optional, if included will act as a filter)

Company Code (Optional, if included will act as a filter)

Terminal Code(Optional, if included will act as a filter)

Contract Code (Optional, if included will act as a filter)

932

Title:

Transactions Download for Merchants

Function:

Download transactions records (fueling details subset)

Allowed for:

Merchants on a three-layer subscription model

Identification:

Subscriber Code

Merchant Code

Terminal Code (Optional, if included will act as a filter)

\
\

7.  Transactions Download (POST) – Body Section Format *Request* {.western}
    ------------------------------------------------------------

Field Name

Size

Type

Condition

Descriptions/Field Value(s)

SubscriberCode

3

A/N

Required

Fixed. To be assigned by ATIONet

ActionCode

3

N

Required

See Action Codes section above

MerchantCode

30

A/N

Conditional

See Action Codes section above

CompanyCode

30

A/N

Conditional

See Action Codes section above

ContractCode

20

A/N

Optional

See Action Codes section above

TerminalCode

50

A/N

Optional

See Action Codes section above

DateFrom

19

A/N

Required

From date to filter transactions

“yyyy/MM/dd hh:mm:ss”

DateTo

19

A/N

Optional

To date to filter transactions

“yyyy/MM/dd hh:mm:ss”

\

1.  Transactions Download (POST) – Body Section Format *Response* {.western}
    -------------------------------------------------------------

Field Name

Size

Type

Descriptions/Field Value(s)

TransactionID

36

A/N

Transaction’s UID

SubscriberCode

3

A/N

Code of the subscriber who owns the transaction

TransactionSequenceNumber

50

A/N

Transaction ID as received from the site’s controller system. Usually a
transaction counter. Site-based, might repeat from site to site.

AuthorizationCode

50

A/N

Authorization Code

ResponseCode

5

A/N

Host response code sent to the terminal

ResponseMessage

50

A/N

Host response text sent to the terminal

Status

1

N

2- “Completed”, 3- “Confirmed”

StatusDescription

50

A/N

“Completed” or “Confirmed”

A transaction is Completed when the completion message sent from the
site’s terminal is processed and approved by ATIONet, meaning that the
sale or delivery transaction was successfully performed at the site.

A transaction is Confirmed when the site’s terminal receives an
acknowledge message of the successful processing of completion message
from ATIONet.

Thus, Confirmed or Completed transactions are considered valid records
of a successful transaction at the site. But, a transaction that is only
Completed (not confirmed) might indicate that the site’s terminal is not
aware of ATIONet status. Depending on the site’s system, this could lead
to differences between site’s and ATIONet sales totals.

HostDateTime

19

A/N

ATIONet’s transaction datetime “yyyy/mm/dd hh:mm:ss”.

ATIONet Host date time is UCT

SubscriberDateTime

19

A/N

Subscriber transaction datetime “yyyy/mm/dd hh:mm:ss”.

Subscriber date time is Subscriber TimeZone

SubscriberTimeZone

50

A/N

TimeZone code of the subscriber (abbreviation)

SiteDateTime

19

A/N

Site transaction datetime “yyyy/mm/dd hh:mm:ss”.

Site date time is Site TimeZone

SiteTimeZone

50

A/N

TimeZone code of the site (abbreviation)

DateTime

19

A/N

Site’s transaction date “yyyy/mm/dd hh:mm:ss”.

MerchantCode

30

A/N

Code of the company who owns the site

N/A to Homebase subscribers

MerchantName

250

A/N

Name of the company who owns the site

N/A to Homebase subscriber

SiteCode

50

A/N

Site Code

SiteName

100

A/N

Name of the Site

TerminalCode

50

A/N

Site’s Terminal identification code.

A Terminal is the device or system that captures the transaction at the
site, depending on the controller (system) type at the site, it may be
the actual terminal (for example the specific OPT) or the whole system
(several OPTs served by a single controller).

SubAccountId

36

A/N

SubAccount’s UID

SubAccountExternalCode

50

A/N

SubAccount’s external code

AccountTypeDescription

10

A/N

“Driver” or “Vehicle”

This field indicates whether the sub-account charged with the
transaction is a Vehicle or a Driver.

NOTE: The rest of the fields related to Vehicle or Driver in the
transaction will be populated or not depending on this value and should
be evaluated accordingly.

VehicleCode

50

A/N

Vehicle Code

DriverCode

50

A/N

Driver Code

ProductAmountRequested

10

N

Amount (money) requested on a single-product pre-authorization.

xxxxxxx.xx

NOTE: ATIONet Native Transaction Protocol allows for one product to be
included directly on the message body. More products could be included
in the Product Data structure, therefore “Product” figures might be
different (lesser) than “Transaction” figures, which always represents
total values. On most situations (just one fueling per transaction,
without dry products), “Product” and “Transaction” value-fields would
have the same values.

ProductVolumeRequested

10

N

Volume requested on a single-product pre-authorization. xxxxxxx.xx

ProductVolumeAuthorized

10

N

Volume authorized. xxxxxxx.xx

ProductAmountAuthorized

10

N

Amount authorized. xxxxxxx.xx

ProductVolumeDispensed

10

N

Actual fueling volume (adjusted by the completion message). xxxxxxx.xx

ProductAmountDispensed

10

N

Actual fueling amount (adjusted by the completion message). xxxxxxx.xx

ProductUnitPrice

10

N

PUP on a single-product transaction.

xxx.xxx

TransactionAmountRequested

10

N

Transaction amount requested on the pre-authorization. xxxxxxx.xx

TransactionAmountAuthorized

10

N

Transaction amount authorized.\
xxxxxxx.xx

TransactionAmountDispensed

10

N

Actual amount fueled. xxxxxxx.xx

MeasurementUnitCode

50

A/N

Unit of measuring for the volume fields, according to site’s
configuration.

CurrencyCode

50

A/N

Currency of the amount fields, according to site’s configuration

FuelCode

50

N

Site’s product code

FuelMasterCode

50

A/N

Standardized product code. Helps to identify a fuel product category
across multiple Merchant brands and site’s product codes

FuelMasterDescription

100

A/N

Standardized product description. Helps to identify a fuel product
category across multiple Merchant brands and site’s product codes

InvoiceNumber

50

A/N

Number assigned by the Terminal to the document issued for the
transaction. May be empty.

BatchNumber

11

N

Batch Identification. Informed by the site’s controller. Persisted on
ATIONet for information purposes only. May be empty

ShiftNumber

50

A/N

Shift (or Date+Shift) Identification. Informed by the site’s controller.
Persisted on ATIONet for information purposes only. May be empty

PumpNumer

2

N

Fueling position number. Informed by the terminal.

EntryMethod

1

N

1 = Manual Entry

2 = Magnetic Card Swipe

3 = Smart Card

4 = AVI

CompanyCode

30

A/N

Company code

Not meaningful for Homebase subscribers

CompanyName

250

A/N

Company name

Not meaningful for Homebase subscribers

ClassificationLabel1

200

A/N

Classifications

ATIONet allows for up to four user-defined classification field for
Vehicles or Drivers.

ClassificationLabel2

200

A/N

\

ClassificationLabel3

200

A/N

\

ClassificationLabel4

200

A/N

\

ContractCode

20

A/N

Contract code

Not meaningful for Homebase subscribers

SubContractCode

50

A/N

SubContract code

Not meaningful for Homebase subscribers

PrimaryIdentificationLabel

50

A/N

Public ID of the primary identification device (chipkey ID, account
number on a mag card, RFID serial number, etc.)

SecondaryIdentificationLabel

50

A/N

Public ID of the secondary identification device (chipkey ID, account
number on a mag card, RFID serial number, etc.)

FleetCode

50

A/N

Fleet Code

FleetName

50

A/N

Fleet Name

VehiclePlate

50

A/N

Licence plate

VehicleClassDescription

50

A/N

Vehicle Class

VehicleClassificationValue1

50

A/N

\

VehicleClassificationValue2

50

A/N

\

VehicleClassificationValue3

50

A/N

\

VehicleClassificationValue4

50

A/N

\

DriverName

100

A/N

Name of Driver

DriverLicenceState

50

A/N

Driver licence jurisdiction

DriverLicenceNumber

50

A/N

Driver licence

DriverID

50

N

DriverID prompt result

DriverClassificationValue1

50

A/N

\

DriverClassificationValue2

50

A/N

\

DriverClassificationValue3

50

A/N

\

DriverClassificationValue4

50

A/N

\

EngineHours

10

N

Engine hours prompt result

Odometer

10

N

Odometer prompt result

LastOdometer

10

N

Previous odometer value

LastEngineHours

10

N

Previous engine hours value

TrailerHourMeterReading

10

N

Trailer hours prompt result

TruckUnitNumber

50

A/N

Truck Unit ID prompt result

TrailerNumber

50

A/N

Trailer ID prompt result

TripNumber

50

A/N

Trip/Guide/Route prompt result

PurchaseOrderNumber

50

A/N

PO prompt result

8.  Account Enquiries {.western}
    =================

The Account Enquiries messages retrieve data from ATIONet, specific to a
Contract or Sub-Account (Vehicle or Driver types).

Depending on the type of enquiry, this message might be used by one or
the other party of the contract (the subscriber or the fleet company).

9.  Action Codes {.western}
    ------------

The Action Code specifies the type of enquiry requested. The submitted
code must match one of the pre-defined operation types. Not all
operation types are available for all subscribers and/or fleet
companies; availability depends on subscription types but also on
contract terms with ATIONet.

Action Code

Description

941

Title:

Sub-account Balance Enquiry

Function:

Retrieves the total Balance for a given Sub-Account (Vehicle or Driver).
Works with product or money based current accounts. On a product
account, it returns the volume balance and the master product code. May
return up to two product-volume pair when the vehicle is a dual-product
unit.

This message only retrieves information from ATIONet’s Current Account
subsystem, without considering any other business rule that may apply to
the Site, Vehicle and/or Driver, which may potentially impact on the
amount or limit that would be authorized at transaction time.

\
\

10. Identification {.western}
    --------------

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

1.  Account Enquiry (POST) – Body Section Record Format *Request* {.western}
    -------------------------------------------------------------

    Field Name

    Size

    Type

    Condition

    Descriptions/Field Value(s)

    SubscriberCode

    3

    A/N

    Required

    Fixed. To be assigned by ATIONet

    ActionCode

    3

    N

    Required

    Operation type code.\
    See Action Code Section.

    CompanyCode

    30

    A/N

    Optional

    See Identification section

    ContractCode

    20

    A/N

    Optional

    See Identification section

    DriverCode

    50

    A/N

    Optional

    See Identification section

    VehicleCode

    50

    A/N

    Optional

    See Identification section

    VehiclePlate

    50

    A/N

    Optional

    See Identification section

    SubAccountExternalCode

    50

    A/N

    Optional

    See Identification section

    SubAccountId

    36

    A/N

    Optional

    See Identification section

    Identifier

    50

    A/N

    Optional

    Public ID of the identification device (chipkey ID, account number
    on a mag card, RFID serial number, etc.)

    See Identification section

2.  Account Enquiry (POST) – Body Section Record Format *Response* {.western}
    --------------------------------------------------------------

Field Name

Size

Type

Descriptions/Field Value(s)

SubscriberCode

3

A/N

Fixed. To be assigned by ATIONet

CompanyCode

30

A/N

Company identification. Should be ignored on Homebase subscribers.

CompanyName

250

A/N

Company name. Should be ignored on Homebase subscribers.

ContractCode

20

A/N

Contract identification. Should be ignored on Homebase subscribers.

SubContractCode

50

A/N

SubContract code

Not meaningful for Homebase subscribers

SubAccountId

36

A/N

SubAccount’s UID

SubAccountExternalCode

50

A/N

SubAccount’s external code

DriverCode

50

A/N

See Identification section

VehicleCode

50

A/N

See Identification section

VehiclePlate

50

A/N

See Identification section

Identifier

250

A/N

Identifications related to subaccount

FuelMasterCode

50

A/N

Standardized product code. Helps to identify a fuel product category
across multiple Merchant brands and site’s product codes

FuelMasterDescription

100

A/N

Standardized product description. Helps to identify a fuel product
category across multiple Merchant brands and site’s product codes

CurrencyCode

50

A

Currency configured for the Contract

Amount

10

N

Amount balance for the sub-account.

xxxxxxx.xx

9.  Account Downloads {.western}
    =================

The Account Download messages are POST actions to recover all the
currents accounts movements processed by ATIONet for a given Company
Code depending on the particular Action Code.

The Action Code is validated against the type of company of the
authenticated user. Request not passing this validation will be
rejected.

The download will be limited by dates (from and to), which must be
included in the request

13. Action Codes {.western}
    ------------

The Action Code specifies the type of record transaction to be
retrieved; this differentiation is based on the different roles on an
ATIONet operation (Fleet Company, Merchant, Network, Home-base), which
also mandates different ways to identify the requester and scope of
transactions to download.

Action Code

Description

951

Title:

Movements Download

Function:

Download complete current account movements records

Allowed for:

Subscribers and Fleet Companies

Identification:

Subscriber Code

Company Code (Optional, if included will act as a filter)

\
\

14. Account Download (POST) – Body Section Format *Request* {.western}
    -------------------------------------------------------

Field Name

Size

Type

Condition

Descriptions/Field Value(s)

SubscriberCode

3

A/N

Required

Fixed. To be assigned by ATIONet

ActionCode

3

N

Required

See Action Codes section above

CompanyCode

30

A/N

Conditional

See Action Codes section above

DateFrom

19

A/N

Required

From date to filter movements

“yyyy/MM/dd hh:mm:ss”

DateTo

19

A/N

Optional

To date to filter movements

“yyyy/MM/dd hh:mm:ss”

\

15. Account Download (POST) – Body Section Format *Response* {.western}
    --------------------------------------------------------

Field Name

Size

Type

Descriptions/Field Value(s)

Id

36

A/N

Current account’s UID

MovementId

36

A/N

Movements’s UID

SubscriberCode

3

A/N

Code of the subscriber who owns the transaction

HostDateTime

19

A/N

ATIONet’s transaction date time “yyyy/mm/dd hh:mm:ss”.

ATIONet Host date time is UCT

DateTime

19

A/N

movement date expressed in subscriber time zone

“yyyy/mm/dd hh:mm:ss”.

SubscriberTimeZone

50

A/N

TimeZone code of the subscriber (abbreviation)

Type

1

N

Internal ATIOnet movement type code

TypeDescription

50

A/N

Movement type description

Origin

1

N

Internal ATIOnet code for the origin of the movement

OriginDescription

50

A/N

Description for the origin of the movement

Description

1000

A/N

Movement description

SubAccountId

36

A/N

SubAccount’s UID

SubAccountExternalCode

50

A/N

SubAccount’s external code

CompanyCode

30

A/N

Company code

Not meaningful for Homebase subscribers

CompanyName

250

A/N

Company name

Not meaningful for Homebase subscribers

ContractCode

20

A/N

Contract code

Not meaningful for Homebase subscribers

SubContractCode

50

A/N

SubContract code

Not meaningful for Homebase subscribers

IsDebit

1

N

Indicates that’s a debit or credit movement

1 = “True”, 2= “False”

FuelMasterCode

50

A/N

Standardized product code. Helps to identify a fuel product category
across multiple Merchant brands and site’s product codes

FuelMasterDescription

100

A/N

Standardized product description. Helps to identify a fuel product
category across multiple Merchant brands and site’s product codes

CurrencyCode

50

A/N

Currency of the amount fields

Amount

10

N

Amount balance for the sub-account.

xxxxxxx.xx

\
\


