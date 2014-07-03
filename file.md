 ATIONet Native Interface API Protocol Specification 

<table>
	<tr>
		<th>Tables</th>
		<th>Are</th>
		<th>Cool</th>
	</tr>
	<tr>
		<td>col 3 is</td>
		<td>sdfs</td>
		<td>dfsdf</td>
	</tr>
	<tr>
		<td>col 3 is</td>
		<td>sdfs</td>
		<td>dfsdf</td>
	</tr>
</table>

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

Document Information

File:

file

Doc Version:

1.3

Release Date:

30, October 2013

Author:

ATIO International LLC

\
\

Change Log

Ver.

Date

Change Summary

1.0

04/Jan/2013

Initial version.

General information\
Actions: Statement Charges (partial)\
 Transactions Download

1.1

07/Jan/2013

Statement Charges\
- Added Action 902 Negative Balance transfer to a sub-account

New group of actions: 941 – 950 Account Inquiries (partial)\
Actions: 941 Sub-account Balance Enquiry\
 942 Sub-account Limit Enquiry

Transactions Downloads\
- Consolidated Classification Fields for Vehicles and Drivers\
- Reorganized Response record, moved Classification fields after Driver
Fields.

1.2

\

\

\
\

**Contents**

[1.Scope 4](#__RefHeading__2823_1988951115)

[1Scope details: 4](#__RefHeading__2825_1988951115)

[2.System Interface API 4](#__RefHeading__2827_1988951115)

[2Interface API Messages 4](#__RefHeading__2829_1988951115)

[3.Data security 4](#__RefHeading__2831_1988951115)

[4.Message Structure 4](#__RefHeading__2833_1988951115)

[5.Error handling 5](#__RefHeading__2835_1988951115)

[6.Statement Charges Interface 5](#__RefHeading__2837_1988951115)

[3Action Codes 5](#__RefHeading__2839_1988951115)

[4Identification 6](#__RefHeading__2841_1988951115)

[5Statement Charge (POST) – Body Section Record Format
6](#__RefHeading__2843_1988951115)

[7.Transactions Download Interface 6](#__RefHeading__2845_1988951115)

[6Action Codes 6](#__RefHeading__2847_1988951115)

[7Transactions Download (POST) – Body Section Format Request
7](#__RefHeading__2849_1988951115)

[8Transactions Download (POST) – Body Section Format Response
7](#__RefHeading__2851_1988951115)

[8.Account Enquiries 20](#__RefHeading__2853_1988951115)

[9Action Codes 20](#__RefHeading__2855_1988951115)

[10Identification 20](#__RefHeading__2857_1988951115)

[11Account Enquiry (POST) – Body Section Record Format Request
20](#__RefHeading__2859_1988951115)

[12Account Enquiry (POST) – Body Section Record Format Response
21](#__RefHeading__2861_1988951115)

[9.Account Downloads 21](#__RefHeading__2863_1988951115)

[13Action Codes 21](#__RefHeading__2865_1988951115)

[14Identification 22](#__RefHeading__2867_1988951115)

[15Account Enquiry (POST) – Body Section Record Format Request
22](#__RefHeading__2869_1988951115)

[16Account Enquiry (POST) – Body Section Record Format Response
22](#__RefHeading__2871_1988951115)

\
\

\
\

\

**Overview**

**Introduction**

This specification is intended to document ATIONet’s Native Interface
API messaging format and related features required for the systems
applying for integration with ATIONet.

The Interface API allows the The following sections provide descriptions
of the messages themselves, the expected behaviour for each supported
action type and a common ground for the functionality of each relevant
item.

**Definitions**

**Subscriber.** ATIONet’s subscription owner. The person or company who
runs the service.

**Homebase.** A type of ATIONet subscription where the subscriber owns
the site(s) but also the fleet(s) of vehicles.

**Network**. A type of ATIONet subscription where the subscriber enrolls
Fleet Companies and retail or commercial sites to operate with its own
method-of-payment. The Network company doesn’t own the site(s) or the
vehicles.

**Merchant**. On a Network type subscription, the Merchant is the
company who own the sites.

**Retail**. A type of ATIONet subscription where the subscriber owns the
sites and enrolls Fleet Companies to operate with its own
method-of-payment.

**Terminal**. **** Transaction capture device at the site.

\

\
\

\
\

\

1.  Scope {.western style="page-break-before: always"}
    =====

Version 1.0 of this document covers a particular version of ATIONet’s
Host protocol. Although feature’s descriptions are generally not related
to a particular version of the protocol, some changes may apply which
would be specifically commented and identified on each feature’s
description paragraph.

1.  Scope details: {.western}
    --------------

Protocol: ATIONet Native Interface API

Version: Version 1.0

API URI: native.ationet.com/v1/interface\
\
\

2.  System Interface API {.western}
    ====================

The Interface API provide system-to-system access to certain features of
ATIONet otherwise only available via the ATIONet Console, and it’s
intended to allow direct interaction of third-party systems on
Subscribers, Merchants and fleet Companies with ATIONet.

Availability of part or all the functionality of the Interface API is
subject to the business type and contract terms of the ATIONet
subscriber.

1.  Interface API Messages {.western}
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

Transactions Download\
[HTTP POST]

931 to 932

1.0

\

Returns a list of completed transactions from ATIONet host, between two
dates, for a given Subscriber, Merchant or fleet Company

Account Enquiries\
[HTTP POST]

941 to 949

1.0

\
\

\
\

\
\

\
\

\
1.2

Returns specific values of a Contract or Sub-account.\
941 – Sub-Account Balance Enquiry\
942 – Sub-Account Limit Enquiry\
\
\

943 – Contract Balance Enquiry\
\

Account Downloads\
[HTTP POST]\
950

1.2

\

950 – Movements Download\
\

3.  Data security {.western}
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
group will return a single JSON-formatted item with the “Response Code”
and “Response Text”. The body of these responses will never be empty.

\

Failure to process the request will be indicated by an HTTP 400’s range
status code. The body will contain a single JSON-formatted item with a
“Response Code” and “Response Text”.

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

Special behavior for ***Home-base*** subscribers

When the subscriber is a HomeBase, the action will first trigger a
Deposit action on the Contract and the Contract to sub-account transfer.

902

Title:

Balance withdrawal from a sub-account

Function:

Withdraws a given value from the global balance of the Contract to the
sub-account related to the Vehicle or Driver.

Sub-account Balance must have enough funds (or product volume) to allow
the withdrawal; otherwise the action will be rejected by the current
accounts subsystem.

Special behavior for ***Home-base*** subscribers

When the subscriber is a HomeBase, the action will reduce the balance of
the sub-account but will not transfer the balance to the Contract.

\
\

4.  Identification {.western}
    --------------

When a Statement Charge is received, ATIONet will try to identify the
Company and the Identifier of the sub-account (Vehicle or Driver), this
can be performed thru several combinations of the Identification Fields
on the body of the message:

1.  Identifier field only. Only accepted for Home-base subscriptions.

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

20

A/N

Optional

See Identification section

ContractCode

20

A/N

Optional

See Identification section

DriverCode

20

A/N

Optional

See Identification section

VehicleCode

20

A/N

Optional

See Identification section

VehiclePlate

20

A/N

Optional

See Identification section

Identifier

20

A/N

Optional

Public ID of the identification device (chipkey ID, account number on a
mag card, RFID serial number, etc.)

See Identification section

MasterProductCode1

4

A/N

Conditional

Required if Charge Volume is specified

ChargeAmount

10

N

Conditional

Either Charge Amount or Charge Volume is required

xxxxxxx.xx

ChargeVolume

10

N

Conditional

Either Charge Amount or Charge Volume is required

xxxxxxx.xx

CurrencyCode

3

A

Conditional

Required if Charge Amount is specified

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

Terminal Id (Optional, if included will act as a filter)

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

Terminal Id

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

20

A/N

Conditional

See Action Codes section above

CompanyCode

20

A/N

Conditional

See Action Codes section above

ContractCode

20

A/N

Optional

See Action Codes section above

TerminalId

8

A/N

Optional

See Action Codes section above

DateFrom

8

A/N

Required

From date to filter transactions

“yyyy/MM/dd hh:mm:ss”

DateTo

8

A/N

Optional

To date to filter transactions, if not specified the ATIONet’s system
date is used (ATIONET’s time-zone is UCT)

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

TransactionSequenceNumber

50

A/N

Transaction ID as received from the site’s controller system. Usually a
transaction counter. Site-based, might repeat from site to site.

AuthorizationCode

9

A/N

Authorization Code

ResponseCode

5

N

Host response code sent to the terminal

ResponseText

50

A/N

Host response text sent to the terminal

Status

\

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

15

A/N

ATIONet’s transaction datetime “yyyymmdd hhmmss”.

ATIONet Host time is UCT

LocalTimeZone

6

A/N

Time zone code of the site (abbreviation)

LocalTransactionDateTime

13/15

A/N

Site’s transaction date “yyyymmdd hhmmss” or “yymmdd hhmm” if the site’s
controller does not include seconds precision.

MerchantCode

20

A/N

Code of the company who owns the site

N/A to Homebase subscribers

SiteCode

20

A/N

Site Code

SiteName

100

A/N

Name of the Site

TerminalCode

8

A/N

Site’s Terminal identification code.

A Terminal is the device or system that captures the transaction at the
site, depending on the controller (system) type at the site, it may be
the actual terminal (for example the specific OPT) or the whole system
(several OPTs served by a single controller).

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

7

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

3

A/N

Unit of measuring for the volume fields, according to site’s
configuration.

CurrencyCode

3

A/N

Currency of the amount fields, according to site’s configuration

ProductCode

4

N

Site’s product code

MasterProductDescription

50

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

11

N

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

FuelUsage

50

A/N

Fuel consumption as captured by the terminal at transaction time

FuelTaxFlag

50

A/N

Reserved

CompanyCode

20

A/N

Company code

Not meaningful for Homebase subscribers

ContractCode

20

A/N

Contract code

Not meaningful for Homebase subscribers

FleetCode

20

A/N

Fleet Code

FleetName

50

A/N

Fleet Name

VehicleLicencePlate

50

A/N

Licence plate

VehicleClassDescription

50

A/N

Vehicle Class

DriverName

100

A/N

Name of Driver

DriverLicenceState

5

A/N

Driver licence jurisdiction

DriverLicenceNumber

10

A/N

Driver licence

DriverID

10

N

DriverID prompt result

ClassificationLabel1

200

A/N

Classifications

ATIONet allows for up to four user-defined classification field for
Vehicles or Drivers.

ClassificationValue1

50

A/N

\

ClassificationLabel2

200

A/N

\

ClassificationValue2

50

A/N

\

ClassificationLabel3

200

A/N

\

ClassificationValue3

50

A/N

\

ClassificationLabel4

200

A/N

\

ClassificationValue4

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

10

N

Truck Unit ID prompt result

TrailerNumber

10

N

Trailer ID prompt result

TripNumber

10

N

Trip/Guide/Route prompt result

PurchaseOrderNumber

10

N

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

Thus, this message should not be used to obtain the authorization limit
for a transaction. The Sub-Account Limit Enquiry (942) should be used
instead.

942

Title:

Sub-Account Limit Enquiry

Function:

This message tests a pre-authorization transaction based on submitted
data and returns the authorization limits that such transaction would
return.

943

Title:

Contract Balance Enquiry

Function:

Retrieves the total Balance for a given Contract. Works with product or
money based contracts. May return multiple product-volume pairs when the
contract has multiple balance totals.

\
\

10. Identification {.western}
    --------------

When an Account Enquiry is received, ATIONet will try to identify the
Company and the Identifier of the sub-account (Vehicle or Driver), this
can be performed thru several combinations of the Identification Fields
on the body of the message:

1.  Identifier field only. Only accepted for Home-base subscriptions.

2.  Company Code + Identifier.

3.  Company Code + Contract Code + (Driver Code or Vehicle Code or
    Vehicle Plate)

11. Account Enquiry (POST) – Body Section Record Format *Request* {.western}
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

    20

    A/N

    Optional

    See Identification section

    ContractCode

    20

    A/N

    Optional

    See Identification section

    DriverCode

    20

    A/N

    Optional

    See Identification section

    VehicleCode

    20

    A/N

    Optional

    See Identification section

    VehiclePlate

    20

    A/N

    Optional

    See Identification section

    Identifier

    20

    A/N

    Optional

    Public ID of the identification device (chipkey ID, account number
    on a mag card, RFID serial number, etc.)

    See Identification section

    ProductCode

    4

    A/N

    Conditional

    Required if Charge Volume is specified

    ChargeAmount

    10

    N

    Conditional

    Either Charge Amount or Charge Volume is required

    xxxxxxx.xx

    ChargeVolume

    10

    N

    Conditional

    Either Charge Amount or Charge Volume is required

    xxxxxxx.xx

    CurrencyCode

    3

    A

    Conditional

    Required if Charge Amount is specified

12. Account Enquiry (POST) – Body Section Record Format *Response* {.western}
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

20

A/N

Company identification. Should be ignored on Homebase subscribers.

ContractCode

20

A/N

Contract identification. Should be ignored on Homebase subscribers.

DriverCode

20

A/N

See Identification section

VehicleCode

20

A/N

See Identification section

VehiclePlate

20

A/N

See Identification section

Identifier

20

A/N

Public ID of the identification device (chipkey ID, account number on a
mag card, RFID serial number, etc.)

See Identification section

ProductCode1

4

A/N

Master Product Code. Empty if contract is money based.

ProductVolume1

10

N

Volume balance for Product 1. Empty if contract is money based.

xxxxxxx.xx

ProductCode2

4

A/N

Master Product Code. Empty if contract is money based or there is only
one product configured for that Vehicle or Driver

ProductVolume2

10

N

Volume balance for Product 2. Empty if contract is money based or there
is only one product configured for that Vehicle or Driver.

xxxxxxx.xx

ProductCode3

4

A/N

Master Product Code. Empty if contract is money based or there are less
than three products configured for that Vehicle or Driver.

ProductVolume2

10

N

Volume balance for Product 2. Empty if contract is money based or there
are less than three products configured for that Vehicle or Driver.

xxxxxxx.xx

CurrencyCode

3

A

Currency configured for the Contract

MoneyBalance

3

N

Amount balance for the sub-account. Empty if the account is
product-based.

xxxxxxx.xx

\
\

9.  Account Downloads {.western}
    =================

The Account Downloads messages retrieve data from ATIONet, specific to a
Contract or Sub-Account (Vehicle or Driver types).

Depending on the type of enquiry, this message might be used by one or
the other party of the contract (the subscriber or the fleet company).

13. Action Codes {.western}
    ------------

The Action Code specifies the type of enquiry requested. The submitted
code must match one of the pre-defined operation types. Not all
operation types are available for all subscribers and/or fleet
companies; availability depends on subscription types but also on
contract terms with ATIONet.

Action Code

Description

944

Title:

Sub-Account Movements Download

Function:

Retrieves a list of movements from the Current Accounts sub-system for a
given Sub-account (Vehicle or Driver types) according to a specified
filter.

945

Title:

Contract Movements Download

Function:

Retrieves a list of movements from the Current Accounts sub-system for a
given Contract according to a specified filter.

\
\

14. Identification {.western}
    --------------

When an Account Enquiry is received, ATIONet will try to identify the
Company and the Identifier of the sub-account (Vehicle or Driver), this
can be performed thru several combinations of the Identification Fields
on the body of the message:

4.  Identifier field only. Only accepted for Home-base subscriptions.

5.  Company Code + Identifier.

6.  Company Code + Contract Code + (Driver Code or Vehicle Code or
    Vehicle Plate)

15. Account Enquiry (POST) – Body Section Record Format *Request* {.western}
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

    20

    A/N

    Optional

    See Identification section

    ContractCode

    20

    A/N

    Optional

    See Identification section

    DriverCode

    20

    A/N

    Optional

    See Identification section

    VehicleCode

    20

    A/N

    Optional

    See Identification section

    VehiclePlate

    20

    A/N

    Optional

    See Identification section

    Identifier

    20

    A/N

    Optional

    Public ID of the identification device (chipkey ID, account number
    on a mag card, RFID serial number, etc.)

    See Identification section

    ProductCode

    4

    A/N

    Conditional

    Required if Charge Volume is specified

    ChargeAmount

    10

    N

    Conditional

    Either Charge Amount or Charge Volume is required

    xxxxxxx.xx

    ChargeVolume

    10

    N

    Conditional

    Either Charge Amount or Charge Volume is required

    xxxxxxx.xx

    CurrencyCode

    3

    A

    Conditional

    Required if Charge Amount is specified

16. Account Enquiry (POST) – Body Section Record Format *Response* {.western}
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

20

A/N

Company identification. Should be ignored on Homebase subscribers.

ContractCode

20

A/N

Contract identification. Should be ignored on Homebase subscribers.

DriverCode

20

A/N

See Identification section

VehicleCode

20

A/N

See Identification section

VehiclePlate

20

A/N

See Identification section

Identifier

20

A/N

Public ID of the identification device (chipkey ID, account number on a
mag card, RFID serial number, etc.)

See Identification section

ProductCode1

4

A/N

Master Product Code. Empty if contract is money based.

ProductVolume1

10

N

Volume balance for Product 1. Empty if contract is money based.

xxxxxxx.xx

ProductCode2

4

A/N

Master Product Code. Empty if contract is money based or there is only
one product configured for that Vehicle or Driver

ProductVolume2

10

N

Volume balance for Product 2. Empty if contract is money based or there
is only one product configured for that Vehicle or Driver.

xxxxxxx.xx

ProductCode3

4

A/N

Master Product Code. Empty if contract is money based or there are less
than three products configured for that Vehicle or Driver.

ProductVolume2

10

N

Volume balance for Product 2. Empty if contract is money based or there
are less than three products configured for that Vehicle or Driver.

xxxxxxx.xx

CurrencyCode

3

A

Currency configured for the Contract

MoneyBalance

3

N

Amount balance for the sub-account. Empty if the account is
product-based.

xxxxxxx.xx

\
\


